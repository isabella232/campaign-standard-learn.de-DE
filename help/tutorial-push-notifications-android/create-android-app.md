---
title: 'Schritt 1: Erstellen der Android-App und Konfigurieren der Verwendung von Firebase Cloud Messaging'
description: In diesem Teil erstellen wir [!DNL Android] App zum Empfang [!UICONTROL Push-Benachrichtigungen] von Adobe Campaign Standard gesendet. Um die Push-Benachrichtigungen zu erhalten, muss die App bei Google registriert sein. [!DNL Firebase Cloud Service].
feature: Push
jira: KT-4825
doc-type: tutorial
activity: use
team: TM
recommendations: noDisplay
exl-id: f087d9f2-cce9-4903-977f-3c5b47522c06
source-git-commit: c84867ef59a10448a377a959d0b67ae71343a4aa
workflow-type: tm+mt
source-wordcount: '364'
ht-degree: 0%

---

# 1. Schritt - Erstellung [!DNL Android] App und zu verwendende Konfiguration [!DNL Firebase Cloud Messaging]

In diesem Teil erstellen Sie [!DNL Android] App zum Empfang [!UICONTROL Push-Benachrichtigungen] von Adobe Campaign Standard gesendet. Um die Push-Benachrichtigungen zu erhalten, muss die App bei Google registriert sein. [!DNL Firebase Cloud Service].

1. Bei Ihrer [!DNL Firebase] -Konto.

   [!DNL Firebase] ist die mobile Plattform von Google, mit der Sie schnell hochwertige Apps entwickeln können. Wenn Sie keine [!DNL Firebase] Konto erstellen, erstellen Sie bitte ein [von hier](https://firebase.google.com).

2. Starten [!DNL Android Studio]
3. Klicken **[!UICONTROL Datei]** > **[!UICONTROL Neu]** > **[!UICONTROL Neues Projekt].**
4. Auswählen **[!UICONTROL Leere Aktivität]** und klicken Sie auf **[!UICONTROL Nächste].**

   ![android-project](assets/android-project.PNG)

5. Geben Sie einen aussagekräftigen Namen für das Projekt an.

   Für diese Demo haben wir unser Projekt als *[!DNL ACSPushTutorial]*

   ![android-project-configuration](assets/android-project-configuration.PNG)

6. Akzeptieren Sie die standardmäßigen Paketnamen und klicken Sie auf **[!DNL Finish]** , um Ihr Projekt zu erstellen.
7. Die Projektstruktur sollte dem folgenden Screenshot ähneln

   ![android-project-structure](assets/android-project-structure.PNG)

8. Klicken **[!UICONTROL Instrumente]** > **[!UICONTROL Firebase].** (Dadurch wird das Projekt zu [!DNL Firebase])
9. Klicken **[!UICONTROL Firebase Cloud Messaging einrichten].**

   ![Einrichten der Firebase](assets/android-project-firebase-messaging.PNG)

10. Klicken **[!UICONTROL Verbindung zu Firebase herstellen].**
11. Nachdem Ihre App mit Firebase verbunden ist, klicken Sie auf **[!UICONTROL Hinzufügen von FCM zu Ihrer App].**
12. Klicken **[!UICONTROL Accept Changes].**

   Wenn Sie FCM zu Ihrer App hinzufügen, benötigt der Assistent Ihre Berechtigung, um einige Änderungen an Ihrem Projekt vorzunehmen.

   ![[!DNL add-fcm-to-your-app]](assets/firebase-add-fcm-to-app.PNG)

Bei erfolgreicher Integration Ihrer App mit Firebase erhalten Sie eine Meldung wie die folgende:

![[!DNL fcm-successfull]](assets/android-firebase-success.PNG)

[Stellen Sie sicher, dass Ihr Projekt in [!DNL Firebase ]console](https://console.firebase.google.com/)

## Konfigurieren [!UICONTROL Push-Kanal] Einstellungen

1. Anmelden bei [!DNL Firebase] console
2. Öffnen Sie die **[!UICONTROL ACSPushTutorial]** Projekt.
3. Klicken Sie auf **Zahnradsymbol** und öffnen Sie die Projekteinstellungen.

   ![project-settings](assets/firebase-project-settings.PNG)

4. Registerkarte zum **[!UICONTROL Cloud Messaging]** Registerkarte.
5. Kopieren des Serverschlüssels

   ![server-key](assets/firebase-server-key.PNG)

6. Bei Ihrer Adobe Campaign Standard-Instanz anmelden
7. Klicken **[!UICONTROL Adobe Campaign]** > **[!UICONTROL Administration]** > **[!UICONTROL Kanäle]** > **[!UICONTROL Mobile App].**
8. Wählen Sie die entsprechende **[!UICONTROL Eigenschaft für mobile Anwendungen].**
9. Klicken Sie auf **[!DNL Android]icon** im **[!UICONTROL Push-Kanal-Einstellungen]** Abschnitt.
10. Fügen Sie den Serverschlüssel in das Feld für den Serverschlüssel ein.

Wenn alles gut läuft, sollte eine SUCCESS-Meldung angezeigt werden.

![push-channel-settings](assets/push-channel-settings.PNG)

Zusammenfassend ist festzustellen, dass wir eine [!DNL Android App] und die [!DNL Android App] mit [!DNL Firebase]. Anschließend wurde die App in Adobe Campaign mit der [!DNL Android App] durch Einfügen der [!DNL Android] Der Serverschlüssel der App in der Mobile App in Adobe Campaign Standard.
