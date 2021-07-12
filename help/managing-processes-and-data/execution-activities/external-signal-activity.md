---
title: Aktivität "Externes Signal"- Aufruf eines Workflows mit Parametern
description: Erfahren Sie, wie Sie einen Workflow von einem anderen starten, um komplexere Journey zu unterstützen und gleichzeitig in der Lage sind, Probleme besser zu überwachen und besser auf sie zu reagieren.
feature: Ausführungsaktivität
kt: 2750
thumbnail: 27249
doc-type: feature video
activity: use
team: TM
exl-id: d3996185-681c-4906-85f0-0543ab767519
role: User, Developer
level: Experienced
source-git-commit: 2be2719ddd84490b796d9abc6300376fa896ff0c
workflow-type: tm+mt
source-wordcount: '315'
ht-degree: 18%

---

# [!UICONTROL Aktivität &quot;Externes Signal&quot;-  ]Aufruf eines Workflows mit Parametern

Die [!UICONTROL Aktivität &quot;Externes Signal&quot;] wird verwendet, um verschiedene Prozesse zu organisieren und zu orchestrieren, die zum gleichen Kunden-Journey gehören, und diese in verschiedenen Workflows zu verwalten. So kann ein Workflow durch einen anderen aktiviert werden, wodurch komplexere Customer Journeys möglich werden. Dies wiederum erlaubt eine bessere Überwachung der Prozesse und eine raschere Reaktion im Fall von Problemen.

In ACS 19.2 kann die Aktivität [!UICONTROL Externes Signal] nicht nur einen Workflow aufrufen, sondern auch Parameter an den Workflow übergeben (Zielgruppenname, zu importierender Dateiname, Teil des Nachrichteninhalts usw.) zum Workflow von einem anderen Workflow oder einem REST-API-Aufruf aus, um ihn in Ihre externen Systeme zu integrieren.

Dies umfasst auch eine neue Aktivität **Test** , in der Sie Tests für diese Funktion durchführen können.

Im folgenden Video werden die Konfigurationsschritte erläutert, die für Folgendes erforderlich sind:

1. **Erhalten Sie externe** Parameter von einem externen System wie z. B. einem Content Management System (CRM):

   * Parameter in der Aktivität &quot;Externes Signal&quot; deklarieren
   * Konfigurieren Sie den API-Aufruf, um die Parameter zu definieren und den Workflow &quot;Aktivität &quot;Externes Signal&quot;Trigger. Weitere Informationen zum Konfigurieren eines API-Aufrufs finden Sie unter [Auslösen einer Signalaktivität](https://docs.campaign.adobe.com/doc/standard/en/api/ACS_API.html#triggering-a-signal-activity).

1. **Anpassen eines Workflows mit externen Parametern**  (Ereignisvariablen):

   Nachdem der Workflow ausgelöst wurde, werden die Parameter in die Ereignisvariablen des Workflows aufgenommen und können im Workflow verwendet werden. Die [Dokumentation](https://helpx.adobe.com/campaign/standard/automating/using/calling-a-workflow-with-external-parameters.html) enthält alle Aktivitäten, die mit Ereignisvariablen angepasst werden können:

   * Konfigurieren der Testaktivität (neu in Version 19.2)
   * Konfigurieren der Aktivität Audience lesen und E-Mail-Versand

1. **Konfigurieren einer Ende-** Aktivität zum Aufrufen eines Workflows mit externen Parametern

>[!VIDEO](https://video.tv.adobe.com/v/27249/?quality=12)

## Zusätzliche Ressourcen

* [Externes Signal (Dokumentation)](https://experienceleague.adobe.com/docs/campaign-standard/using/managing-processes-and-data/calling-workflow-external-parameters/calling-a-workflow-with-external-parameters.html)
