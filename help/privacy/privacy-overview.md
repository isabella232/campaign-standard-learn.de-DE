---
title: Datenschutzanfragen bei Adobe Campaign Standard (ACS) – Überblick
description: In diesem Tutorial wird erläutert, wie die Erstellung von Datenschutzanfragen über die Adobe Campaign Standard-Benutzeroberfläche erfolgt.
feature: Datenschutz-Tools
kt: 1480
doc-type: feature video
activity: use
team: TM
exl-id: fb766403-694c-4a7b-b3d1-4a418df85891
source-git-commit: 481cbdcc9ac7446cc36fbff6e3d6e43fe333d30b
workflow-type: tm+mt
source-wordcount: '353'
ht-degree: 62%

---

# Datenschutzanfragen über die Adobe Campaign Standard-Benutzeroberfläche

Adobe Campaign bietet Datenverantwortlichen drei Methoden zum Ausführen von Datenschutzzugriffs- und Löschanfragen von PII-Daten unter Einhaltung von Datenschutzvorschriften wie der DSGVO (Datenschutz-Grundverordnung) und dem CCPA (California Consumer Privacy Act):

* **Über die Integration von Privacy Core Service:** Die von [!UICONTROL Privacy Service] an alle Experience Cloud-Lösungen übertragenen Datenschutzanfragen werden von Campaign mithilfe eines speziellen Workflows automatisch verarbeitet. Informationen zum Erstellen von Datenschutzanfragen über den Privacy Core Service finden Sie unter [Adobe Experience Platform Privacy Service](https://www.adobe.io/apis/experienceplatform/gdpr.html)

* **Über die API:** Adobe Campaign bietet eine API, mit der Datenschutzanfragen durch die Verwendung von REST automatisch verarbeitet werden können.

* **Über die Adobe Campaign-Benutzeroberfläche:** Für jede Datenschutzanfrage erstellt der Datenverantwortliche eine Datenschutzanfrage in Adobe Campaign.

>[!NOTE]
>
> **ÄNDERUNGEN BEI ACS 19.4:**
> 
> Die [Privacy Service-Integration](https://www.adobe.io/apis/experienceplatform/gdpr.html) ist die Methode, die Sie für alle Zugriffs- und Löschanfragen verwenden sollten. Mit Version 19.4. wurde die Campaign-API und -Schnittstelle für Zugriffs- und Löschanfragen eingestellt. Weiterführende Informationen zu veralteten und entfernten Funktionen von Campaign Standard finden Sie auf [dieser Seite](https://experienceleague.adobe.com/docs/campaign-standard/using/release-notes/deprecated-features.html?lang=en).
>
>**Opt-out aus dem Verkauf von personenbezogenen Daten (CCPA)**
>
> In der Campaign-Benutzeroberfläche und der API ist standardmäßig ein Feld für die CCPA-Abmeldung verfügbar.
>
> Sie können Ihre Version überprüfen, klicken Sie auf **?** oben rechts in der Benutzeroberfläche klicken und &quot;Info&quot; auswählen.

## Video-Tutorials

### Voraussetzungen für Datenschutzanfragen

1. [Namespace erstellen](/help/privacy/namespaces-for-privacy-requests.md)
1. [Benutzerdefinierte Ressourcen ändern](/help/privacy/custom-resources-for-privacy-requests.md)

### Erstellen, verfolgen und Ausführen von Datenschutzanfragen über die Benutzeroberfläche von Adobe Campaign

* [Erstellen und Verfolgen von Datenschutzanfragen über die Adobe Campaign-Benutzeroberfläche](/help/privacy/create-and-track-privacy-requests.md)
* [Ausführen von Datenschutzanfragen](/help/privacy/execute-privacy-requests.md)

## Zusätzliche Ressourcen

* [Allgemeine Datenschutzrichtlinien für Campaign](https://experienceleague.adobe.com/docs/campaign-classic/using/getting-started/privacy/privacy-management.html?lang=en#getting-started)
* [CCPA für ACS](https://experienceleague.adobe.com/docs/campaign-standard/using/getting-started/privacy/privacy-requests.html?lang=en#privacy-requests)
* [Adobe Experience Platform Privacy Service](https://www.adobe.io/apis/experienceplatform/gdpr.html)
* [Adobe Campaign Standard REST API-Dokumentation](https://final-docs.campaign.adobe.com/doc/standard/en/api/ACS_API.html#privacy-management)
