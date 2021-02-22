---
title: Aktivität externer Signale - Aufruf eines Workflows mit Parametern
description: Die Aktivität "Externes Signal"dient zur Organisation und Orchestrierung verschiedener Prozesse, die zum gleichen Journey gehören, in verschiedene Workflows. So kann ein Workflow durch einen anderen aktiviert werden, wodurch komplexere Customer Journeys möglich werden. Dies wiederum erlaubt eine bessere Überwachung der Prozesse und eine raschere Reaktion im Fall von Problemen.
feature: Aktivität "Externes Signal"
topics: Workflows
kt: 2750
thumbnail: 27249
doc-type: feature video
activity: use
team: TM
translation-type: tm+mt
source-git-commit: 2237e6a7d6a8c202ea87aeeb4b1e6fa83e1c677c
workflow-type: tm+mt
source-wordcount: '342'
ht-degree: 25%

---


# [!UICONTROL Aktivität für externe Signale  ]- Aufruf eines Workflows mit Parametern

Die [!UICONTROL Externe Signal-Aktivität] wird verwendet, um verschiedene Prozesse zu organisieren und zu orchestrieren, die zum gleichen Journey gehören, und zwar in verschiedene Workflows. So kann ein Workflow durch einen anderen aktiviert werden, wodurch komplexere Customer Journeys möglich werden. Dies wiederum erlaubt eine bessere Überwachung der Prozesse und eine raschere Reaktion im Fall von Problemen.

In ACS 19.2 kann die [!UICONTROL Externe Signal-Aktivität] nicht nur einen Workflow aufrufen, sondern auch Parameter an den Workflow übergeben (Audience zu Zielgruppe, zu importierender Dateiname, Teil des Nachrichteninhalts usw.) in den Workflow von einem anderen Workflow oder einem REST API-Aufruf zur Integration in Ihre externen Systeme.

Dazu gehört auch eine neue **Test**-Aktivität, mit der Sie Tests zu dieser Funktion durchführen können.

Im folgenden Video werden die Konfigurationsschritte erläutert, die erforderlich sind, um

1. **Externe** Parameter von einem externen System wie z. B. einem Content-Management-System (CRM) empfangen:

   * Deklarieren der Parameter in der Aktivität &quot;Externes Signal&quot;
   * Konfigurieren Sie den API-Aufruf, um die Parameter zu definieren und die Workflow-Aktivität &quot;Externes Signal&quot;Trigger. Weitere Informationen zum Konfigurieren eines API-Aufrufs finden Sie unter [Auslösen einer Signal-Aktivität](https://docs.campaign.adobe.com/doc/standard/en/api/ACS_API.html#triggering-a-signal-activity).

1. **Anpassen eines Workflows mit externen Parametern**  (Ereignis-Variablen):

   Nachdem der Workflow ausgelöst wurde, werden die Parameter in die Ereignisvariablen des Workflows aufgenommen und können im Workflow verwendet werden. Informationen zu allen Aktivitäten, die mit Ereignis-Variablen angepasst werden können, finden Sie unter [documentation](https://helpx.adobe.com/campaign/standard/automating/using/calling-a-workflow-with-external-parameters.html):

   * Konfigurieren der Test-Aktivität (neu in 19.2)
   * Audience und Aktivität von E-Mail-Versänden konfigurieren

1. **Konfigurieren einer End-** Aktivität zum Aufrufen eines Workflows mit externen Parametern

>[!VIDEO](https://video.tv.adobe.com/v/27249/?quality=12)

## Zusätzliche Ressourcen

* [Externes Signal (Dokumentation)](https://experienceleague.adobe.com/docs/campaign-standard/using/managing-processes-and-data/calling-workflow-external-parameters/calling-a-workflow-with-external-parameters.html)
