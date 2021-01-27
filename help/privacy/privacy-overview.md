---
title: Datenschutzanfragen beim Adobe Campaign Standard (ACS) - Überblick
description: In dem Lernprogramm wird erläutert, wie Pprivacy-Anforderungen über die Oberfläche von Adobe Campaign Standard (ACS) erstellt werden.
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
ht-degree: 32%

---


# Datenschutzanforderungen mit der Adobe Campaign Standard-Benutzeroberfläche

Adobe Campaign Angebots Data Controllers drei Methoden zum Ausführen von Datenschutzaufrufen und Löschen von Anfragen von PII-Daten unter Einhaltung von Datenschutzvorschriften wie GDPR (Allgemeine Datenschutzverordnung) und CCPA (California Consumer Privacy Act):

* **Über die Integration des Datenschutz-Core-Service:** Datenschutzanforderungen, die vom  [!UICONTROL Datenschutzdienst an alle Experience Cloud-Lösungen gesendet ] werden, werden automatisch über einen dedizierten Arbeitsablauf von der Kampagne verarbeitet. Informationen zum Erstellen von Datenschutzanfragen vom Privacy Core Service finden Sie unter [Adobe Experience Platform Privacy Service](https://adobe.io/apis/cloudplatform/gdpr.html).

* **Über die API:** Adobe Campaign stellt eine API bereit, die den automatischen Prozess von Datenschutzanforderungen mithilfe von REST ermöglicht

* **Über die Adobe Campaign-Oberfläche:** Für jede Datenschutzanforderung erstellt der Datencontroller eine neue Datenschutzanforderung in Adobe Campaign

>[!NOTE]
>
> **ÄNDERUNGEN AN ACS 19.4:**
> 
> Die [Privacy Service-Integration](https://adobe.io/apis/cloudplatform/gdpr.html) ist die Methode, die Sie für alle Zugriffs- und Löschanforderungen verwenden sollten. Mit Version 19.4. wurde die Campaign-API und -Schnittstelle für Zugriffs- und Löschanfragen eingestellt. Weiterführende Informationen zu veralteten und entfernten Funktionen von Campaign Standard finden Sie auf [dieser Seite](https://helpx.adobe.com/de/campaign/kb/acs-deprecated-and-removed-features.html).
>
>**Opt-out aus dem Verkauf von personenbezogenen Daten (CCPA)**
>
>Ab Version 19.4. verfügen die Campaign-Oberfläche und die API nativ über das Feld &quot;CCPA-Opt-out&quot;. Um diese Informationen in Version 19.3 nutzen zu können, müssen Sie dieses Feld in Adobe Campaign Standard erstellen. Weitere Informationen finden Sie in der [detaillierten Dokumentation](https://helpx.adobe.com/de/campaign/kb/acs-privacy.html#ccpa).
>
> Sie können Ihre Version überprüfen, indem Sie auf das Symbol &quot;?&quot; oben rechts in der Benutzeroberfläche klicken und &quot;Info&quot; auswählen.

## Video-Tutorials

### Voraussetzungen für Datenschutzanforderungen

1. [Erstellen eines Namensraums](/help/privacy/namespaces-for-privacy-requests.md)
1. [Benutzerdefinierte Ressourcen ändern](/help/privacy/custom-resources-for-privacy-requests.md)

### Erstellen, verfolgen und ausführen von Datenschutzanforderungen über die Adobe Campaign-Benutzeroberfläche

* [Erstellen und verfolgen Sie Datenschutzanforderungen über die Benutzeroberfläche von Adobe Campaign](/help/privacy/create-and-track-privacy-requests.md)
* [Datenschutzanforderungen ausführen](/help/privacy/execute-privacy-requests.md)

## Zusätzliche Ressourcen

* [Allgemeine Datenschutzrichtlinien für Campaign](https://helpx.adobe.com/de/campaign/kb/campaign-privacy-overview.html)
* [CCPA für ACS](https://helpx.adobe.com/campaign/kb/acs-privacy.html#ccpa)
* [Adobe Experience Platform Privacy Service](https://adobe.io/apis/cloudplatform/gdpr.html)
* [Adobe Campaign Standard REST API-Dokumentation](https://final-docs.campaign.adobe.com/doc/standard/en/api/ACS_API.html#privacy-management)
