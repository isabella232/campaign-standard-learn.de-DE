---
title: Ereignis konfigurieren
description: 'Wenn Sie eine In-App-Nachricht in Adobe Campaign Standard (ACS) konfigurieren, definieren Ereignis, welche vom Benutzer initiierte Aktion die Anzeige der Nachricht auslöst. '
feature: In-App
topics: Mobile
kt: 2548
doc-type: feature video
activity: use
team: TM
translation-type: tm+mt
source-git-commit: 82fb2d39dc61a55c0aa20ca1fa215f35a7dd9088
workflow-type: tm+mt
source-wordcount: '262'
ht-degree: 4%

---


# Konfigurieren von [!UICONTROL Ereignissen] {#configuring-events}

Beim Konfigurieren einer [!UICONTROL In-App] -Nachricht müssen Sie definieren, welche vom Benutzer initiierte Aktion die Anzeige der Nachricht auslöst. Diese Aktionen werden als [!UICONTROL Ereignisse]bezeichnet. Drei Kategorien [!UICONTROL Ereignis] stehen zur Verfügung: [!UICONTROL Mobile Application-Ereignis], [!UICONTROL Life Cycle-Ereignis]und [!UICONTROL Analytics-Ereignis].

## [!UICONTROL Mobile-App-Ereignisse] {#mobile-application-events}

[!UICONTROL Ereignis] für Mobilanwendungen sind [!UICONTROL benutzerdefinierte Ereignis] , die in Ihrer Mobilanwendung implementiert sind.

Beispiele:

* Ein Kunde hat einen Artikel angezeigt
* Ein Kunde fügt einen Artikel zum Warenkorb hinzu
* Stehen gelassener Warenkorb
* Ein Kunde hat etwas gekauft

Sie müssen diese [!UICONTROL Ereignis] in Adobe Campaign konfigurieren. Im folgenden Video wird beschrieben, wie Sie dies tun.

>[!VIDEO](https://video.tv.adobe.com/v/26245?quality=12)

## [!UICONTROL Lebenszyklus-Ereignisse]  {#life-cycle-events}

[!UICONTROL LebenszyklusEreignis] sind vordefinierte [!UICONTROL Ereignis]. Die folgenden [!UICONTROL Ereignisse] stehen zur Verfügung:

* [!UICONTROL gestartet]
* [!UICONTROL aktualisiert]
* [!UICONTROL abgestürzt]

Ein Beispielanwendungsfall könnte eine Meldung sein, die nach einer Aktualisierung neue Funktionen einführt, oder eine Ereignis-Promotion.

>[!NOTE]
>
>Das [!UICONTROL Lebenszyklusmodul] muss in der mobilen Anwendung konfiguriert werden. Weitere Informationen zum Hinzufügen des Lebenszyklus [zu Ihrer App finden Sie hier](https://aep-sdks.gitbook.io/docs/using-mobile-extensions/mobile-core/lifecycle)

## [!UICONTROL Analytics-Ereignisse] {#analytics-events}

Die folgenden drei Kategorien werden je nach Instrumentierung der mobilen App unterstützt:

* Adobe Analytics
* [!UICONTROL Kontextdaten]
* [!UICONTROL Status der Ansicht]

>[!NOTE]
>
>[!UICONTROL Für Analytics-Ereignis] ist eine Adobe Analytics-Lizenz erforderlich. Sobald Sie die [[!DNL Analytics] Erweiterung konfiguriert](https://aep-sdks.gitbook.io/docs/using-mobile-extensions/adobe-analytics#configure-analytics-extension-in-launch) haben und [Analytics zu Ihrer App](https://aep-sdks.gitbook.io/docs/using-mobile-extensions/adobe-analytics#add-analytics-to-your-app)hinzugefügt haben, sind diese Ereignis in der [!UICONTROL In-App] -Konfiguration in ACS verfügbar.

## Zusätzliche Ressourcen

* [Lebenszyklusmetriken aktivieren (Dokumentation)](https://aep-sdks.gitbook.io/docs/getting-started/initialize-the-sdk#enable-lifecycle-metrics)
