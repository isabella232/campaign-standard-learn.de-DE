---
title: 'Schritt 3: Registrieren der Erweiterungen für Ihre Mobile App'
description: In diesem Teil werden wir den Code zur Registrierung der UserProfile, Identity, Lifecycle und Signal Extensions hinzufügen.
feature: Push-Benachrichtigung
kt: 4827
doc-type: tutorial
activity: use
team: TM
exl-id: d8c0d8c6-2e04-4c27-b27a-d0de79dd953b
translation-type: tm+mt
source-git-commit: ada0b029245190f53d58fa93c79c161719bfe9fd
workflow-type: tm+mt
source-wordcount: '130'
ht-degree: 15%

---

# Schritt 3: Registrieren der Erweiterungen für Ihre Mobile App

In diesem Teil werden wir den Code zur Registrierung des User Profil, Identity, Lifecycle und Signal Extensions hinzufügen. Diese Erweiterungen sind Teil von [[!UICONTROL Mobile Core Extensions]](https://aep-sdks.gitbook.io/docs/using-mobile-extensions/mobile-core). Wir müssen auch die Adobe Campaign Standard-Erweiterung registrieren, wie im folgenden Code dargestellt.

Öffnen Sie Ihr Projekt im Studio [!DNL Android]. Löschen Sie den gesamten Code in MainApp **mit Ausnahme der ersten Zeile, die Ihre Paketanweisung** ist.

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

In Zeile 32 müssen Sie die Umgebung-ID der Eigenschaft für &quot;Start[!UICONTROL &quot;angeben. ] Dies ist über die Registerkarte [!UICONTROL Umgebung] Ihrer [!UICONTROL Eigenschaft Launch] möglich.

![launch-id](assets/launch-id-property.PNG)
