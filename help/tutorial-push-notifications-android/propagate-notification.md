---
title: 'Schritt 5: Propagate-Benachrichtigungen'
description: In diesem Teil werden wir die vom Adobe Campaign empfangene Nachricht mit Android Notification Manager.Firebase weiterleiten
feature: Push
topics: Mobile
kt: 4829
doc-type: tutorial
activity: use
team: TM
translation-type: tm+mt
source-git-commit: 13b4f1d395dfe53f9fc5263e7b06be700e30b986
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# hinzufügen Dienst zum Senden der Benachrichtigung

In diesem Teil werden wir die Nachricht, die wir von Adobe Campaign erhalten haben, mit [!DNL Android Notification Manager]. [!DNL Notification manager] wird verwendet, um den Benutzer über Ereignis zu informieren, die auftreten.
So teilen Sie dem Benutzer mit, dass im Hintergrund etwas passiert ist:

* Start [!DNL Android Studio]
* Projekt öffnen *[!DNL ACSPushTutorial]*
* Projektstruktur erweitern
* Klicken Sie mit der rechten Maustaste auf den Paketordner ([!DNL com.example.acspushtutorial]) und [!DNL New ->Java Class]
* Benennen Sie diese Klasse *[!DNL MyService]* und stellen Sie sicher, dass sie erweitert wird [!DNL FirebaseMessagingService]
* Create *[!DNL sendNotification]* method in this class. Bei dieser Methode müssen Sie den Inhalt und den Kanal der Benachrichtigung mit einem [!DNL NotificationCompat.Builder] Objekt festlegen. Um die Benachrichtigung anzuzeigen, rufen Sie [!DNL NotificationManagerCompat.notify()]an und übergeben Sie ihr eine eindeutige ID für die Benachrichtigung und das Ergebnis von [!DNL NotificationCompat.Builder.build()].

<!--
Removed `{.line-numbers}` below
-->

```java
package com.example.pushmessaging;
import android.app.NotificationChannel;
import android.app.NotificationManager;
import android.app.PendingIntent;
import android.content.Context;
import android.content.Intent;
import android.media.RingtoneManager;
import android.net.Uri;
import android.os.Build;
import android.util.Log;

import androidx.core.app.NotificationCompat;

import com.google.firebase.messaging.FirebaseMessagingService;
import com.google.firebase.messaging.RemoteMessage;

import java.util.Map;

public class MyService extends FirebaseMessagingService {
@Override
public void onMessageReceived(RemoteMessage remoteMessage)
{
Map<String,String> data  = remoteMessage.getData();
Log.d("data payload: ", data.toString());
sendNotification(remoteMessage);
}


private void sendNotification(RemoteMessage message) {
Intent intent = new Intent(this, MainActivity.class);
intent.addFlags(Intent.FLAG_ACTIVITY_CLEAR_TOP);
PendingIntent pendingIntent = PendingIntent.getActivity(this, 0 /* Request code */, intent, PendingIntent.FLAG_ONE_SHOT);

String channelId = "0";
Uri defaultSoundUri = RingtoneManager.getDefaultUri(RingtoneManager.TYPE_NOTIFICATION);
NotificationCompat.Builder notificationBuilder =
        new NotificationCompat.Builder(this, channelId)
                .setSmallIcon(R.drawable.ic_launcher_background)
                .setContentTitle("Message from AEM")
                .setContentText(message.getData().get("body"))
                .setAutoCancel(true)
                .setSound(defaultSoundUri)
                .setContentIntent(pendingIntent);

NotificationManager notificationManager =
        (NotificationManager) getSystemService(Context.NOTIFICATION_SERVICE);

// Since android Oreo notification channel is needed.
if (Build.VERSION.SDK_INT >= Build.VERSION_CODES.O) {
    NotificationChannel channel = new NotificationChannel(channelId,
            "Channel human readable title",
            NotificationManager.IMPORTANCE_DEFAULT);
    notificationManager.createNotificationChannel(channel);
}

notificationManager.notify(0 /* ID of notification */, notificationBuilder.build());
}
}
```

## Ändern [!DNL AndroidManifest.xml]

hinzufügen Sie den Dienst, der für Sie erstellt wurde [!DNL AndroidManifest.xml]. Das endgültige Ergebnis [!DNL AndroidManifest.xml] sollte wie folgt aussehen:

<!--
Removed `{.line-numbers}` below
-->

```xml
<?xml version="1.0" encoding="utf-8"?>
<manifest xmlns:android="http://schemas.android.com/apk/res/android"
    package="com.example.pushmessaging">

    <uses-permission android:name="android.permission.INTERNET" />
    <uses-permission android:name="android.permission.ACCESS_NETWORK_STATE" />

    <application
        android:name=".MainApp"
        android:allowBackup="true"
        android:icon="@mipmap/ic_launcher"
        android:label="@string/app_name"
        android:roundIcon="@mipmap/ic_launcher_round"
        android:supportsRtl="true"
        android:theme="@style/AppTheme">
        <service
            android:name=".MyService"
            android:exported="false">
            <intent-filter>
                <action android:name="com.google.firebase.MESSAGING_EVENT" />
            </intent-filter>
        </service>

        <activity android:name=".MainActivity">
            <intent-filter>
                <action android:name="android.intent.action.MAIN" />

                <category android:name="android.intent.category.LAUNCHER" />
            </intent-filter>
        </activity>
    </application>

</manifest>
```

## App ausführen

Führen Sie die App aus, indem Sie auf den **grünen Pfeil** in der Symbolleiste oder im [!DNL Run] Menü klicken.
