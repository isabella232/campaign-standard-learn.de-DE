---
title: 'Schritt 2: Integrieren des Mobile SDK'
description: In diesem Teil integrieren wir die Android-App mit dem Mobile SDK. So integrieren Sie das mobile SDK in die Android-App
feature: Push
kt: 4826
doc-type: tutorial
activity: use
team: TM
exl-id: 0fa53536-8330-4e96-be2f-afc078609bcd
source-git-commit: ada0b029245190f53d58fa93c79c161719bfe9fd
workflow-type: tm+mt
source-wordcount: '164'
ht-degree: 3%

---

# SCHRITT 2: Integrieren [!UICONTROL Mobile SDK] mit Android-App

In diesem Teil werden wir die [!DNL Android] App mit [!UICONTROL Mobile SDK]. Integration [!UICONTROL Mobile SDK] mit dem [!DNL Android] App verwenden, führen Sie die folgenden Schritte aus:

* Öffnen Sie die *ACSPushTutorial* Projekt in [!DNL Android Studio]
* Erstellen Sie eine neue Java-Klasse mit dem Namen *MainApp* , die [!DNL android.app.Application]
* Ihre Projektstruktur sollte an dieser Stelle wie unten dargestellt aussehen

![main-app](assets/android-main-app.PNG)

* Erweitern Sie die [!DNL Gradle Scripts] Ordner. Doppelklicken Sie auf [!DNL build.gradle] des Moduls. Fügen Sie die folgenden Abhängigkeiten in den Abschnitt &quot;Abhängigkeiten&quot;des [!DNL build.gradle] -Datei. Ihre [!DNL build.gradle] -Datei sollte wie unten dargestellt aussehen

<!--
Removed `{.line-numbers}` below
-->

```java
implementation 'com.adobe.marketing.mobile:campaign:1.+'
implementation 'com.adobe.marketing.mobile:userprofile:1.+'
implementation 'com.adobe.marketing.mobile:sdk-core:1.+'
```

![module-gradle](assets/module-build-gradle.PNG)

* Synchronisieren [!DNL Android] Projekt durch Klicken auf die Schaltfläche Jetzt synchronisieren , um Ihr Projekt zu synchronisieren

## Ändern [!DNL AndroidManifest.xml]{#modify-android-manifest}

Öffnen *AndroidManifest.xml* und fügen Sie die folgenden 2 Zeilen nach dem Manifestelement und vor dem Anwendungselement ein. Dadurch kann Ihre App mit der Außenwelt kommunizieren

<!--
Removed `{.line-numbers}` below
-->

```xml
<uses-permission android:name="android.permission.INTERNET" />
<uses-permission android:name="android.permission.ACCESS_NETWORK_STATE" />
```

Kopieren Sie die folgende Zeile im Anwendungselement
[!DNL android:name=".MainApp"]
Speichern Sie Ihre [!DNL AndroidManifest.xml]
Ihre [!DNL AndroidManifest.xml] sollte wie folgt aussehen:

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
