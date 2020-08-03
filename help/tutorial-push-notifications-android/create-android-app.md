---
title: 'Schritt 1: Erstellen einer Android-App und Konfigurieren für die Verwendung von Firebase Cloud-Nachrichten'
description: In diesem Teil werden wir aus Adobe Campaign Standard [!DNL Android] App to receive [!UICONTROL Push notifications] erstellen. Um die Push-Benachrichtigungen zu erhalten, muss die App bei Google registriert [!DNL Firebase Cloud Service]sein.
feature: Push
topics: Mobile
kt: 4825
doc-type: tutorial
activity: use
team: TM
translation-type: tm+mt
source-git-commit: afe1ae6c8d73b7b776e0eec327fa16db76c23ce1
workflow-type: tm+mt
source-wordcount: '359'
ht-degree: 0%

---


# Schritt 1: Erstellen der [!DNL Android] App und Konfigurieren für die Verwendung [!DNL Firebase Cloud Messaging]

In diesem Teil erstellen Sie eine [!DNL Android] App zum Empfangen von [!UICONTROL Push-Benachrichtigungen] von Adobe Campaign Standard. Um die Push-Benachrichtigungen zu erhalten, muss die App bei Google registriert sein [!DNL Firebase Cloud Service].

1. Melden Sie sich bei Ihrem [!DNL Firebase] Konto an.

   [!DNL Firebase] ist die mobile Plattform von Google, mit der Sie schnell hochwertige Apps entwickeln können. Wenn Sie kein [!DNL Firebase] Konto haben, erstellen Sie bitte eines [von hier](https://firebase.google.com).

2. Start [!DNL Android Studio]
3. Klicken Sie auf **[!UICONTROL Datei]** > **[!UICONTROL Neu]** > **[!UICONTROL Neues Projekt].**
4. Wählen Sie **[!UICONTROL Leere Aktivität]** und klicken Sie auf **[!UICONTROL Weiter].**

   ![android-Projekt](assets/android-project.PNG)

5. Geben Sie einen aussagekräftigen Namen für das Projekt ein.

   Für die Zwecke dieser Demo haben wir unser Projekt als *[!DNL ACSPushTutorial]*

   ![android-project-configuration](assets/android-project-configuration.PNG)

6. Akzeptieren Sie die standardmäßigen Paketnamen und klicken Sie auf **[!DNL Finish]** , um das Projekt zu erstellen.
7. Die Projektstruktur sollte dem Screenshot unten ähneln

   ![android-project-structure](assets/android-project-structure.PNG)

8. Klicken Sie auf **[!UICONTROL Werkzeuge]** > **[!UICONTROL Firebase].**(Hierdurch wird das Projekt hinzugefügt[!DNL Firebase])
9. Klicken Sie auf **[!UICONTROL Setup Firebase Cloud Messaging].**

   ![setup firebase](assets/android-project-firebase-messaging.PNG)

10. Klicken Sie auf **[!UICONTROL Mit Firebase]verbinden.**
11. Nachdem Ihre App mit Firebase verbunden ist, klicken Sie auf **[!UICONTROL Hinzufügen FCM zu Ihrer App].**
12. Klicken Sie auf Änderungen **[!UICONTROL annehmen].**

   Wenn Sie Ihrer App FCM hinzufügen, benötigt der Assistent Ihre Berechtigung, um einige Änderungen an Ihrem Projekt vorzunehmen.

   ![[!DNL add-fcm-to-your-app]](assets/firebase-add-fcm-to-app.PNG)

Bei erfolgreicher Integration Ihrer App mit Firebase erhalten Sie eine Meldung wie die folgende:

![[!DNL fcm-successfull]](assets/android-firebase-success.PNG)

[Vergewissern Sie sich, dass Ihr Projekt [!DNL Firebase ]in der Konsole aufgeführt ist](https://console.firebase.google.com/)

## Einstellungen für [!UICONTROL Push-Kanal] konfigurieren

1. Bei [!DNL Firebase] Konsole anmelden
2. Öffnen Sie das **[!UICONTROL ACSPushTutorial]** -Projekt.
3. Klicken Sie auf das **Zahnradsymbol** und öffnen Sie die Projekteinstellungen

   ![Projekteinstellungen](assets/firebase-project-settings.PNG)

4. Registerkarte zur Registerkarte **[!UICONTROL Cloud Messaging]** .
5. Kopieren Sie den Serverschlüssel

   ![server-key](assets/firebase-server-key.PNG)

6. Bei Ihrer Adobe Campaign Standard-Instanz anmelden
7. Klicken Sie auf **[!UICONTROL Adobe Campaign]** > **[!UICONTROL Administration]** > **[!UICONTROL Kanal]** > **[!UICONTROL Mobilanwendung].**
8. Wählen Sie die entsprechende **[!UICONTROL Mobilanwendungseigenschaft]aus.**
9. Klicken Sie auf das **[!DNL Android]Symbol **im Abschnitt mit den Einstellungen**[!UICONTROL des ]**Push-Kanals.
10. Fügen Sie den Serverschlüssel in das Feld für den Serverschlüssel ein.

Wenn alles gut läuft, sollte eine SUCCESS-Meldung angezeigt werden.

![push-Kanal-settings](assets/push-channel-settings.PNG)

Zusammenfassend haben wir eine [!DNL Android App] und verbunden die [!DNL Android App] mit [!DNL Firebase]. Anschließend haben wir die mobile App in Adobe Campaign mit der verbunden, [!DNL Android App] indem wir den Serverschlüssel der [!DNL Android] App in den Adobe Campaign Standard in die mobile App eingefügt haben.
