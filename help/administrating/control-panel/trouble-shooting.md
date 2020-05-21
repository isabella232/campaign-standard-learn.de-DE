---
title: Probleme beim Aufnehmen der Systemsteuerung
description: Über die Systemsteuerung können Sie Ihre SFTP-Datenspeicherung nach Instanz- und Whitelist-IP-Adressen überwachen und verwalten.
feature: Control Panel
topics: null
kt: 2938
doc-type: article
activity: use
team: PM
translation-type: tm+mt
source-git-commit: cb5d5bc58137fd374eafe165c6ea13288a60d7db
workflow-type: tm+mt
source-wordcount: '356'
ht-degree: 3%

---


# Probleme beim Aufnehmen der [!UICONTROL-Systemsteuerung]

Erfahren Sie, wie Sie Probleme mit der Systemsteuerung beheben können.

## Anmelden und Homepage

Probleme bei der Anmeldung und Homepage.

### Symptom: Anmeldung bei Adobe Experience Cloud nicht möglich

**Vorgehensweise:**
Der Benutzer muss seinen [!DNL IMS Org ID] (xxx) finden. Der Administrator muss den Benutzer für jede Instanz, die er verwalten möchte, dem [!UICONTROL Profil] des Produkts hinzufügen [!DNL “Campaign-xxx-Admins”] . Wenn der Benutzer ein Administrator aller Instanzen ist, muss er sich möglicherweise selbst als *[!UICONTROL Benutzer]* hinzufügen.

### Symptom: Links in der [!UICONTROL Adobe Experience Cloud-Startseite] zum Zugriff auf die [!UICONTROL Systemsteuerung] werden für Benutzer nicht angezeigt

**Ursache:**
Benutzer sehen die Links erst dann als Benutzer zum [!UICONTROL Profil des Produkts] `Campaign-xxx-Administrators/Admin`

**Vorgehensweise:**
Der Administrator muss den Benutzer für jede Instanz, die er verwalten möchte, dem [!UICONTROL Profil] des Produkts hinzufügen *[!DNL Campaign-xxx-Admins]* . Wenn der Benutzer ein Administrator aller Instanzen ist, muss er sich möglicherweise selbst als *[!UICONTROL Benutzer]* hinzufügen.

### Symptom: Eine Instanz wird nicht in der [!UICONTROL Systemsteuerung aufgeführt]

**Ursache:**
In der Regel muss der Benutzer als *[!UICONTROL Benutzer]* -Profil `!DNL Campaign-xxx-Administrators/Admin` für die fehlende Instanz hinzugefügt werden

**Vorgehensweise:**
Der Administrator muss den Profil für jede Instanz, die er verwalten möchte, dem Produkt- hinzufügen. `Campaign-xxx-Admins` Wenn der Benutzer ein Administrator aller Instanzen ist, muss er sich möglicherweise selbst als *[!UICONTROL Benutzer]* hinzufügen.

### Hilfreiche Videos

>[!VIDEO](https://video.tv.adobe.com/v/27183?quality=12)
*Prüfung[!DNL IMS Org ID](00:26 Min.)*

>[!VIDEO](https://video.tv.adobe.com/v/27147?quality=12)
*Hinzufügen eines Administrators zum[!UICONTROL Produkt-Profil]*[!DNL administrators]*, um die[!UICONTROL Systemsteuerung]verwenden zu können (01:03 Min.)*

### Hilfreiche Dokumentation

* [Entdecken Sie die [!UICONTROL Systemsteuerung]](https://helpx.adobe.com/campaign/kb/control-panel-overview.html)
* [[!UICONTROL Berechtigungen für das Control Panel verwalten]](https://helpx.adobe.com/campaign/kb/control-panel-access.html)

## Verbindung zum SFTP-Server herstellen (Client oder API)

Für die Verbindung mit den SFTP-Servern ist Folgendes erforderlich:

* [!UICONTROL Whitelisting] der IP-Adresse, von der Sie eine Verbindung zum SFTP-Server herstellen
* Private/öffentliche Schlüsselpaare, die bei Adobe Campaign registriert werden müssen
* Wenn Sie eine direkte Verbindung zum SFTP-Server herstellen, benötigen Sie auch die SFTP-Clientsoftware

### Hilfreiche Dokumentation

* [Anmeldung bei Ihrem SFTP-Server](https://helpx.adobe.com/campaign/kb/control-panel-sftp.html#LoggingintoyourSFTPserver)

