---
title: Aktivität externer Signale - Aufruf eines Workflows mit Parametern
description: Mit der Aktivität "Externes Signal"können verschiedene Prozesse organisiert und koordiniert werden, die zum gleichen Kundenverlauf in verschiedene Workflows gehören. So kann ein Workflow durch einen anderen aktiviert werden, wodurch komplexere Customer Journeys möglich werden. Dies wiederum erlaubt eine bessere Überwachung der Prozesse und eine raschere Reaktion im Fall von Problemen.
feature: External Signal Activity
topics: Workflows
kt: 2750
doc-type: feature video
activity: use
team: TM
translation-type: tm+mt
source-git-commit: 9b1d8c5fb895d84da14a0402ec1f130b90a991b0
workflow-type: tm+mt
source-wordcount: '341'
ht-degree: 24%

---


# [!UICONTROL Aktivität für externe Signale ]- Aufruf eines Workflows mit Parametern

The [!UICONTROL External Signal activity] is used to organize and orchestrate different processes that are part of the same customer journey into different workflows. So kann ein Workflow durch einen anderen aktiviert werden, wodurch komplexere Customer Journeys möglich werden. Dies wiederum erlaubt eine bessere Überwachung der Prozesse und eine raschere Reaktion im Fall von Problemen.

In ACS 19.2 kann die [!UICONTROL externe Signal-Aktivität] nicht nur einen Workflow aufrufen, sondern auch Parameter an den Workflow übergeben (Name der Audience an Zielgruppe, zu importierender Dateiname, Teil des Nachrichteninhalts usw.) in den Workflow von einem anderen Workflow oder einem REST API-Aufruf zur Integration in Ihre externen Systeme.

This also includes a new **Test** Activity where you can run tests on this functionality.

Im folgenden Video werden die Konfigurationsschritte erläutert, die erforderlich sind, um

1. **Erhalten Sie externe Parameter** von einem externen System, z. B. einem Content-Management-System (CRM):

   * Deklarieren der Parameter in der Aktivität &quot;Externes Signal&quot;
   * Konfigurieren Sie den API-Aufruf, um die Parameter zu definieren und die Workflow-Aktivität &quot;Externes Signal&quot;auszulösen. Weitere Informationen zum Konfigurieren eines API-Aufrufs finden Sie unter [Auslösen einer Signal-Aktivität](https://docs.campaign.adobe.com/doc/standard/en/api/ACS_API.html#triggering-a-signal-activity).

1. **Anpassen eines Workflows mit externen Parametern** (Ereignis-Variablen):

   Nachdem der Workflow ausgelöst wurde, werden die Parameter in die Ereignisvariablen des Workflows aufgenommen und können im Workflow verwendet werden. Informationen zu allen Aktivitäten, die mit Ereignis-Variablen angepasst werden können, finden Sie in der [Dokumentation](https://helpx.adobe.com/campaign/standard/automating/using/calling-a-workflow-with-external-parameters.html) :

   * Konfigurieren der Test-Aktivität (neu in 19.2)
   * Audience und Aktivität von E-Mail-Versänden konfigurieren

1. **Eine End-Aktivität** zum Aufrufen eines Workflows mit externen Parametern konfigurieren

>[!VIDEO](https://video.tv.adobe.com/v/27249/?quality=12)

## Zusätzliche Ressourcen

* [Externes Signal (Dokumentation)](https://docs.adobe.com/content/help/en/campaign-standard/using/managing-processes-and-data/data-management-activities/external-api.html)
