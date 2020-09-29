---
title: Transition - Wechseln zwischen E-Mail-Plattformen
description: 'Beim Verschieben von E-Mail-Dienstleistern (ESPs) ist es nicht möglich, auch Ihre bestehenden, etablierten IP-Adressen Transition. Es ist wichtig, dass Sie bewährte Verfahren befolgen, um einen positiven Ruf zu entwickeln, wenn Sie von Neuem beginnen. Da die neuen IP-Adressen, die Sie verwenden werden, noch nicht bekannt sind, können ISPs der E-Mail, die von ihnen stammt, nicht voll vertrauen und müssen vorsichtig sein, was sie für die Zustellung an ihre Kunden zulassen. '
feature: null
topics: Deliverability
kt: null
doc-type: article
activity: understand
team: TM
translation-type: tm+mt
source-git-commit: f4dbccc1fea3db4dbddec0d4329b359993b62d20
workflow-type: tm+mt
source-wordcount: '1686'
ht-degree: 0%

---


# Transition - Wechseln zwischen E-Mail-Plattformen

Beim Verschieben von E-Mail-Dienstleistern (ESPs) ist es nicht möglich, auch Ihre bestehenden, etablierten IP-Adressen Transition. Es ist wichtig, dass Sie bewährte Verfahren befolgen, um einen positiven Ruf zu entwickeln, wenn Sie von Neuem beginnen. Da die neuen IP-Adressen, die Sie verwenden werden, noch nicht bekannt sind, können ISPs der E-Mail, die von ihnen stammt, nicht voll vertrauen und müssen vorsichtig sein, was sie für die Zustellung an ihre Kunden zulassen.

Denk darüber nach, was du tust, wenn du jemanden neu kennenlernst. Normalerweise müssen Sie Vertrauen aufbauen, anstatt ihnen sofort zu vertrauen. Denken Sie nicht, dass Ihre Marke automatisch bei diesem Vertrauen helfen wird, denn Spammer benutzen Ihren Namen, um schlechte Dinge zu tun. ISPs müssen Ihre Versandmethoden neu bewerten, da die E-Mail-Zustellbarkeit eine besonders aufschlussreiche Aktion darstellt.

Ein positiver Ruf ist ein Prozess. Aber sobald sie eingerichtet ist, haben kleine negative Indikatoren weniger Einfluss auf Sie und Ihren E-Mail-Versand.

![Transition](assets/transition-process.png)

Die Wartezeit zum Aufwärmen Ihrer IP-Adressen und Domänen kann unterschiedlich sein, aber für typische Absender ist es üblich, bis zu acht Wochen lang einen Ruf bei den meisten Tier-1-ISPs zu etablieren ([!DNL Gmail], [!DNL Microsoft], [!DNL Verizon]/[!DNL Yahoo]/[!DNL AOL]usw.).
In den nächsten Abschnitten werden wir einige Schlüsselbereiche untersuchen, auf die wir uns konzentrieren können, um richtig an Bord zu gehen.

## Infrastruktur

Erfolgreiche Lieferbarkeit hängt von einer soliden Grundlage ab. Die E-Mail-Infrastruktur ist ein Kernelement. Eine ordnungsgemäß konstruierte E-Mail-Infrastruktur umfasst mehrere Komponenten — d. h. Domäne(n) und IP-Adresse(n). Diese Komponenten sind wie die Maschinen hinter den E-Mails, die Sie senden, und sie sind oft der Anker des guten Rufs. Berater für Lieferbarkeit sorgen dafür, dass diese Elemente während der Implementierung korrekt eingerichtet werden. Aufgrund des Reputationsfaktors ist es jedoch wichtig, dass Sie über dieses Grundverständnis verfügen.

### Domäneneinrichtung und -strategie

Die Zeiten haben sich geändert, und einige ISPs (wie [!DNL Gmail] und [!DNL Yahoo]) beinhalten nun den Ruf der Domäne als zusätzlichen Punkt, wenn es darum geht, einem Absender einen Ruf der E-Mail zuzuordnen. Der Ruf Ihrer Domäne basiert auf Ihrer sendenden Domäne und nicht auf Ihrer IP-Adresse. Das bedeutet, dass Ihre Marke bei der Entscheidung über das ISP-Filtern Vorrang hat.

Ein Teil des Einstiegsprozesses für neue Absender im Adobe Campaign umfasst die Einrichtung Ihrer sendenden Domänen und die Sicherstellung der ordnungsgemäßen Einrichtung Ihrer Infrastruktur. Sie sollten mit einem Experten zusammenarbeiten, welche Domänen Sie langfristig verwenden möchten. Im Folgenden finden Sie einige Tipps, die eine gute Domänenstrategie gestalten:

* Achten Sie bei der gewählten Domäne darauf, dass die Marke so klar und reflektiert wird, dass die Benutzer die E-Mail nicht fälschlicherweise als Spam identifizieren. Einige Beispiele sind [!DNL newsletter.foo.com], [!DNL receipts.foo.com]usw.
* Sie sollten Ihre Mutterdomäne oder Unternehmensdomäne nicht verwenden, da dies den Versand von E-Mails Ihrer Organisation an ISPs beeinträchtigen könnte.
* Erwägen Sie, eine Subdomäne Ihrer übergeordneten Domäne zu verwenden, um Ihre sendende Domäne zu legitimieren.
* Trennen Sie Ihre Subdomänen für transaktions- und Marketingnachrichten-Kategorien. Dies wird Ihnen dabei helfen, den E-Mail-Traffic zuverlässiger zu gestalten, da ISPs nach dieser Versandmethode suchen, die eine bekannte Best Practice für E-Mails ist und dringend empfohlen wird.

### IP-Strategie

Es ist wichtig, eine gut strukturierte IP-Strategie zu entwickeln, um einen positiven Ruf zu schaffen. Die Anzahl der IPs und des Setups hängt von Ihrem Geschäftsmodell und Ihren Marketingzielen ab. Arbeiten Sie mit einem Experten zusammen, um eine klare Strategie zum Beginn zu entwickeln. Betrachten Sie die folgenden Punkte, die wichtig sind:

* Zu viele IPs können Reputationsprobleme auslösen, da es sich um eine gängige Taktik von Spammer zu Schneeschuhen handelt. Diese Taktik wird von Spammer verwendet, bei der der Traffic über viele IPs verteilt wird, um den Versand von Spam-Mails zu maximieren. Auch wenn Sie kein Spammer sind, könnten Sie wie ein Spammer aussehen, wenn Sie zu viele IPs verwenden, insbesondere wenn diese IPs zuvor keinen Traffic hatten.
* Zu wenige IPs können Durchsatzprobleme verursachen und möglicherweise Reputationsprobleme auslösen. Der Durchsatz variiert je nach ISP. Wie viel und wie schnell ein ISP akzeptieren will, hängt in der Regel von seiner Infrastruktur und der Entsendung von Reputationsschwellen ab.
* Die Trennung von Traffic für Messaging-Typen ist der Schlüssel. Es ist wichtig, dass Sie Marketing- und Transaktionsnachrichten in einem separaten IP-Pool abwickeln.
* Abhängig von Ihrer Mail-Strategie kann es ratsam sein, verschiedene Produkte oder Marketingströme auf verschiedene IP-Pools zu trennen, wenn Ihr Ruf deutlich anders ist. Einige Marketingexperten segmentieren auch nach Region. Die Trennung der IP-Adresse für Traffic mit einem geringeren Ruf wird das Reputationsproblem nicht beheben, aber es werden Probleme mit Ihren E-Mail-Versänden mit &quot;gutem Ruf&quot;vermieden. Schließlich wollen Sie Ihre gute Audience nicht für eine riskantere opfern.

### Feedback-Schleifen

Hinter den Kulissen verarbeitet Adobe Campaign Daten zu Absprüngen, Beschwerden, Abmeldungen und mehr. Die Einrichtung dieser Feedback-Schleifen ist ein wichtiger Aspekt für die Lieferbarkeit. Beschwerden können einen Ruf beschädigen. Daher sollten Sie E-Mail-Adressen, die Beschwerden registrieren, aus der Audience Ihrer Zielgruppe entfernen. Beachten Sie, dass diese Daten [!DNL Gmail] nicht zurückgegeben werden. Header zum Abmelden von Listen und Interaktionsfilterung sind besonders wichtig für [!DNL Gmail] Abonnenten, die jetzt die Mehrzahl der Abonnentendatenbanken bilden.

### Authentifizierung

Die Authentifizierung ist der Prozess, mit dem ISPs die Identität eines Absenders überprüfen. Die beiden am häufigsten verwendeten Authentifizierungsprotokolle sind [!DNL Sender Policy Framework (SPF)] und [!DNL DomainKeys Identified Mail] (DKIM). Diese sind für den Endbenutzer nicht sichtbar, helfen ISPs jedoch, E-Mails von bestätigten Absendern zu filtern. [!DNL Domain-based Message Authentication Reporting and Conformance] (DMARC) gewinnt an Popularität, obwohl seine Richtlinien noch nicht von allen ISPs in ihre Reputationssysteme integriert sind.

#### **SPF**

[!DNL Sender Policy Framework (SPF)] ist eine Authentifizierungsmethode, mit der der Inhaber einer Domäne angeben kann, welche E-Mail-Server er verwendet, um E-Mails von dieser Domäne zu senden.

#### **DKIM**

[!DNL Domain Keys Identified Mail (DKIM)] ist eine Authentifizierungsmethode, mit der gefälschte Absenderadressen erkannt werden (häufig als [!DNL spoofing]). Wenn DKIM aktiviert ist, kann der Empfänger bestätigen, ob der Absender berechtigt ist, E-Mails von dieser Domäne zu senden.

#### **DMARC**

[!DNL Domain-based Message Authentication, Reporting and Conformance (DMARC)] ist eine Authentifizierungsmethode, die Domäneninhabern die Möglichkeit gibt, ihre Domäne vor unbefugter Verwendung zu schützen. DMARC verwendet SPF oder DKIM oder beides, um einem Domäneninhaber zu ermöglichen, zu steuern, was mit E-Mails passiert, bei denen die Authentifizierung fehlschlägt: geliefert, unter Quarantäne gestellt oder abgelehnt.

## Targeting-Kriterien

Beim Versand von neuem Traffic sollten Sie nur die Zielgruppe Ihrer am meisten engagierten Benutzer während der ersten Phase der IP-Erwärmung vornehmen. Dies hilft, einen positiven Ruf von get-go zu etablieren, um effektiv Vertrauen aufzubauen, bevor Sie Ihre weniger engagierten Audiencen einführen. Hier ist eine grundlegende Formel für Interaktionen:

![Formel für das Management](assets/formula-for-enagement.png)

In der Regel basiert eine Interaktionsrate auf einem bestimmten Zeitraum. Diese Metrik kann drastisch variieren, je nachdem, ob die Formel auf einer Gesamtebene oder für bestimmte Mailing-Typen oder Kampagnen angewendet wird. Die spezifischen Targeting-Kriterien müssen durch die Zusammenarbeit mit Ihrem Adobe Campaign-Bereitstellungsberater bereitgestellt werden, da jeder Absender und ISP variiert und in der Regel einen angepassten Plan benötigt.

## ISP-spezifische Aspekte bei der IP-Erwärmung

ISPs haben unterschiedliche Regeln und verschiedene Arten, ihren Traffic zu betrachten. Zum Beispiel [!DNL Gmail] ist einer der ausgefeiltesten ISPs, weil sie sich neben allen anderen Reputationsmaßnahmen sehr streng mit Interaktion (Öffnen und Klicks) auseinander setzen. Dies erfordert einen angepassten Plan, bei dem nur die am häufigsten verwendeten Benutzer zu Beginn der Anwendung Zielgruppe werden. Andere ISPs erfordern möglicherweise dasselbe. Arbeiten Sie mit Ihrem Adobe Campaign-Bereitstellungsberater an einem bestimmten Plan.

## Volumen

Die Anzahl der Mails, die Sie senden, ist entscheidend, um einen positiven Ruf zu schaffen. Legen Sie sich in einen ISPs Schuhe — Wenn Sie einen Beginn sehen, der eine Tonne Traffic von jemandem sieht, den Sie nicht kennen, wäre das alarmierend. Die sofortige Versendung großer Mengen von E-Mails ist riskant und wird mit Sicherheit zu Reputationsproblemen führen, die oft schwer zu lösen sind. Es kann frustrierend, zeitaufwendig und kostspielig sein, sich selbst aus schlechter Reputation zu befreien und Probleme zu krümmen und zu blockieren, die sich daraus ergeben, dass sie zu früh gesendet werden.

Die Mengenschwellenwerte variieren je nach ISP und können auch je nach Ihren durchschnittlichen Einsatzmetriken variieren. Einige Absender benötigen eine sehr niedrige und langsame Mengenrampe, während andere eine höhere Lautstärke ermöglichen. Wir empfehlen die Zusammenarbeit mit einem Experten, wie einem Adobe Campaign-Bereitstellungsberater, um einen maßgeschneiderten Volumenplan zu entwickeln.

Hier finden Sie eine Liste mit Hinweisen und Tipps zur reibungslosen Transition:

* **Berechtigungen** sind die Grundlage für jedes erfolgreiche E-Mail-Programm.
* **Geringer und langsamer Beginn** mit niedrigem Versandvolumen und steigern sich dann, wenn Sie Ihren Ruf als Absender feststellen.
* Eine **Tandem-Mailingstrategie** ermöglicht es Ihnen, das Volumen bei der Kampagne zu erhöhen, während Sie mit Ihrem aktuellen ESP abbrechen, ohne dass Ihr E-Mail-Kalender gestört wird.
* **Interaktion ist wichtig** - Beginn mit den Abonnenten, die Ihre E-Mails regelmäßig öffnen und anklicken.
* **Befolgen Sie den Plan** — Unsere Empfehlungen haben Hunderten von Kampagnen geholfen, ihre E-Mail-Programme erfolgreich zu erhöhen.
* **Überwachen Sie Ihr E-Mail-Konto** für die Antwort. Es ist ein schlechtes Erlebnis, das Ihr Kunde verwenden [!DNL nore-ply@xyz.com] oder nicht beantworten kann.
* Inaktive Adressen können sich negativ auf die Zustellbarkeit auswirken. **Reaktivieren und reaktivieren Sie die Berechtigung** auf Ihrer aktuellen Plattform, nicht auf Ihren neuen IPs.
* **Domänen** : Verwenden Sie eine sendende Domäne, die eine Subdomäne der eigentlichen Domäne Ihrer Firma ist. Wenn beispielsweise Ihre Firma Domäne ist [!DNL xyz.com], bietet [!DNL email.xyz.com] sie mehr Glaubwürdigkeit als [!DNL xyzemail.com]
* **Transparenz** - Registrierungsdetails für Ihre E-Mail-Domäne sollten öffentlich verfügbar sein und nicht privat sein.

In vielen Fällen folgt transaktionale Postsendungen nicht dem traditionellen Ansatz zur Förderung der Erwärmung. Es ist offensichtlich schwierig, die Lautstärke in transaktionalen E-Mails zu kontrollieren, da es normalerweise eine Benutzerinteraktion erfordert, um den E-Mail-Touch auszulösen. In einigen Fällen kann die transaktionale Post einfach ohne formalen Plan übergeben werden. In anderen Fällen ist es möglicherweise besser, jeden Nachrichtentyp im Zeitverlauf Transition, um die Lautstärke langsam zu erhöhen. Sie können beispielsweise wie folgt Transitionen durchführen:

1. Kaufbestätigungen - hoher Einsatz im Allgemeinen
2. Warenkorbabbruch - mittlerer Einsatz im Allgemeinen
3. Begrüßungs-E-Mails - hohe Interaktion, können aber je nach Erfassungsmethoden Ihrer Liste falsche Adressen enthalten
4. Win-back-E-Mails - geringere Interaktion im Allgemeinen

## Zusätzliche Ressourcen

* [Einrichten einer neuen Plattform](https://docs.adobe.com/content/help/en/campaign-standard/using/testing-and-sending/managing-deliverability/starting-new-platform.html)
