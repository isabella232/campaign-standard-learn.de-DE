---
title: Fehlerbehebung beim Control Panel
description: Im Control Panel können Sie Ihre SFTP-Speicherung nach Instanz und Zulassungslisten-IP-Adressen überwachen und verwalten.
feature: Control Panel
kt: 2938
doc-type: article
activity: use
team: PM
recommendations: noDisplay
exl-id: f546f791-a69b-4586-abfa-3e626b8feb17
source-git-commit: 57dbf456625d22cd2e4526d92e5a8c20a048d339
workflow-type: tm+mt
source-wordcount: '348'
ht-degree: 100%

---

# Fehlerbehebung beim [!UICONTROL Control Panel]

Erfahren Sie, wie Sie Probleme bei der Verwendung des Control Panels beheben können.

## Anmelden und Homepage

Probleme bei der Anmeldung und Homepage.

### Problem: Anmeldung bei Adobe Experience Cloud nicht möglich

**Vorgehensweise:**
Der Benutzer muss seine [!DNL IMS Org ID] (xxx) finden. Der Administrator muss den Benutzer für jede Instanz, die er verwalten möchte, dem [!UICONTROL Produktprofil] [!DNL “Campaign-xxx-Admins”] hinzufügen. Wenn der Benutzer ein Administrator aller Instanzen ist, muss er sich dennoch selbst als *[!UICONTROL Benutzer]* hinzufügen.

### Symptom: Links auf der [!UICONTROL Adobe Experience Cloud-Startseite] zum Zugriff auf das [!UICONTROL Control Panel] werden einem Benutzer nicht angezeigt.

**Ursache:**
Benutzer sehen die Links erst, wenn sie als Benutzer zum [!UICONTROL Produktprofil] `Campaign-xxx-Administrators/Admin` hinzugefügt werden.

**Vorgehensweise:**
Der Administrator muss den Benutzer für jede Instanz, die er verwalten möchte, dem [!UICONTROL Produktprofil] *[!DNL Campaign-xxx-Admins]* hinzufügen. Wenn der Benutzer ein Administrator aller Instanzen ist, muss er sich dennoch selbst als *[!UICONTROL Benutzer]* hinzufügen.

### Problem: Eine Instanz wird im [!UICONTROL Control Panel] nicht aufgeführt.

**Ursache:****
Der Benutzer muss wahrscheinlich für die fehlende Instanz dem Produktprofil `Campaign-xxx-Administrators/Admin` als Benutzer hinzugefügt werden.

**Vorgehensweise:**
Der Administrator muss den Benutzer für jede Instanz, die er verwalten möchte, dem Produktprofil `Campaign-xxx-Admins` hinzufügen. Wenn der Benutzer ein Administrator aller Instanzen ist, muss er sich dennoch selbst als *[!UICONTROL Benutzer]* hinzufügen.

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
* Schlüsselpaar aus privatem/öffentlichem Schlüssel, das bei Adobe Campaign registriert werden muss
* Wenn Sie eine direkte Verbindung zum SFTP-Server herstellen möchten, benötigen Sie auch SFTP-Client-Software.

### Hilfreiche Dokumentation {#helpful-docs}

* [Anmeldung bei Ihrem SFTP-Server](https://experienceleague.adobe.com/docs/control-panel/using/control-panel-home.html?lang=en)
