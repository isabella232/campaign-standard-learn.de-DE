---
title: Informationen zum Adobe Experience Platform Data Connector
description: Adobe Experience Platform Data Connector hilft Bestandskunden, ihre Daten in Adobe Experience Platform verfügbar zu machen, indem XTK-Daten (in Campaign erfasste Daten) den XDM-Daten (Experience-Datenmodell) in Adobe Experience Platform zugeordnet werden.
feature: Adobe Experience Platform Data Connector
topics: ACoP
kt: 2826
doc-type: feature video
activity: understand
team: TM
translation-type: tm+mt
source-git-commit: d87971b70bde8de1822f18cbafd8e2d7b4808edc
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---


# Understanding the Adobe Experience Platform [!UICONTROL Data Connector]

>[!NOTE]
>
>Diese Funktion befindet sich derzeit in der Beta-Phase und wird häufig aktualisiert und ohne Vorankündigung geändert.
>
>Wenden Sie sich an den [!UICONTROL Kundendienst] , wenn Sie diese Funktion implementieren möchten.

## Übersicht

Adobe Experience Platform [!UICONTROL Data Connector] helps existing customers to make their data available on Adobe Experience Platform by mapping XTK data (data ingested in Adobe Campaign) to [!DNL Experience Data Model] (XDM) data on Adobe Experience Platform.

Beachten Sie, dass der Connector unidirektional ist und die Daten von Adobe Campaign Standard an Adobe Experience Platform sendet. Die Daten werden nie von der Adobe Experience Platform nach Adobe Campaign Standard gesendet.

Adobe Experience Platform [!UICONTROL Data Connector] is intended for data engineers who understand Adobe Campaign Standard [!UICONTROL custom resources] and have an understanding of how customer&#39;s overall data schema should be inside Adobe Experience Platform.

>[!VIDEO](https://video.tv.adobe.com/v/27304?quality=12)

*Dieses Video gibt einen Überblick über den Adobe Experience Platform[!UICONTROL Data Connector](09:35 Min.)*

>[!NOTE]
>
>The out-of-the-box transfer of [!UICONTROL subscription events] is not supported. To transfer [!UICONTROL subscription events], you can create corresponding XDM and dataset on Adobe Experience Platform, then configure a custom data mapping for these data.
>
>Vorhandene [!UICONTROL Erlebnis-Ereignis] können nicht in Adobe Experience Platform integriert werden, aber fortlaufend generierte [!UICONTROL Erlebnis-Ereignis] werden in Adobe Experience Platform gestreamt.

## Wichtige Schritte zum Durchführen einer Datenzuordnung

Die folgenden Lernprogramme beschreiben die wichtigsten Schritte zum Durchführen einer Datenzuordnung zwischen Campaign Standard und Adobe Experience Platform:

1. [Benutzerdefinierte Ressourcen zuordnen](/help/administrating/adobe-experience-platform-data-connector/mapping-custom-resources.md)
2. [Zuordnen von Erlebnisereignissen](/help/administrating/adobe-experience-platform-data-connector/mapping-experience-events.md)
3. [Zuordnen von Seed-Tabellendaten](/help/administrating/adobe-experience-platform-data-connector/mapping-seed-table-data.md)
4. [Ändern der Datenzuordnung](/help/administrating/adobe-experience-platform-data-connector/modifying-data-mapping.md)
5. [Überprüfen des Status von Datenerfassungsvorgängen](/help/administrating/adobe-experience-platform-data-connector/checking-status-of-data-ingestion-jobs.md)

## Zusätzliche Ressourcen

* [Über Adobe Experience Platform Data Connector](https://docs.adobe.com/content/help/en/campaign-standard/using/administrating/mapping-campaign-and-aep-data/aep-about-data-connector.html)
* [Übersicht über das Experience-Datenmodell](https://docs.adobe.com/content/help/en/campaign-standard/using/administrating/mapping-campaign-and-aep-data/aep-data-model-overview.html)
* [Mapping-Definition](https://docs.adobe.com/content/help/en/campaign-standard/using/administrating/mapping-campaign-and-aep-data/aep-mapping-definition.html)
* [Mapping-Aktivierung](https://docs.adobe.com/content/help/en/campaign-standard/using/administrating/mapping-campaign-and-aep-data/aep-mapping-activation.html)
* [Datenerfassung über APIs aktivieren](https://docs.adobe.com/content/help/en/campaign-standard/using/administrating/mapping-campaign-and-aep-data/aep-triggering-data-ingestion.html)
