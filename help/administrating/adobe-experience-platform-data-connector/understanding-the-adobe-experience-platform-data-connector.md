---
title: Grundlegendes zum Adobe Experience Platform Data Connector
description: Adobe Experience Platform Data Connector hilft Bestandskunden, ihre Daten in Adobe Experience Platform verfügbar zu machen, indem XTK-Daten (in Campaign erfasste Daten) den XDM-Daten (Experience-Datenmodell) in Adobe Experience Platform zugeordnet werden.
feature: People Core Service-Integration
kt: 2826
thumbnail: 27304.jpg
doc-type: feature video
activity: understand
team: TM
exl-id: 686961f9-5374-4cc6-8b36-7ee0584ea720
source-git-commit: 2ba22e7e7d193278fd06cb4b2dc80f650f754ec8
workflow-type: tm+mt
source-wordcount: '310'
ht-degree: 16%

---

# Grundlegendes zu Adobe Experience Platform [!UICONTROL Data Connector]

>[!NOTE]
>
>Diese Funktion befindet sich in der Beta-Phase und unterliegt häufigen Aktualisierungen und Änderungen ohne Vorankündigung.
>
>Wenden Sie sich an den [!UICONTROL Adobe-Support], wenn Sie diese Funktion implementieren möchten.

## Übersicht

Adobe Experience Platform [!UICONTROL Data Connector] unterstützt Bestandskunden dabei, ihre Daten in Adobe Experience Platform verfügbar zu machen, indem XTK-Daten (in Adobe Campaign erfasste Daten) [!DNL Experience Data Model] (XDM)-Daten in Adobe Experience Platform zugeordnet werden.

Der Connector ist unidirektional und sendet die Daten von Adobe Campaign Standard an Adobe Experience Platform. Die Daten werden nie von der Adobe Experience Platform an Adobe Campaign Standard gesendet.

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
5. [Überprüfen des Status eines Datenerfassungsauftrags](/help/administrating/adobe-experience-platform-data-connector/checking-status-of-data-ingestion-jobs.md)

## Zusätzliche Ressourcen

* [Über Adobe Experience Platform Data Connector](https://experienceleague.adobe.com/docs/campaign-standard/using/integrating-with-adobe-cloud/adobe-experience-platform/data-connector/aep-about-data-connector.html)

