---
title: Informationen zum Adobe Experience Platform Data Connector
description: Adobe Experience Platform Data Connector hilft Bestandskunden, ihre Daten in Adobe Experience Platform verfügbar zu machen, indem XTK-Daten (in Campaign erfasste Daten) den XDM-Daten (Experience-Datenmodell) in Adobe Experience Platform zugeordnet werden.
kt: 2826
thumbnail: 27304.jpg
doc-type: feature video
activity: understand
team: TM
exl-id: 686961f9-5374-4cc6-8b36-7ee0584ea720
source-git-commit: 5a2f8c9a78bf5100b272f9b4461131545b3aeb8b
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Grundlagen zum Adobe Experience Platform [!UICONTROL Data Connector]

>[!NOTE]
>
>Diese Funktion befindet sich derzeit in der Beta-Phase und unterliegt häufigen Aktualisierungen und Änderungen ohne Vorankündigung.
>
>Wenden Sie sich an den [!UICONTROL Adobe-Support], wenn Sie diese Funktion implementieren möchten.

## Übersicht

Adobe Experience Platform [!UICONTROL Data Connector] unterstützt Bestandskunden dabei, ihre Daten in Adobe Experience Platform verfügbar zu machen, indem XTK-Daten (in Adobe Campaign erfasste Daten) [!DNL Experience Data Model] (XDM)-Daten in Adobe Experience Platform zugeordnet werden.

Beachten Sie, dass der Connector unidirektional ist und die Daten von Adobe Campaign Standard an Adobe Experience Platform sendet. Die Daten werden nie von der Adobe Experience Platform an Adobe Campaign Standard gesendet.

Adobe Experience Platform [!UICONTROL Data Connector] ist für Dateningenieure gedacht, die mit Adobe Campaign Standard [!UICONTROL benutzerdefinierten Ressourcen] vertraut sind und verstehen, wie das gesamte Datenschema des Kunden in Adobe Experience Platform aussehen sollte.

>[!VIDEO](https://video.tv.adobe.com/v/27304?quality=12)

*In diesem Video erhalten Sie einen Überblick über den Adobe Experience Platform  [!UICONTROL Data Connector]  (09:35 Min.)*

>[!NOTE]
>
>Die vordefinierte Übertragung von [!UICONTROL Abonnementereignissen] wird nicht unterstützt. Um [!UICONTROL Abonnementereignisse] zu übertragen, können Sie entsprechende XDM- und Datensätze in Adobe Experience Platform erstellen und dann ein benutzerdefiniertes Daten-Mapping für diese Daten konfigurieren.
>
>Vorhandene [!UICONTROL Erlebnisereignisse] können nicht in Adobe Experience Platform aufgenommen werden, aber fortlaufend generierte [!UICONTROL Erlebnisereignisse] werden an Adobe Experience Platform gestreamt.

## Wichtige Schritte zum Durchführen eines Daten-Mappings

In den folgenden Tutorials werden die wichtigsten Schritte zum Durchführen einer Datenzuordnung zwischen Campaign Standard und Adobe Experience Platform beschrieben:

1. [Zuordnen benutzerdefinierter Ressourcen](/help/administrating/adobe-experience-platform-data-connector/mapping-custom-resources.md)
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
