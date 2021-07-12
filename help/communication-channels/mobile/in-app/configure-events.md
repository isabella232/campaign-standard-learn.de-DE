---
title: Konfigurieren von Ereignissen
description: '"Erfahren Sie, wie Ereignisse definieren, welche vom Benutzer initiierte Aktion eine In-App-Nachricht Trigger, die angezeigt werden soll. "'
feature: In-App
kt: 2548
thumbnail: 26245.jpg
doc-type: feature video
activity: use
team: TM
exl-id: 2c7937f4-b0da-46e5-934e-c660012c2c6f
role: User, Developer
level: Beginner, Intermediate
source-git-commit: 2be2719ddd84490b796d9abc6300376fa896ff0c
workflow-type: tm+mt
source-wordcount: '257'
ht-degree: 8%

---

# [!UICONTROL Ereignisse] konfigurieren {#configuring-events}

Bei der Konfiguration einer [!UICONTROL In-App]-Nachricht müssen Sie definieren, welche vom Benutzer initiierte Aktion die Nachricht Trigger. Diese Aktionen werden als [!UICONTROL Ereignisse] bezeichnet. Drei Kategorien von [!UICONTROL Ereignissen] sind verfügbar: [!UICONTROL Mobile-App-Ereignisse], [!UICONTROL Life-Cycle-Ereignisse] und [!UICONTROL Analytics-Ereignisse].

## [!UICONTROL Mobile-App-Ereignisse] {#mobile-application-events}

[!UICONTROL Mobile-App-] Ereignisse sind  [!UICONTROL benutzerdefinierte ] Ereignisse, die in Ihrer Mobile App implementiert sind.

Beispiele:

* Ein Kunde hat einen Artikel angesehen
* Ein Kunde fügt einen Artikel zum Warenkorb hinzu
* Stehen gelassener Warenkorb
* Ein Kunde hat etwas gekauft

Sie müssen diese [!UICONTROL Ereignisse] in Adobe Campaign konfigurieren. Im folgenden Video wird beschrieben, wie Sie dies durchführen.

>[!VIDEO](https://video.tv.adobe.com/v/26245?quality=12)

## [!UICONTROL Lebenszyklusereignisse] {#life-cycle-events}

[!UICONTROL Lebenszyklusereignisse ] sind vordefinierte  [!UICONTROL Ereignisse]. Die folgenden [!UICONTROL Ereignisse] sind verfügbar:

* [!UICONTROL gestartet]
* [!UICONTROL aktualisiert]
* [!UICONTROL abgestürzt]

Ein Anwendungsbeispiel könnte eine Nachricht sein, die nach einem Upgrade neue Funktionen einführt, oder eine Ereignispromotion.

>[!NOTE]
>
>Das [!UICONTROL Lebenszyklusmodul] muss in der Mobile App konfiguriert werden. Weitere Informationen zu [Hinzufügen des Lebenszyklus zu Ihrer App](https://aep-sdks.gitbook.io/docs/using-mobile-extensions/mobile-core/lifecycle) finden Sie hier .

## [!UICONTROL Analytics-Ereignisse] {#analytics-events}

Je nach der Konfiguration Ihrer App werden die folgenden drei Kategorien unterstützt:

* Adobe Analytics
* [!UICONTROL Kontextdaten]
* [!UICONTROL Ansichtsstatus]

>[!NOTE]
>
>[!UICONTROL Für Analytics-] Ereignisse ist eine Adobe Analytics-Lizenz erforderlich. Sobald Sie die [[!DNL Analytics] Erweiterung](https://aep-sdks.gitbook.io/docs/using-mobile-extensions/adobe-analytics#configure-analytics-extension-in-launch) konfiguriert und [Analytics zu Ihrer App](https://aep-sdks.gitbook.io/docs/using-mobile-extensions/adobe-analytics#add-analytics-to-your-app) hinzugefügt haben, sind diese Ereignisse in der [!UICONTROL In-App]-Konfiguration in ACS verfügbar.

## Zusätzliche Ressourcen

* [Lebenszyklusmetriken aktivieren (Dokumentation)](https://aep-sdks.gitbook.io/docs/getting-started/initialize-the-sdk#enable-lifecycle-metrics)
