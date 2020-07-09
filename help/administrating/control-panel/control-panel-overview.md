---
title: Control Panel
description: Über die Systemsteuerung können Sie Ihre SFTP-Datenspeicherung nach Instanz und zulassungsliste-IP-Adressen überwachen und verwalten.
feature: Control Panel
topics: Control Panel
kt: 4696
doc-type: feature video
activity: use
team: PM
translation-type: tm+mt
source-git-commit: db20c4e6aeb10dc04a6c4556fefaa8cd18366c44
workflow-type: tm+mt
source-wordcount: '417'
ht-degree: 6%

---


# [!UICONTROL Control Panel] {#control-panel}

>[!NOTE]
>
>Die Begriffe &quot;[!UICONTROL Whitelist]&quot;und &quot;[!UICONTROL schwarze Liste]&quot;wurden in den Unterlagen zum Adobe Campaign durch &quot;[!UICONTROL zulassungsliste]&quot;und &quot;[!UICONTROL blockierungsliste]&quot;ersetzt. Einige Vorkommen dieser Begriffe befinden sich möglicherweise noch in der Produktoberfläche, in Optionsnamen, im internen Code sowie in den Übungsvideos. Sie werden in den kommenden Versionen der Systemsteuerung ersetzt.

Die [!UICONTROL Systemsteuerung] ermöglicht es Adobe Campaign-Administratoren, wichtige Assets zu überwachen und administrative Aufgaben durchzuführen, z. B. die Verwaltung der SFTP-Datenspeicherung nach Instanz oder [!UICONTROL zulassungsliste] -IP-Adressen.

## Accessing [!UICONTROL Control Panel]

Um auf die Systemsteuerung zuzugreifen, gehen Sie zu Experience Cloud Home: [https://experiencecloud.adobe.com](https://experiencecloud.adobe.com):

* **[!UICONTROL Experience Cloud-Startseite]** > **[!UICONTROL Schnellzugriff]**

   oder
* **[!UICONTROL Experience Cloud-Startseite]** > [!UICONTROL Lösungsauswahl]: **Kampagne** > **[!UICONTROL Bedienfeldkarte]**

   oder

* Direkt von der URL: [https://experience.adobe.com/#/controlpanel](https://experience.adobe.com/#/controlpanel)

## Voraussetzungen

Bevor Sie beginnen, müssen Sie die folgenden Voraussetzungen erfüllen:

### Bestätigen [!DNL IMS Org ID]

Du musst dein [!DNL IMS org ID]wissen. Im folgenden Video wird beschrieben, wo Sie die Instanz suchen können [!DNL IMS org ID].

>[!VIDEO](https://video.tv.adobe.com/v/27183?quality=12)
*Prüfung[!DNL IMS Org ID](00:26 Min.)*

### Administratorrechte

Für den Zugriff auf die [!UICONTROL Systemsteuerung]sind Administratorrechte erforderlich.
Im folgenden Video wird erläutert, wie Sie einer Instanz einer Kampagne einen Administrator hinzufügen

>[!VIDEO](https://video.tv.adobe.com/v/27147?quality=12)
*Hinzufügen eines Administrators zum Profil &quot;[!UICONTROL Administratoren]&quot;zur Verwendung der[!UICONTROL Systemsteuerung](01:03 Min.)*

## Bedienfeldübungen

* **Verwalten von SFTP-Servern**

   *Erfahren Sie, wie Sie die Serverkapazität und die zulassungsliste-IP-Adressen überwachen und SSH-Schlüssel hinzufügen können:*

   * [Überwachen der Serverkapazität, Auflisten von IP-Adressen und Hinzufügen von SSH-Schlüsseln](/help/administrating/control-panel/monitoring-server-capacity-allow-listing-adding-ssh-key.md)
   * [Erstellen eines SSH-Schlüssels](/help/administrating/control-panel/generate-ssh-key.md)
   * [Herstellen einer Verbindung zu einem SFTP-Server](/help/administrating/control-panel/connect-to-sftp-server.md)
* **[Subdomänen übertragen](/help/administrating/control-panel/subdomain-delegation.md)**

   *Erfahren Sie, wie Sie eine Subdomäne vollständig an Adobe Campaign delegieren*
* **[SSL-Zertifikate hinzufügen](/help/administrating/control-panel/adding-ssl-certificates.md)**

   *Erfahren Sie, wie Sie SSL-Zertifikate hinzufügen können, um Ihre Subdomänen zu schützen.*
* **[Verwalten von SSL-Zertifikaten](/help/administrating/control-panel/managing-ssl-certificates.md)**

   *Erfahren Sie, wie Sie den Status der SSL-Zertifikate Ihrer Subdomänen sowie Erneuerungen anfordern können.*
* **[Verwaltung von Google TXT-Einträgen](/help/administrating/control-panel/google-txt-record-management.md)**

   *Erfahren Sie, wie Sie allen Subdomänen, die zum Senden von E-Mails an GMAIL-Adressen verwendet werden, über die Systemsteuerung der Kampagne Google TXT-Site-Überprüfungsdatensätze hinzufügen.*

* **GPG-Schlüsselverwaltung**

   *Erfahren Sie, wie Sie ein Public-Private-Key-Paar für die Verschlüsselung ausländischer Kampagnen auf einer angegebenen Instanz erstellen und installieren sowie einen öffentlichen Schlüssel für die Entschlüsselung eingehender Daten importieren und auf einer Kampagne installieren:*

   * [Generieren und Installieren von GPG-Schlüsseln für die Datenverschlüsselung](./gpg-key-management/generating-and-installing-gpg-keys-for-data-encryption.md)
   * [Verschlüsseln von Daten mit einem GPG-Schlüssel](./gpg-key-management/using-a-gpg-key-to-encrypt-data.md)
   * [Entschlüsseln von Daten](./gpg-key-management/decrypting-data.md)

* **[Probleme beim Schießen](/help/administrating/control-panel/trouble-shooting.md)**

   *Informationen zur Fehlerbehebung in der Systemsteuerung*

## Zusätzliche Ressourcen

* [Hilfe-Center für Systemsteuerung](https://docs.adobe.com/content/help/de-DE/control-panel/using/control-panel-home.html)

