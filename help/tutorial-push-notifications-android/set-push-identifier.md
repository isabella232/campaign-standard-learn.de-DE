---
title: SCHRITT 4 - Festlegen des Pushidentifizierers
description: Der **pushIdentifier** ist eine Zeichenfolge, die das Gerätetoken für Push-Benachrichtigungen enthält. Dies ist dasselbe Token, das von Firebase gesendet und mit der MobileCore.setPushIdentifier-Methode an das SDK übergeben wird.
feature: Push
topics: MOBILE
kt: 4828
doc-type: tutorial
activity: use
team: TM
translation-type: tm+mt
source-git-commit: a2f194821a9ce06272eaed979ee2d8c62cccac2b
workflow-type: tm+mt
source-wordcount: '221'
ht-degree: 0%

---

# Schritt 4: Festlegen [!DNL pushidentifier]

Die Zeichenfolge **[!DNL pushidentifier]** enthält das Gerätetoken für [!DNL Push] Benachrichtigungen. Dies ist dasselbe Token, das von gesendet wird [!DNL Firebase] und mit der [!DNL MobileCore.setPushIdentifier] -Methode an das SDK übergeben wird.

Öffnen Sie Ihr Projekt im [!DNL Android ]Studio. Löschen Sie den gesamten Code [!DNL MainActivity] mit Ausnahme der ersten Zeile, die Ihre Paketanweisung **** ist.

Fügen Sie den folgenden Code ein in [!DNL MainActivity]:

```java{.line-numbers}
import androidx.annotation.NonNull;
import androidx.appcompat.app.AppCompatActivity;

import android.os.Bundle;
import android.util.Log;
import android.widget.Toast;

import com.adobe.marketing.mobile.MobileCore;
import com.google.android.gms.tasks.OnCompleteListener;
import com.google.android.gms.tasks.Task;
import com.google.firebase.iid.FirebaseInstanceId;
import com.google.firebase.iid.InstanceIdResult;

public class MainActivity extends AppCompatActivity {

@Override
protected void onCreate(Bundle savedInstanceState) {
super.onCreate(savedInstanceState);
setContentView(R.layout.activity_main);

registerToken();
}

void registerToken() {
FirebaseInstanceId.getInstance().getInstanceId()
    .addOnCompleteListener(new OnCompleteListener<InstanceIdResult>() {
        @Override
        public void onComplete(@NonNull Task<InstanceIdResult> task) {
            if (!task.isSuccessful()) {
                Log.w("Message App", "getInstanceId failed", task.getException());
                return;
            }

// Get new Instance ID token
String token = task.getResult().getToken();

Log.d("Got token", token);

MobileCore.setPushIdentifier(token);
}
});
}

@Override
public void onResume() {
super.onResume();
MobileCore.setApplication(getApplication());
MobileCore.lifecycleStart(null);
}

@Override
public void onPause() {
super.onPause();
MobileCore.lifecyclePause();
}
}
```

## App testen

Jetzt ist es eine gute Zeit, Ihre App zu testen, bevor Sie weitermachen.

* Führen Sie die App aus, indem Sie auf den grünen Pfeil klicken oder **[!DNL Run->Run'app']** auswählen.
* Der [!DNL Android] Emulator sollte Beginn enthalten, und die App sollte mit [!DNL "Hello World" ]Text ausgeführt werden.
* Öffnen Sie das [!DNL logcat] Fenster. Suchen Sie nach &quot;[!DNL Got]&quot;. Sie sollten das Token sehen, das Sie aus dem [!DNL Firebase] Schreiben in das Protokoll erhalten haben, wie unten gezeigt. Die lange Zeichenfolge nach &quot;[!DNL Got token]&quot;ist die Zeichenfolge, [!DNL pushidentifier ]die an Adobe Campaign gesendet wird.

![logcat-token](assets/logcat-got-token.PNG)

### Mobilanwendungs-Abonnenten überprüfen

Melden Sie sich bei Ihrer Adobe Campaign Standard-Instanz an.
Navigieren Sie zu **[!UICONTROL Administration->Kanal->Mobile App(AEP SDK)]**. Öffnen Sie die entsprechende Mobilanwendung. Registerkarte zur Registerkarte [!UICONTROL Mobilanwendungs-Abonnenten] . Es sollte ein [!UICONTROL Registrierungstoken ]angezeigt werden.

![mobile-application-subscribers](assets/mobile-application-subscribers.PNG)

>[HINWEIS]
>
>Wenn das Registrierungstoken auf der Registerkarte &quot;Abonnenten [!UICONTROL von] Mobilanwendungen&quot;nicht angezeigt wird, beenden Sie hier den Vorgang, bevor Sie fortfahren.
