---
title: 'Schritt 3: Registrieren der Erweiterungen für Ihre Mobile App'
description: In diesem Teil fügen wir den Code zur Registrierung der UserProfile-, Identity-, Lifecycle- und Signal-Erweiterungen hinzu.
feature: Push
kt: 4827
doc-type: tutorial
activity: use
team: TM
exl-id: d8c0d8c6-2e04-4c27-b27a-d0de79dd953b
source-git-commit: ada0b029245190f53d58fa93c79c161719bfe9fd
workflow-type: tm+mt
source-wordcount: '129'
ht-degree: 14%

---

# Schritt 3: Registrieren der Erweiterungen für Ihre Mobile App

In diesem Teil fügen wir den Code hinzu, um die Erweiterungen Benutzerprofil, Identität, Lebenszyklus und Signal zu registrieren. Diese Erweiterungen sind Teil von [[!UICONTROL Mobile Core-Erweiterungen]](https://aep-sdks.gitbook.io/docs/using-mobile-extensions/mobile-core). Außerdem müssen wir die Adobe Campaign Standard-Erweiterung registrieren, wie im folgenden Code dargestellt.

Öffnen Sie Ihr Projekt in [!DNL Android] Studio. Den gesamten Code in MainApp löschen **mit Ausnahme der ersten Zeile, die Ihre Paketanweisung ist**.

Fügen Sie den folgenden Code in MainApp ein

<!--
Removed `{.line-numbers}` below
-->

```java
import [!DNL android].app.Application;
import android.util.Log;

import com.adobe.marketing.mobile.AdobeCallback;
import com.adobe.marketing.mobile.Campaign;
import com.adobe.marketing.mobile.Identity;
import com.adobe.marketing.mobile.InvalidInitException;
import com.adobe.marketing.mobile.Lifecycle;
import com.adobe.marketing.mobile.LoggingMode;
import com.adobe.marketing.mobile.MobileCore;
import com.adobe.marketing.mobile.Signal;
import com.adobe.marketing.mobile.UserProfile;

public class MainApp extends Application {

@Override
public void onCreate() {
super.onCreate();

MobileCore.setApplication(this);
MobileCore.setLogLevel(LoggingMode.DEBUG);

try{
    Campaign.registerExtension();
    UserProfile.registerExtension();
    Identity.registerExtension();
    Lifecycle.registerExtension();
    Signal.registerExtension();
    MobileCore.start(new AdobeCallback () {
        @Override
        public void call(Object o) {
            MobileCore.configureWithAppID("copy your launch property id here");
        }
    });
} catch (InvalidInitException e) {
    Log.d("ACS Exception", "exception");
}
}
}
```

Zeile 32:[!UICONTROL  Launch] Die Umgebungsdatei-ID der Eigenschaft. Der Zugriff darauf erfolgt über die [!UICONTROL Umgebungs-Tab] Ihrer [!UICONTROL Launch] -Eigenschaft.

![launch-id](assets/launch-id-property.PNG)
