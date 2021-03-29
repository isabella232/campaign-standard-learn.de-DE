---
title: Datenschutzanfragen bei Adobe Campaign Standard (ACS) – Überblick
description: In dem Tutorial wird erläutert, wie Datenschutzanfragen über die Benutzeroberfläche von Adobe Campaign Standard (ACS) erstellt werden.
feature: DSGVO, CCAP
topic: Datenschutz
kt: 1480
doc-type: feature video
activity: use
team: TM
translation-type: ht
source-git-commit: 556bff4c94e16d3a94561dee1ccb311bc003b631
workflow-type: ht
source-wordcount: '373'
ht-degree: 100%

---


# Datenschutzanfragen über die Adobe Campaign Standard-Benutzeroberfläche

Adobe Campaign bietet Datenverantwortlichen drei Methoden zum Ausführen von Datenschutzzugriffs- und Löschanfragen von PII-Daten unter Einhaltung von Datenschutzvorschriften wie der DSGVO (Datenschutz-Grundverordnung) und dem CCPA (California Consumer Privacy Act):

* **Über die Integration von Privacy Core Service:** Die von [!UICONTROL Privacy Service] an alle Experience Cloud-Lösungen übertragenen Datenschutzanfragen werden von Campaign mithilfe eines speziellen Workflows automatisch verarbeitet. Weitere Informationen zum Erstellen von Datenschutzanfragen mithilfe von Privacy Core Service finden Sie in der Dokumentation zum [Adobe Experience Platform Privacy Service](https://adobe.io/apis/cloudplatform/gdpr.html).

* **Über die API:** Adobe Campaign bietet eine API, mit der Datenschutzanfragen durch die Verwendung von REST automatisch verarbeitet werden können.

* **Über die Adobe Campaign-Benutzeroberfläche:** Für jede Datenschutzanfrage erstellt der Datenverantwortliche eine neue Datenschutzanfrage in Adobe Campaign.

>[!NOTE]
>
> **ÄNDERUNGEN BEI ACS 19.4:**
> 
> Die [Privacy Service-Integration](https://adobe.io/apis/cloudplatform/gdpr.html) ist die Methode, die Sie für alle Zugriffs- und Löschanfragen verwenden sollten. Mit Version 19.4. wurde die Campaign-API und -Schnittstelle für Zugriffs- und Löschanfragen eingestellt. Weiterführende Informationen zu veralteten und entfernten Funktionen von Campaign Standard finden Sie auf [dieser Seite](https://helpx.adobe.com/de/campaign/kb/acs-deprecated-and-removed-features.html).
>
>**Opt-out aus dem Verkauf von personenbezogenen Daten (CCPA)**
>
>Ab Version 19.4. verfügen die Campaign-Oberfläche und die API nativ über das Feld &quot;CCPA-Opt-out&quot;. Um diese Informationen in Version 19.3 nutzen zu können, müssen Sie dieses Feld in Adobe Campaign Standard erstellen. Weitere Informationen finden Sie in der [entsprechenden Dokumentation](https://helpx.adobe.com/de/campaign/kb/acs-privacy.html#ccpa).
>
> Sie können Ihre Version überprüfen, indem Sie auf das Symbol &quot;?&quot; oben rechts in der Benutzeroberfläche klicken und &quot;Info&quot; auswählen.

## Video-Tutorials

### Voraussetzungen für Datenschutzanfragen

1. [Namespace erstellen](/help/privacy/namespaces-for-privacy-requests.md)
1. [Benutzerdefinierte Ressourcen ändern](/help/privacy/custom-resources-for-privacy-requests.md)

### Datenschutzanfragen über die Adobe Campaign-Benutzeroberfläche erstellen, verfolgen und ausführen

* [Erstellen und Verfolgen von Datenschutzanfragen über die Adobe Campaign-Benutzeroberfläche](/help/privacy/create-and-track-privacy-requests.md)
* [Ausführen von Datenschutzanfragen](/help/privacy/execute-privacy-requests.md)

## Zusätzliche Ressourcen

* [Allgemeine Datenschutzrichtlinien für Campaign](https://helpx.adobe.com/de/campaign/kb/campaign-privacy-overview.html)
* [CCPA für ACS](https://helpx.adobe.com/de/campaign/kb/acs-privacy.html#ccpa)
* [Adobe Experience Platform Privacy Service](https://adobe.io/apis/cloudplatform/gdpr.html)
* [Adobe Campaign Standard REST API-Dokumentation](https://final-docs.campaign.adobe.com/doc/standard/en/api/ACS_API.html#privacy-management)
