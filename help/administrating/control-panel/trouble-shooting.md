---
title: Probleme beim Aufschießen des Control Panels
description: Mit dem Control Panel können Sie Ihre SFTP-Datenspeicherung nach Instanz und Zulassungsliste-IP-Adressen überwachen und verwalten.
feature: Control Panel
topics: null
kt: 2938
doc-type: article
activity: use
team: PM
translation-type: tm+mt
source-git-commit: 2f0527f3d9e2248eea68079e00855cce7a96fce4
workflow-type: tm+mt
source-wordcount: '357'
ht-degree: 3%

---


# Probleme beim Schießen des [!UICONTROL Control Panels]

Erfahren Sie, wie Sie Probleme bei der Verwendung des Control Panels beheben können.

## Anmelden und Homepage

Probleme bei der Anmeldung und Homepage.

### Symptom: Anmeldung bei Adobe Experience Cloud nicht möglich

**Vorgehensweise:**
Der Benutzer muss seinen [!DNL IMS Org ID] (xxx) finden. Der Administrator muss den Benutzer für jede Instanz, die er verwalten möchte, dem [!UICONTROL Profil] des Produkts hinzufügen [!DNL “Campaign-xxx-Admins”] . Wenn der Benutzer ein Administrator aller Instanzen ist, muss er sich möglicherweise selbst als *[!UICONTROL Benutzer]* hinzufügen.

### Symptom: Links in der [!UICONTROL Adobe Experience Cloud-Startseite] für den Zugriff auf [!UICONTROL Control Panel] werden für Benutzer nicht angezeigt

**Ursache:**
Benutzer sehen die Links erst dann als Benutzer zum [!UICONTROL Profil des Produkts] `Campaign-xxx-Administrators/Admin`

**Vorgehensweise:**
Der Administrator muss den Benutzer für jede Instanz, die er verwalten möchte, dem [!UICONTROL Profil] des Produkts hinzufügen *[!DNL Campaign-xxx-Admins]* . Wenn der Benutzer ein Administrator aller Instanzen ist, muss er sich möglicherweise selbst als *[!UICONTROL Benutzer]* hinzufügen.

### Symptom: Eine Instanz wird nicht im [!UICONTROL Control Panel aufgeführt]

**Ursache:**
In der Regel muss der Benutzer als *[!UICONTROL Benutzer]* -Profil `!DNL Campaign-xxx-Administrators/Admin` für die fehlende Instanz hinzugefügt werden

**Vorgehensweise:**
Der Administrator muss den Profil für jede Instanz, die er verwalten möchte, dem Produkt- hinzufügen. `Campaign-xxx-Admins` Wenn der Benutzer ein Administrator aller Instanzen ist, muss er sich möglicherweise selbst als *[!UICONTROL Benutzer]* hinzufügen.

### Hilfreiche Videos

>[!VIDEO](https://video.tv.adobe.com/v/27183?quality=12)
*Prüfung[!DNL IMS Org ID](00:26 Min.)*

>[!VIDEO](https://video.tv.adobe.com/v/27147?quality=12)
*Hinzufügen eines Administrators zum[!UICONTROL Produkt-Profil]*[!DNL administrators]*, um[!UICONTROL Control Panel]verwenden zu können (01:03 Min.)*

### Hilfreiche Dokumentation

* [Entdecken Sie den [!UICONTROL Control Panel]](https://helpx.adobe.com/campaign/kb/control-panel-overview.html)
* [[!UICONTROL Berechtigungen für das Control Panel verwalten]](https://helpx.adobe.com/campaign/kb/control-panel-access.html)

## Verbindung zum SFTP-Server herstellen (Client oder API)

Für die Verbindung mit den SFTP-Servern ist Folgendes erforderlich:

* [!UICONTROL die Auflistung] der IP-Adresse zulassen, von der Sie eine Verbindung zum SFTP-Server herstellen
* Private/öffentliche Schlüsselpaare, die bei Adobe Campaign registriert werden müssen
* Wenn Sie eine direkte Verbindung zum SFTP-Server herstellen, benötigen Sie auch die SFTP-Clientsoftware

### Hilfreiche Dokumentation

* [Anmeldung bei Ihrem SFTP-Server](https://helpx.adobe.com/campaign/kb/control-panel-sftp.html#LoggingintoyourSFTPserver)

