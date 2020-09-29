---
title: 'Schritt 3: Erweiterungen für Ihre mobile App registrieren'
description: In diesem Teil werden wir den Code zur Registrierung der UserProfile, Identity, Lifecycle und Signal Extensions hinzufügen.
feature: Push
topics: Mobile
kt: 4827
doc-type: tutorial
activity: use
team: TM
translation-type: tm+mt
source-git-commit: 13b4f1d395dfe53f9fc5263e7b06be700e30b986
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---


# Schritt 3: Erweiterungen für Ihre mobile App registrieren

In diesem Teil werden wir den Code zur Registrierung des User Profil, Identity, Lifecycle und Signal Extensions hinzufügen. Diese Erweiterungen sind Teil der [[!UICONTROL Mobile Core Extensions]](https://aep-sdks.gitbook.io/docs/using-mobile-extensions/mobile-core). Wir müssen auch die Adobe Campaign Standard-Erweiterung registrieren, wie im folgenden Code dargestellt.

Öffnen Sie Ihr Projekt im [!DNL Android] Studio. Löschen Sie den gesamten Code in MainApp, **mit Ausnahme der ersten Zeile, die Ihre Paketanweisung** ist.

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

In Zeile 32 müssen Sie die Umgebung-ID Ihrer[!UICONTROL  Launch] -Eigenschaft angeben. Dies ist über die Registerkarte &quot; [!UICONTROL Umgebung&quot;] der Eigenschaft &quot; [!UICONTROL Launch] &quot;möglich.

![launch-id](assets/launch-id-property.PNG)
