---
title: Einführung in In-App-Nachrichten
description: Erfahren Sie, wie Sie dem Benutzer als Reaktion auf das Echtzeit-Verhalten eines Kunden in der Mobile App kontextuell relevante In-App-Nachrichten präsentieren.
feature: In-App
kt: 1911
doc-type: feature video
activity: use
team: TM
exl-id: c51716eb-7239-4fc0-9ccf-9f5f0a5fae65
role: User
level: Beginner
source-git-commit: 30e8e10575aad4dcf2b0473cdd9fd6d5fc2815f4
workflow-type: tm+mt
source-wordcount: '758'
ht-degree: 16%

---

# Einführung in [!UICONTROL In-App]-Nachrichten {#introduction}

Mit dem Kanal [!UICONTROL In-App-Nachrichten] können Sie eine Nachricht anzeigen, wenn der Benutzer in der Mobile App aktiv ist. Für diesen Kanal müssen Mobile Apps in [!UICONTROL Adobe Experience Platform SDK] integriert werden.

In diesem Tutorial werden die zum Einrichten der mobilen Eigenschaften erforderlichen Schritte, die Erweiterung [!UICONTROL Launch] für den Kanal [!UICONTROL In-App-Nachrichten] sowie das Vorbereiten, Anpassen und Senden von [!UICONTROL In-App]-Nachrichten in Adobe Campaign Standard erläutert. Die Links führen zu den Video-Tutorials zu den einzelnen hervorgehobenen Themen.

## Voraussetzungen {#prerequisites}

1. Stellen Sie sicher, dass Sie auf den Kanal **[!UICONTROL In-App]** zugreifen können. Wenn Sie keinen Zugriff auf diesen Kanal haben, kontaktieren Sie das für Ihr Konto zuständige Team.
1. Vergewissern Sie sich, dass Ihr **Benutzer** über die erforderlichen **Berechtigungen** in Adobe Campaign Standard und [!UICONTROL Launch] verfügt.

   1. Stellen Sie in Adobe Campaign Standard sicher, dass der IMS-Benutzer Teil der Gruppen [!UICONTROL Standardbenutzer] und [!UICONTROL Administrator] ist.

      Dieser Schritt ermöglicht es dem Benutzer, sich bei Adobe Campaign Standard anzumelden, zur Experience Platform SDK-Seite für mobile Apps zu navigieren und die Eigenschaften der mobilen App anzuzeigen, die Sie in [!UICONTROL Launch] erstellt haben.

   1. Stellen Sie in [!UICONTROL Launch] sicher, dass Ihr IMS-Benutzer Teil eines [!UICONTROL Launch]-Produktprofils ist. Dieser Schritt ermöglicht es dem Benutzer, sich bei [!UICONTROL Launch] anzumelden, um die Eigenschaften zu erstellen und anzuzeigen. Im Produktprofil sollten keine Berechtigungen für das Unternehmen oder die Eigenschaften festgelegt sein, aber der Benutzer sollte sich trotzdem anmelden können.

1. In Adobe Experience Platform Launch:

   1. Erstellen Sie die Mobile App, indem Sie eine mobile Eigenschaft erstellen und Ihre Mobile App mit dem Experience Platform SDK instrumentieren.
   1. Installieren Sie die Erweiterung **Adobe Campaign Standard** für Ihre Mobile App.

Weitere Informationen zu Erweiterungen finden Sie unter [Konfigurieren der Campaign Standard-Erweiterung in Adobe Launch](https://aep-sdks.gitbook.io/docs/using-mobile-extensions/adobe-campaign-standard) in der Dokumentation.

## Schritte zum Einrichten von [!UICONTROL In-App]-Nachrichten {#steps-to-set-up}

1. [Konfigurieren einer Mobile App mithilfe von Adobe Experience Platform SDKs](/help/communication-channels/mobile/configure-mobile-apps-using-aep-sdk.md).
1. [Ereignisse konfigurieren](/help/communication-channels/mobile/in-app/configure-events.md).

## [!UICONTROL In-App] Sendungen erstellen, verwalten und veröffentlichen {#create-manage-publish}

Sie können entweder einmalige In-App-Sendungen erstellen, indem Sie auf der Startseite auf die Karte **[!UICONTROL In-App-Nachricht erstellen]** klicken, über [!UICONTROL Marketingaktivitäten] oder Sie können [In-App-Versand innerhalb eines Workflows](/help/communication-channels/mobile/in-app/in-app-activity.md) erstellen.

Beim Einrichten des Versands stehen Ihnen drei Optionen zur Verfügung, mit denen Sie aus unterschiedlichen Versandvorlagen auswählen können:

1. [**Senden einer In-App-**](/help/communication-channels/mobile/in-app/broadcast-in-app-message.md) Nachricht an alle Benutzer einer Mobile App.

   Mit diesem Nachrichtentyp können Sie Nachrichten an alle (aktuellen oder künftigen) Benutzer Ihrer Mobile App senden, selbst wenn in Adobe Campaign kein Profil existiert. Daher ist eine Personalisierung bei der Anpassung der Nachrichten nicht möglich, da das Benutzerprofil nicht unbedingt in Adobe Campaign vorhanden ist.

1. Targeting aller Benutzer auf der Basis ihres mobilen App-Profils.

   Mit diesem Nachrichtentyp können Sie alle bekannten oder anonymen Benutzer einer Mobile App auswählen, die über ein mobiles Profil in Adobe Campaign verfügen. Dieser Nachrichtentyp kann nur mit nicht-personenbezogenen und nicht-sensiblen Attributen personalisiert werden und benötigt auch keinen sicheren Handshake zwischen dem Mobile SDK und dem In-App-Messaging-Dienst von Adobe Campaign. Die Personalisierungsstrategie basiert also auf dem, was Sie über die Benutzer aus ihrer Interaktion mit dem Gerät gelernt haben. Geben Sie beispielsweise alle Benutzer als Ziel an, die ihre App in der letzten Woche mehr als fünfmal gestartet haben.

1. [**Ansprechen von Benutzern auf der Basis ihres Campaign-Profils**](/help/communication-channels/mobile/in-app/target-users-based-on-campaign-profile.md).

   Mit diesem Nachrichtentyp können Sie Adobe Campaign-Profile (CRM-Profile) auswählen, die sich für Ihre Mobile App angemeldet haben. Die Nachricht kann mit allen in Adobe Campaign verfügbaren Profilattributen personalisiert werden. Sie erfordert einen sicheren Handshake zwischen dem Mobile SDK und dem In-App-Messaging-Dienst von Campaign, um sicherzustellen, dass Nachrichten mit persönlichen und sensiblen Informationen nur von autorisierten Benutzern verwendet werden.

Diese Vorlage ist nützlich, um Anwendungsfälle für die kanalübergreifende Orchestrierung der Customer Journey zu unterstützen, bei denen Sie bereits Benutzer auf andere Kanäle wie E-Mail oder Push angesprochen haben. Je nach Antwort möchten Sie dann mit einer In-App-Nachricht interagieren.

## Berichte zu In-App-Sendungen erstellen {#report}

Nachdem Ihr Versand veröffentlicht wurde, können Sie [einen Bericht zu Ihrem In-App-Versand erstellen](/help/communication-channels/mobile/in-app/in-app-reporting.md).

## Zusätzliche Ressourcen

* [In-App-Bericht](https://experienceleague.adobe.com/docs/campaign-standard/using/reporting/list-of-reports/in-app-report.html?lang=en)
* [Einrichten einer mobilen Eigenschaft](https://aep-sdks.gitbook.io/docs/getting-started/create-a-mobile-property)
* [Konfiguration einer Mobile App mithilfe von Adobe Experience Platform SDKs](https://experienceleague.adobe.com/docs/campaign-standard/using/administrating/configuring-channels/configuring-a-mobile-application.html?lang=en)
* [In-App-Nachricht vorbereiten und senden](https://experienceleague.adobe.com/docs/campaign-standard/using/communication-channels/in-app-messaging/preparing-and-sending-an-in-app-message.html?lang=en)
* [In-App-Nachricht anpassen](https://experienceleague.adobe.com/docs/campaign-standard/using/communication-channels/in-app-messaging/customizing-an-in-app-message.html?lang=en)
* [In-App-Nachricht in einem Workflow senden](https://experienceleague.adobe.com/docs/campaign-standard/using/managing-processes-and-data/channel-activities/in-app-delivery.html?lang=en)
* [Lebenszyklusmetriken aktivieren](https://aep-sdks.gitbook.io/docs/getting-started/initialize-the-sdk#enable-lifecycle-metrics)
