---
title: Konfigurieren von Ereignissen
description: '"Erfahren Sie, wie Ereignisse definieren, welche vom Benutzer initiierte Aktion eine In-App-Nachricht Trigger, die angezeigt werden soll. "'
feature: In App
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
source-wordcount: '255'
ht-degree: 7%

---

# Konfigurieren [!UICONTROL Veranstaltungen] {#configuring-events}

Beim Konfigurieren von [!UICONTROL In-App] -Meldung eingeben, müssen Sie definieren, welche vom Benutzer initiierte Aktion die Nachricht Trigger, die angezeigt werden soll. Diese Aktionen werden [!UICONTROL events]. Drei Kategorien von [!UICONTROL events] sind verfügbar: [!UICONTROL Mobile-App-Ereignisse], [!UICONTROL Lebenszyklusereignisse]und [!UICONTROL Analytics-Ereignisse].

## [!UICONTROL Mobile-App-Ereignisse] {#mobile-application-events}

[!UICONTROL Mobile-App-Ereignisse] are [!UICONTROL benutzerspezifische Ereignisse] die in Ihrer Mobile App implementiert sind.

Beispiele:

* Ein Kunde hat einen Artikel angesehen
* Ein Kunde fügt einen Artikel zum Warenkorb hinzu
* Stehen gelassener Warenkorb
* Ein Kunde hat etwas gekauft

Sie müssen diese [!UICONTROL events] in Adobe Campaign. Im folgenden Video wird beschrieben, wie Sie dies durchführen.

>[!VIDEO](https://video.tv.adobe.com/v/26245?quality=12)

## [!UICONTROL Lebenszyklusereignisse] {#life-cycle-events}

[!UICONTROL Lebenszyklusereignisse] sind vorkonfiguriert [!UICONTROL events]. Folgendes [!UICONTROL events] sind verfügbar:

* [!UICONTROL gestartet]
* [!UICONTROL aktualisiert]
* [!UICONTROL abgestürzt]

Ein Anwendungsbeispiel könnte eine Nachricht sein, die nach einem Upgrade neue Funktionen einführt, oder eine Ereignispromotion.

>[!NOTE]
>
>Die [!UICONTROL Lebenszyklusmodul] in der Mobile App konfiguriert werden. Weitere Informationen finden Sie hier . [Hinzufügen des Lebenszyklus zu Ihrer App](https://aep-sdks.gitbook.io/docs/using-mobile-extensions/mobile-core/lifecycle)

## [!UICONTROL Analytics-Ereignisse] {#analytics-events}

Je nach der Konfiguration Ihrer App werden die folgenden drei Kategorien unterstützt:

* Adobe Analytics
* [!UICONTROL Kontextdaten]
* [!UICONTROL Ansichtsstatus]

>[!NOTE]
>
>[!UICONTROL Analytics-Ereignisse] eine Adobe Analytics-Lizenz benötigen. Sobald Sie [[!DNL Analytics] Erweiterung konfiguriert](https://aep-sdks.gitbook.io/docs/using-mobile-extensions/adobe-analytics#configure-analytics-extension-in-launch) und [Analytics für Ihre App](https://aep-sdks.gitbook.io/docs/using-mobile-extensions/adobe-analytics#add-analytics-to-your-app), werden diese Ereignisse in der Variablen [!UICONTROL In-App] Konfiguration in ACS.

## Zusätzliche Ressourcen

* [Lebenszyklusmetriken aktivieren (Dokumentation)](https://aep-sdks.gitbook.io/docs/getting-started/initialize-the-sdk#enable-lifecycle-metrics)
