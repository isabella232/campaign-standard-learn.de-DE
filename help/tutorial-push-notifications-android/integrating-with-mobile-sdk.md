---
title: 'Schritt 2: Integration des Mobile SDK'
description: In diesem Teil werden wir die Android-App mit dem Mobile SDK integrieren. So integrieren Sie das mobile SDK in die Android-App
feature: Push
topics: Mobile
kt: 4826
doc-type: tutorial
activity: use
team: TM
translation-type: tm+mt
source-git-commit: c3ff1a137fb8ee9506a11f82e1a27d010bbd97e6
workflow-type: tm+mt
source-wordcount: '164'
ht-degree: 0%

---

# SCHRITT 2 - Integration des [!UICONTROL Mobile SDK] mit der Android-App

In diesem Teil integrieren wir die [!DNL Android] App in das [!UICONTROL Mobile SDK]. Gehen Sie wie folgt vor, um [!UICONTROL mobiles SDK] in die [!DNL Android] App zu integrieren:

* Öffnen Sie das *ACSPushTutorial* -Projekt in [!DNL Android Studio]
* Erstellen Sie eine neue Java-Klasse mit dem Namen *MainApp* , die [!DNL android.app.Application]
* Ihre Projektstruktur sollte an dieser Stelle wie unten aussehen

![main-app](assets/android-main-app.PNG)

* Erweitern Sie den [!DNL Gradle Scripts] Ordner. Dublette klicken Sie auf das Modul [!DNL build.gradle] . Fügen Sie die folgenden Abhängigkeiten in den Abschnitt Abhängigkeiten der [!DNL build.gradle] Datei ein. Ihre [!DNL build.gradle] Datei sollte jetzt wie folgt aussehen

```java
implementation 'com.adobe.marketing.mobile:campaign:1.+'
implementation 'com.adobe.marketing.mobile:userprofile:1.+'
implementation 'com.adobe.marketing.mobile:sdk-core:1.+'
```

![module-gradle](assets/module-build-gradle.PNG)

* Synchronisieren Sie Ihr [!DNL Android] Projekt, indem Sie auf die Schaltfläche Jetzt synchronisieren klicken, um Ihr Projekt zu synchronisieren

## Ändern [!DNL AndroidManifest.xml]{#modify-android-manifest}

Öffnen Sie *AndroidManifest.xml* und fügen Sie die folgenden 2 Zeilen nach dem Manifestelement und vor dem Anwendungselement ein. Dadurch kann Ihre App mit externen Nutzern kommunizieren

```xml
<uses-permission android:name="android.permission.INTERNET" />
<uses-permission android:name="android.permission.ACCESS_NETWORK_STATE" />
```

Kopieren Sie die folgende Zeile im Anwendungselement[!DNL android:name=".MainApp"]Speichern Sie Ihren [!DNL AndroidManifest.xml]Code, der wie folgt aussehen [!DNL AndroidManifest.xml] soll

```xml
<?xml version="1.0" encoding="utf-8"?>
<manifest xmlns:android="http://schemas.android.com/apk/res/android"
    package="com.example.acspushtutorial">
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

<activity android:name=".MainActivity">
<intent-filter>
    <action android:name="android.intent.action.MAIN" />
    <category android:name="android.intent.category.LAUNCHER" />
</intent-filter>
</activity>
</application>

</manifest>
```
