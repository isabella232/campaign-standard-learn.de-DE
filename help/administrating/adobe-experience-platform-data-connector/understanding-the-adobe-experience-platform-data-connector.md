---
title: Informationen zum Adobe Experience Platform Data Connector
description: Adobe Experience Platform Data Connector hilft Bestandskunden, ihre Daten in Adobe Experience Platform verfügbar zu machen, indem XTK-Daten (in Campaign erfasste Daten) den XDM-Daten (Experience-Datenmodell) in Adobe Experience Platform zugeordnet werden.
feature: Adobe Experience Platform Data Connector
topics: ACoP
kt: 2826
thumbnail: 27304.jpg
doc-type: feature video
activity: understand
team: TM
translation-type: tm+mt
source-git-commit: 11263e247184ddc6a8e3df6a8ed0899907fbb366
workflow-type: tm+mt
source-wordcount: '364'
ht-degree: 25%

---


# Erläuterungen zum Adobe Experience Platform [!UICONTROL Data Connector]

>[!NOTE]
>
>Diese Funktion befindet sich derzeit in der Beta-Phase und wird häufig aktualisiert und ohne Vorankündigung geändert.
>
>Wenden Sie sich an den [!UICONTROL Adobe Kundensupport], wenn Sie diese Funktion implementieren möchten.

## Übersicht  

Adobe Experience Platform [!UICONTROL Data Connector] unterstützt Bestandskunden dabei, ihre Daten auf Adobe Experience Platform verfügbar zu machen, indem sie XTK-Daten (in Adobe Campaign erfasste Daten) zu [!DNL Experience Data Model] (XDM)-Daten auf Adobe Experience Platform zuordnen.

Beachten Sie, dass der Connector unidirektional ist und die Daten von Adobe Campaign Standard an Adobe Experience Platform sendet. Die Daten werden nie von der Adobe Experience Platform nach Adobe Campaign Standard gesendet.

Adobe Experience Platform [!UICONTROL Data Connector] ist für Dateningenieure gedacht, die mit Adobe Campaign Standard [!UICONTROL benutzerspezifischen Ressourcen] vertraut sind und verstehen, wie sich das Schema der Kundendaten insgesamt in Adobe Experience Platform befinden sollte.

>[!VIDEO](https://video.tv.adobe.com/v/27304?quality=12)

*Dieses Video gibt einen Überblick über den Adobe Experience Platform  [!UICONTROL Data Connector]  (09:35 Min.)*

>[!NOTE]
>
>Die vordefinierte Übertragung von [!UICONTROL Abonnement-Ereignissen] wird nicht unterstützt. Um [!UICONTROL Abonnement-Ereignis] zu übertragen, können Sie entsprechende XDM- und Datasets auf Adobe Experience Platform erstellen und dann eine benutzerdefinierte Datenzuordnung für diese Daten konfigurieren.
>
>Bestehende [!UICONTROL Erlebnis-Ereignis] können nicht in Adobe Experience Platform integriert werden, aber fortlaufend generierte [!UICONTROL Erlebnis-Ereignis] werden nach Adobe Experience Platform gestreamt.

## Wichtige Schritte zum Durchführen einer Datenzuordnung

Die folgenden Lernprogramme beschreiben die wichtigsten Schritte zum Durchführen einer Datenzuordnung zwischen Campaign Standard und Adobe Experience Platform:

1. [Benutzerdefinierte Ressourcen zuordnen](/help/administrating/adobe-experience-platform-data-connector/mapping-custom-resources.md)
2. [Zuordnen von Erlebnisereignissen](/help/administrating/adobe-experience-platform-data-connector/mapping-experience-events.md)
3. [Zuordnen von Seed-Tabellendaten](/help/administrating/adobe-experience-platform-data-connector/mapping-seed-table-data.md)
4. [Ändern der Datenzuordnung](/help/administrating/adobe-experience-platform-data-connector/modifying-data-mapping.md)
5. [Überprüfen des Status von Datenaufnahmevorgängen](/help/administrating/adobe-experience-platform-data-connector/checking-status-of-data-ingestion-jobs.md)

## Zusätzliche Ressourcen

* [Über Adobe Experience Platform Data Connector](https://docs.adobe.com/content/help/en/campaign-standard/using/administrating/mapping-campaign-and-aep-data/aep-about-data-connector.html)
* [Übersicht über das Experience-Datenmodell](https://docs.adobe.com/content/help/en/campaign-standard/using/administrating/mapping-campaign-and-aep-data/aep-data-model-overview.html)
* [Mapping-Definition](https://docs.adobe.com/content/help/en/campaign-standard/using/administrating/mapping-campaign-and-aep-data/aep-mapping-definition.html)
* [Mapping-Aktivierung](https://docs.adobe.com/content/help/en/campaign-standard/using/administrating/mapping-campaign-and-aep-data/aep-mapping-activation.html)
* [Datenaufnahme über APIs aktivieren](https://docs.adobe.com/content/help/en/campaign-standard/using/administrating/mapping-campaign-and-aep-data/aep-triggering-data-ingestion.html)
