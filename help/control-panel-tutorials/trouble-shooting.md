---
title: Fehlerbehebung beim Control Panel
description: Mit dem Control Panel können Sie Ihren SFTP-Speicher nach Instanz und IP-Adressen der Zulassungsliste überwachen und verwalten.
feature: Control Panel
kt: 2938
doc-type: article
activity: use
team: PM
exl-id: f546f791-a69b-4586-abfa-3e626b8feb17
source-git-commit: 481cbdcc9ac7446cc36fbff6e3d6e43fe333d30b
workflow-type: tm+mt
source-wordcount: '350'
ht-degree: 47%

---

# Fehlerbehebung beim [!UICONTROL Control Panel]

Erfahren Sie, wie Sie Probleme bei der Verwendung des Control Panels beheben können.

## Anmelden und Homepage

Probleme bei der Anmeldung und Homepage.

### Symptom: Anmeldung bei Adobe Experience Cloud nicht möglich

**Vorgehensweise:**
Der Benutzer muss seine  [!DNL IMS Org ID] (xxx) finden. Der Administrator muss den Benutzer für jede Instanz, die er verwalten möchte, dem [!UICONTROL Produktprofil] [!DNL “Campaign-xxx-Admins”] hinzufügen. Wenn der Benutzer ein Administrator aller Instanzen ist, muss er sich selbst als *[!UICONTROL Benutzer]* hinzufügen.

### Symptom: Links auf der [!UICONTROL Adobe Experience Cloud-Startseite] zum Zugriff auf das [!UICONTROL Control Panel] werden einem Benutzer nicht angezeigt.

**Ursache:**
Benutzer sehen die Links erst, wenn sie als Benutzer zum [!UICONTROL Produktprofil] `Campaign-xxx-Administrators/Admin` hinzugefügt werden.

**Vorgehensweise:**
Der Administrator muss den Benutzer für jede Instanz, die er verwalten möchte, dem  [!UICONTROL Produktprofil ] *[!DNL Campaign-xxx-Admins]* hinzufügen. Wenn der Benutzer ein Administrator aller Instanzen ist, muss er sich selbst als *[!UICONTROL Benutzer]* hinzufügen.

### Symptom: Eine Instanz wird im [!UICONTROL Control Panel] nicht aufgeführt

**Ursache:**
Der Benutzer muss höchstwahrscheinlich als  ** userProduct Profile  `Campaign-xxx-Administrators/Admin` für die fehlende Instanz hinzugefügt werden.

**Vorgehensweise:**
Der Administrator muss den Benutzer  `Campaign-xxx-Admins` für jede Instanz, die er verwalten möchte, dem Produktprofil hinzufügen. Wenn der Benutzer ein Administrator aller Instanzen ist, muss er sich selbst als *[!UICONTROL Benutzer]* hinzufügen.

### Nützliche Videos

>[!VIDEO](https://video.tv.adobe.com/v/27183?quality=12)

*Prüfen [!DNL IMS Org ID] (00:26 Min.)*

>[!VIDEO](https://video.tv.adobe.com/v/27147?quality=12)

*Hinzufügen eines Administrators zum [!UICONTROL Produktprofil] [!DNL administrators], um das [!UICONTROL Control Panel] zu verwenden (01:03 min)*

### Hilfreiche Dokumentation

* [[!UICONTROL Control Panel]](https://experienceleague.adobe.com/docs/control-panel/using/control-panel-home.html?lang=de)
* [[!UICONTROL Verwalten von Berechtigungen für das Control Panel]](https://experienceleague.adobe.com/docs/control-panel/using/control-panel-home.html?lang=en)

## Herstellen einer Verbindung zum SFTP-Server (Client oder API)

Für die Verbindung mit den SFTP-Servern ist Folgendes erforderlich:

* Die IP-Adresse, von der Sie eine Verbindung zum SFTP-Server herstellen, muss auf der [!UICONTROL Zulassungsliste] stehen.
* Paar aus privatem/öffentlichem Schlüssel, das bei Adobe Campaign registriert werden muss
* Wenn Sie eine direkte Verbindung zum SFTP-Server herstellen möchten, benötigen Sie SFTP-Client-Software

### Hilfreiche Dokumentation {#helpful-docs}

* [Anmeldung bei Ihrem SFTP-Server](https://experienceleague.adobe.com/docs/control-panel/using/control-panel-home.html?lang=en)
