---
title: Datenschutzanforderungen mit dem Adobe Campaign Standard (ACS) - Übersicht
description: Das Lernprogramm erläutert, wie Pprivacy-Anforderungen über die ACS-Schnittstelle (Adobe Campaign Standard) erstellt werden.
feature: GDPR, CCAP
topic: Privacy
kt: 1480
doc-type: feature video
activity: use
team: TM
translation-type: tm+mt
source-git-commit: 556bff4c94e16d3a94561dee1ccb311bc003b631
workflow-type: tm+mt
source-wordcount: '370'
ht-degree: 18%

---


# Datenschutzanforderungen mit der Benutzeroberfläche des Adobe Campaign Standards

Adobe Campaign Angebots Data Controllers drei Methoden zum Ausführen von Datenschutzaufrufen und Löschen von Anfragen von PII-Daten unter Einhaltung von Datenschutzvorschriften wie GDPR (Allgemeine Datenschutzverordnung) und CCPA (California Consumer Privacy Act):

* **Über die Integration des Datenschutz-Core-Service:** Datenschutzanforderungen, die von [!UICONTROL Privacy Service] an alle Experience Cloud-Lösungen gesendet werden, werden automatisch von der Kampagne über einen dedizierten Arbeitsablauf verarbeitet. Refer to the [Adobe Experience Platform Privacy Service](https://adobe.io/apis/cloudplatform/gdpr.html) to learn how to create privacy requests from the Privacy Core Service

* **Über die API:** Adobe Campaign stellt eine API bereit, die den automatischen Prozess von Datenschutzanfragen mithilfe von REST ermöglicht

* **Über die Adobe Campaign-Oberfläche:** für jede Datenschutzanforderung erstellt der Datencontroller eine neue Datenschutzanforderung in Adobe Campaign

>[!NOTE]
>
> **ÄNDERUNGEN AN ACS 19.4:**
> 
> The [Privacy Service integration](https://adobe.io/apis/cloudplatform/gdpr.html) is the method you should use for all access and delete requests. Mit Version 19.4. wurde die Campaign-API und -Schnittstelle für Zugriffs- und Löschanfragen eingestellt. Weiterführende Informationen zu veralteten und entfernten Funktionen von Campaign Standard finden Sie auf [dieser Seite](https://helpx.adobe.com/de/campaign/kb/acs-deprecated-and-removed-features.html).
>
>**Ausschluss vom Verkauf personenbezogener Daten (CCPA)**
>
>Ab Version 19.4 wird ein CCPA-Ausschluss-Feld in der Benutzeroberfläche und in der API sofort bereitgestellt. Damit 19.3 diese Informationen nutzen kann, müssen Sie dieses Feld in Adobe Campaign Standard erstellen. Weitere Informationen finden Sie in der [ausführlichen Dokumentation](https://helpx.adobe.com/de/campaign/kb/acs-privacy.html#ccpa) .
>
> Sie können Ihre Version überprüfen, indem Sie auf das ? oben rechts auf der Benutzeroberfläche und wählen Sie Info.

## Video-Tutorials

### Voraussetzungen für Datenschutzanforderungen

1. [Erstellen eines Namensraums](/help/privacy/namespaces-for-privacy-requests.md)
1. [Benutzerdefinierte Ressourcen ändern](/help/privacy/custom-resources-for-privacy-requests.md)

### Erstellen, verfolgen und ausführen von Datenschutzanforderungen über die Adobe Campaign-Benutzeroberfläche

* [Erstellen und verfolgen Sie Datenschutzanforderungen über die Benutzeroberfläche von Adobe Campaign](/help/privacy/create-and-track-privacy-requests.md)
* [Datenschutzanforderungen ausführen](/help/privacy/execute-privacy-requests.md)

## Zusätzliche Ressourcen

* [Allgemeine Datenschutzrichtlinien für die Kampagne](https://helpx.adobe.com/de/campaign/kb/campaign-privacy-overview.html)
* [CCPA für ACS](https://helpx.adobe.com/de/campaign/kb/acs-privacy.html#ccpa)
* [Adobe Experience Platform Privacy Service](https://adobe.io/apis/cloudplatform/gdpr.html)
* [Dokumentation zur Adobe Campaign Standard-REST-API](https://final-docs.campaign.adobe.com/doc/standard/en/api/ACS_API.html#privacy-management)
