---
title: 'Schritt 1: Erstellen einer Android-App und Konfigurieren für die Verwendung von Firebase Cloud-Nachrichten'
description: In diesem Teil erstellen wir [!DNL Android] App to receive [!UICONTROL Push notifications] die von Adobe Campaign Standard gesendet werden. Um die Push-Benachrichtigungen zu erhalten, muss die App bei Google registriert sein. [!DNL Firebase Cloud Service]
feature: Push
topics: Mobile
kt: 4825
doc-type: tutorial
activity: use
team: TM
translation-type: tm+mt
source-git-commit: cdd78e97f2769503d3d4f26933ccc7f35e9b20b9
workflow-type: tm+mt
source-wordcount: '359'
ht-degree: 0%

---


# Schritt 1: Erstellen der App und Konfigurieren der Verwendung von [!DNL Firebase Cloud Messaging][!DNL Android]

In diesem Teil erstellen Sie die App [!DNL Android], um [!UICONTROL Push-Benachrichtigungen] von Adobe Campaign Standard zu empfangen. Um die Push-Benachrichtigungen zu erhalten, muss die App bei Google [!DNL Firebase Cloud Service] registriert sein.

1. Melden Sie sich bei Ihrem [!DNL Firebase]-Konto an.

   [!DNL Firebase] ist die mobile Plattform von Google, mit der Sie schnell hochwertige Apps entwickeln können. Wenn Sie kein [!DNL Firebase]-Konto haben, erstellen Sie bitte ein [von hier](https://firebase.google.com).

2. Starten [!DNL Android Studio]
3. Klicken Sie auf **[!UICONTROL Datei]** > **[!UICONTROL Neu]** > **[!UICONTROL Neues Projekt].**.
4. Wählen Sie **[!UICONTROL Leere Aktivität]** und klicken Sie auf **[!UICONTROL Weiter].**

   ![android-Projekt](assets/android-project.PNG)

5. Geben Sie einen aussagekräftigen Namen für das Projekt ein.

   Für diese Demo haben wir unser Projekt als *[!DNL ACSPushTutorial]* bezeichnet

   ![android-project-configuration](assets/android-project-configuration.PNG)

6. Akzeptieren Sie die standardmäßigen Paketnamen und klicken Sie auf **[!DNL Finish]**, um Ihr Projekt zu erstellen.
7. Die Projektstruktur sollte dem Screenshot unten ähneln

   ![android-project-structure](assets/android-project-structure.PNG)

8. Klicken Sie auf **[!UICONTROL Tools]** > **[!UICONTROL Firebase].** (Hierdurch wird das Projekt hinzugefügt  [!DNL Firebase])
9. Klicken Sie auf **[!UICONTROL Firebase Cloud Messaging] einrichten.**

   ![setup firebase](assets/android-project-firebase-messaging.PNG)

10. Klicken Sie auf **[!UICONTROL Verbindung zu Firebase] herstellen.**
11. Nachdem Ihre App mit Firebase verbunden ist, klicken Sie auf **[!UICONTROL Hinzufügen FCM zu Ihrer App].**
12. Klicken Sie auf **[!UICONTROL Änderungen annehmen].**

   Wenn Sie Ihrer App FCM hinzufügen, benötigt der Assistent Ihre Berechtigung, um einige Änderungen an Ihrem Projekt vorzunehmen.

   ![[!DNL add-fcm-to-your-app]](assets/firebase-add-fcm-to-app.PNG)

Bei erfolgreicher Integration Ihrer App mit Firebase erhalten Sie eine Meldung wie die folgende:

![[!DNL fcm-successfull]](assets/android-firebase-success.PNG)

[Vergewissern Sie sich, dass Ihr Projekt  [!DNL Firebase ]in der Konsole aufgeführt ist](https://console.firebase.google.com/)

## Einstellungen für [!UICONTROL Push-Kanal]

1. Anmelden bei [!DNL Firebase]-Konsole
2. Öffnen Sie das Projekt **[!UICONTROL ACSPushTutorial]**.
3. Klicken Sie auf das Zahnradsymbol **und öffnen Sie die Projekteinstellungen**

   ![Projekteinstellungen](assets/firebase-project-settings.PNG)

4. Registerkarten auf der Registerkarte **[!UICONTROL Cloud Messaging]**.
5. Kopieren Sie den Serverschlüssel

   ![server-key](assets/firebase-server-key.PNG)

6. Bei Ihrer Adobe Campaign Standard-Instanz anmelden
7. Klicken Sie auf **[!UICONTROL Adobe Campaign]** > **[!UICONTROL Administration]** > **[!UICONTROL Kanal]** > **[!UICONTROL Mobilanwendung].**
8. Wählen Sie die entsprechende **[!UICONTROL Mobilanwendungseigenschaft].**
9. Klicken Sie auf das Symbol **[!DNL Android]** im Abschnitt **[!UICONTROL Push Kanal settings]**.
10. Fügen Sie den Serverschlüssel in das Feld für den Serverschlüssel ein.

Wenn alles gut läuft, sollte eine SUCCESS-Meldung angezeigt werden.

![push-Kanal-settings](assets/push-channel-settings.PNG)

Zusammenfassend haben wir ein [!DNL Android App] erstellt und das [!DNL Android App] mit [!DNL Firebase] verbunden. Anschließend wurde die mobile App in Adobe Campaign mit dem [!DNL Android App] verbunden, indem der [!DNL Android]-Serverschlüssel der App in die mobile App in Adobe Campaign Standard eingefügt wurde.
