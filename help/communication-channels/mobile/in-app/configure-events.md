---
title: Konfigurieren von Ereignissen
description: 'Beim Konfigurieren einer In-App-Nachricht in Adobe Campaign Standard (ACS) definieren Ereignis, welche vom Benutzer initiierte Aktion die Anzeige der Nachricht Trigger. '
feature: In-App
topics: Mobile
kt: 2548
thumbnail: 26245.jpg
doc-type: feature video
activity: use
team: TM
translation-type: tm+mt
source-git-commit: 11263e247184ddc6a8e3df6a8ed0899907fbb366
workflow-type: tm+mt
source-wordcount: '262'
ht-degree: 7%

---


# [!UICONTROL Ereignis] {#configuring-events} konfigurieren

Beim Konfigurieren einer [!UICONTROL In-App]-Meldung müssen Sie definieren, welche vom Benutzer ausgelöste Aktion die anzuzeigende Meldung Trigger. Diese Aktionen werden als [!UICONTROL Ereignis] bezeichnet. Es stehen drei Kategorien von [!UICONTROL Ereignissen] zur Verfügung: [!UICONTROL Ereignis für Mobilanwendungen], [!UICONTROL Ereignis für Lebenszykluszyklen] und [!UICONTROL Analytics-Ereignis].

## [!UICONTROL Mobile-App-Ereignisse] {#mobile-application-events}

[!UICONTROL Mobilanwendungs-] Ereignisse sind  [!UICONTROL benutzerdefinierte ] Ereignisse, die in Ihrer Mobilanwendung implementiert sind.

Beispiele:

* Ein Kunde hat einen Artikel angezeigt
* Ein Kunde fügt einen Artikel zum Warenkorb hinzu
* Stehen gelassener Warenkorb
* Ein Kunde hat etwas gekauft

Sie müssen diese [!UICONTROL Ereignis] in Adobe Campaign konfigurieren. Im folgenden Video wird beschrieben, wie Sie dies tun.

>[!VIDEO](https://video.tv.adobe.com/v/26245?quality=12)

## [!UICONTROL Lebenszyklus-Ereignisse]  {#life-cycle-events}

[!UICONTROL Lebenszyklusereignisse ] sind vordefinierte  [!UICONTROL Ereignis]. Die folgenden [!UICONTROL Ereignis] stehen zur Verfügung:

* [!UICONTROL gestartet]
* [!UICONTROL aktualisiert]
* [!UICONTROL abgestürzt]

Ein Beispielanwendungsfall könnte eine Meldung sein, die nach einer Aktualisierung neue Funktionen einführt, oder eine Ereignis-Promotion.

>[!NOTE]
>
>Das [!UICONTROL Lebenszyklusmodul] muss in der Mobilanwendung konfiguriert werden. Weitere Informationen zum Hinzufügen des Lebenszyklus zu Ihrer App finden Sie hier[](https://aep-sdks.gitbook.io/docs/using-mobile-extensions/mobile-core/lifecycle)

## [!UICONTROL Analytics-Ereignisse] {#analytics-events}

Die folgenden drei Kategorien werden je nach Instrumentierung der mobilen App unterstützt:

* Adobe Analytics
* [!UICONTROL Kontextdaten]
* [!UICONTROL Status der Ansicht]

>[!NOTE]
>
>[!UICONTROL Für Analytics-] Ereignisse ist eine Adobe Analytics-Lizenz erforderlich. Sobald Sie die Erweiterung [[!DNL Analytics] konfiguriert haben und ](https://aep-sdks.gitbook.io/docs/using-mobile-extensions/adobe-analytics#configure-analytics-extension-in-launch) [Analytics zu Ihrer App](https://aep-sdks.gitbook.io/docs/using-mobile-extensions/adobe-analytics#add-analytics-to-your-app) hinzugefügt haben, sind diese Ereignis in der ACS-Konfiguration [!UICONTROL In-App] verfügbar.

## Zusätzliche Ressourcen

* [Lebenszyklusmetriken aktivieren (Dokumentation)](https://aep-sdks.gitbook.io/docs/getting-started/initialize-the-sdk#enable-lifecycle-metrics)
