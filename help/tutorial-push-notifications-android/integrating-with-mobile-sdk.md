---
title: 'Schritt 2: Integrieren des Mobile SDK'
description: In diesem Teil werden wir die Android-App mit dem Mobile SDK integrieren. So integrieren Sie das mobile SDK in die Android-App
feature: Push
topics: Mobile
kt: 4826
doc-type: tutorial
activity: use
team: TM
translation-type: tm+mt
source-git-commit: 13b4f1d395dfe53f9fc5263e7b06be700e30b986
workflow-type: tm+mt
source-wordcount: '164'
ht-degree: 3%

---

# SCHRITT 2 - Integrieren von [!UICONTROL Mobile SDK] in die Android-App

In diesem Teil integrieren wir die [!DNL Android]-App mit [!UICONTROL Mobile SDK]. Gehen Sie wie folgt vor, um [!UICONTROL mobiles SDK] in die [!DNL Android]-App zu integrieren:

* Öffnen Sie das Projekt *ACSPushTutorial* in [!DNL Android Studio]
* Erstellen Sie eine neue Java-Klasse mit dem Namen *MainApp*, die [!DNL android.app.Application] erweitert
* Ihre Projektstruktur sollte an dieser Stelle wie unten aussehen

![main-app](assets/android-main-app.PNG)

* Erweitern Sie den Ordner [!DNL Gradle Scripts]. Dublette klicken Sie auf das [!DNL build.gradle] des Moduls. Fügen Sie die folgenden Abhängigkeiten in den Abschnitt Abhängigkeiten der Datei [!DNL build.gradle] ein. Die [!DNL build.gradle]-Datei sollte jetzt wie folgt aussehen:

<!--
Removed `{.line-numbers}` below
-->

```java
implementation 'com.adobe.marketing.mobile:campaign:1.+'
implementation 'com.adobe.marketing.mobile:userprofile:1.+'
implementation 'com.adobe.marketing.mobile:sdk-core:1.+'
```

![module-gradle](assets/module-build-gradle.PNG)

* Synchronisieren Sie Ihr [!DNL Android]-Projekt, indem Sie auf die Schaltfläche Jetzt synchronisieren klicken, um Ihr Projekt zu synchronisieren.

## Ändern [!DNL AndroidManifest.xml]{#modify-android-manifest}

Öffnen Sie *AndroidManifest.xml* und fügen Sie die folgenden 2 Zeilen nach dem Manifestelement und vor dem Anwendungselement ein. Dadurch kann Ihre App mit externen Nutzern kommunizieren

<!--
Removed `{.line-numbers}` below
-->

```xml
<uses-permission android:name="android.permission.INTERNET" />
<uses-permission android:name="android.permission.ACCESS_NETWORK_STATE" />
```

Kopieren Sie die folgende Zeile im Anwendungselement
[!DNL android:name=".MainApp"]
Speichern Sie [!DNL AndroidManifest.xml]
Ihr [!DNL AndroidManifest.xml] sollte wie folgt aussehen:

<!--
Removed `{.line-numbers}` below
-->

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
