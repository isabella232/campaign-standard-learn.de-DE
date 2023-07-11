---
title: Grundlegendes zum Adobe Experience Platform Data Connector
description: Adobe Experience Platform Data Connector hilft Bestandskunden, ihre Daten in Adobe Experience Platform verfügbar zu machen, indem XTK-Daten (in Campaign aufgenommene Daten) den XDM-Daten (Experience-Datenmodell) in Adobe Experience Platform zugeordnet werden.
feature: People Core Service Integration
jira: KT-2826
thumbnail: 27304.jpg
role: User
level: Advanced
doc-type: feature video
activity: understand
team: TM
exl-id: 686961f9-5374-4cc6-8b36-7ee0584ea720
source-git-commit: 89f520da0455da693b27c397f95cdabab4552770
workflow-type: tm+mt
source-wordcount: '289'
ht-degree: 16%

---

# Grundlegendes zur Adobe Experience Platform [!UICONTROL Data Connector]

>[!NOTE]
>
>Diese Funktion befindet sich in der Beta-Phase und unterliegt häufigen Aktualisierungen und Änderungen ohne Vorankündigung.
>
>Bitte wenden Sie sich an [!UICONTROL Adobe-Kundensupport] , wenn Sie diese Funktion implementieren möchten.

## Übersicht

Adobe Experience Platform [!UICONTROL Data Connector] hilft Bestandskunden, ihre Daten in Adobe Experience Platform verfügbar zu machen, indem XTK-Daten (in Adobe Campaign erfasste Daten) zugeordnet werden zu [!DNL Experience Data Model] (XDM)-Daten in Adobe Experience Platform.

Der Connector ist unidirektional und sendet die Daten von Adobe Campaign Standard an Adobe Experience Platform. Die Daten werden nie von der Adobe Experience Platform an Adobe Campaign Standard gesendet.

Adobe Experience Platform [!UICONTROL Data Connector] ist für Dateningenieure gedacht, die Adobe Campaign Standard verstehen [!UICONTROL benutzerdefinierte Ressourcen] und verstehen, wie das gesamte Datenschema des Kunden in Adobe Experience Platform aussehen sollte.

>[!VIDEO](https://video.tv.adobe.com/v/27304?quality=12&learn=on)

*In diesem Video erhalten Sie einen Überblick über die Adobe Experience Platform [!UICONTROL Data Connector] (09:35 Min.)*

>[!NOTE]
>
>Die vordefinierte Übertragung von [!UICONTROL Abonnement-Ereignisse] wird nicht unterstützt. Zu transferieren [!UICONTROL Abonnement-Ereignisse], können Sie entsprechende XDM- und Datensätze in Adobe Experience Platform erstellen und dann ein benutzerdefiniertes Daten-Mapping für diese Daten konfigurieren.
>
>Bestehend [!UICONTROL Erlebnisereignisse] kann nicht in Adobe Experience Platform aufgenommen werden, aber fortlaufend generiert werden [!UICONTROL Erlebnisereignisse] werden an Adobe Experience Platform gestreamt.

## Wichtige Schritte zum Durchführen eines Daten-Mappings

In den folgenden Tutorials werden die wichtigsten Schritte zum Durchführen einer Datenzuordnung zwischen Campaign Standard und Adobe Experience Platform beschrieben:

1. [Zuordnen benutzerdefinierter Ressourcen](/help/administrating/adobe-experience-platform-data-connector/mapping-custom-resources.md)
2. [Zuordnen von Erlebnisereignissen](/help/administrating/adobe-experience-platform-data-connector/mapping-experience-events.md)
3. [Zuordnen von Seed-Tabellendaten](/help/administrating/adobe-experience-platform-data-connector/mapping-seed-table-data.md)
4. [Ändern der Datenzuordnung](/help/administrating/adobe-experience-platform-data-connector/modifying-data-mapping.md)
5. [Überprüfen des Status von Datenaufnahmevorgängen](/help/administrating/adobe-experience-platform-data-connector/checking-status-of-data-ingestion-jobs.md)

