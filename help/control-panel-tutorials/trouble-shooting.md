---
title: Fehlerbehebung beim Control Panel
description: Mit dem Control Panel können Sie Ihre SFTP-Datenspeicherung nach Instanz überwachen und verwalten und IP-Adressen auf die Zulassungsliste setzen.
feature: Control Panel
topics: null
kt: 2938
doc-type: article
activity: use
team: PM
translation-type: tm+mt
source-git-commit: 747aa1610f29a9a9409091169c7b398523dd1f77
workflow-type: tm+mt
source-wordcount: '357'
ht-degree: 100%

---


# Fehlerbehebung beim [!UICONTROL Control Panel]

Erfahren Sie, wie Sie Probleme bei der Verwendung des Control Panels beheben können.

## Anmelden und Homepage

Probleme bei der Anmeldung und Homepage.

### Symptom: Anmeldung bei Adobe Experience Cloud nicht möglich.

**Vorgehensweise:**
Der Benutzer muss seine [!DNL IMS Org ID] (xxx) finden. Der Administrator muss den Benutzer für jede Instanz, die er verwalten möchte, dem [!UICONTROL Produktprofil] [!DNL “Campaign-xxx-Admins”] hinzufügen. Wenn der Benutzer ein Administrator aller Instanzen ist, muss er sich möglicherweise selbst als *[!UICONTROL Benutzer]* hinzufügen.

### Symptom: Links auf der [!UICONTROL Adobe Experience Cloud-Startseite] zum Zugriff auf das [!UICONTROL Control Panel] werden einem Benutzer nicht angezeigt.

**Ursache:**
Benutzer sehen die Links erst, wenn sie als Benutzer zum [!UICONTROL Produktprofil] `Campaign-xxx-Administrators/Admin` hinzugefügt werden.

**Vorgehensweise:**
Der Administrator muss den Benutzer für jede Instanz, die er verwalten möchte, dem [!UICONTROL Produktprofil] *[!DNL Campaign-xxx-Admins]* hinzufügen. Wenn der Benutzer ein Administrator aller Instanzen ist, muss er sich möglicherweise selbst als *[!UICONTROL Benutzer]* hinzufügen.

### Symptom: Eine Instanz wird nicht im [!UICONTROL Control Panel] aufgeführt.

**Ursache:**
Höchstwahrscheinlich muss der Benutzer als *[!UICONTROL Benutzer]* zum Produktprofil `Campaign-xxx-Administrators/Admin` für die fehlende Instanz hinzugefügt werden.

**Vorgehensweise:**
Der Administrator muss den Benutzer für jede Instanz, die er verwalten möchte, dem Produktprofil `Campaign-xxx-Admins` hinzufügen. Wenn der Benutzer ein Administrator aller Instanzen ist, muss er sich möglicherweise selbst als *[!UICONTROL Benutzer]* hinzufügen.

### Hilfreiche Videos

>[!VIDEO](https://video.tv.adobe.com/v/27183?quality=12)

*[!DNL IMS Org ID] prüfen (00:26 Min.)*

>[!VIDEO](https://video.tv.adobe.com/v/27147?quality=12)

*Hinzufügen eines Administrators zum [!UICONTROL Produktprofil] [!DNL administrators], um das [!UICONTROL Control Panel] zu verwenden (01:03 min)*

### Hilfreiche Dokumentation

* [[!UICONTROL Control Panel]](https://helpx.adobe.com/de/campaign/kb/control-panel-overview.html)
* [[!UICONTROL Verwalten von Berechtigungen für das Control Panel]](https://helpx.adobe.com/de/campaign/kb/control-panel-access.html)

## Herstellen einer Verbindung zum SFTP-Server (Client oder API)

Für die Verbindung mit den SFTP-Servern ist Folgendes erforderlich:

* Die IP-Adresse, von der Sie eine Verbindung zum SFTP-Server herstellen, muss auf der [!UICONTROL Zulassungsliste] stehen.
* Ein öffentlich-privates Schlüsselpaar, das bei Adobe Campaign registriert sein muss.
* Wenn Sie eine direkte Verbindung zum SFTP-Server herstellen, benötigen Sie auch die SFTP-Clientsoftware.

### Hilfreiche Dokumentation

* [Anmeldung bei Ihrem SFTP-Server](https://helpx.adobe.com/de/campaign/kb/control-panel-sftp.html#LoggingintoyourSFTPserver)

