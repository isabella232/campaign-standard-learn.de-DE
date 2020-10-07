---
title: Andere Metriken, die für die Lieferbarkeit wichtig sind
description: Eine der besten Methoden, um ein Problem mit dem Ruf des Senders zu identifizieren, sind die Metriken. Sehen wir uns einige wichtige Leistungsmetriken an, die überwacht werden sollen, und wie diese zur Identifizierung eines Reputationsproblems verwendet werden können.
feature: null
topics: Deliverability
kt: 5256
doc-type: article
activity: understand
team: TM
translation-type: tm+mt
source-git-commit: 6e4824185b84715d514bf21aace9e57c602e970d
workflow-type: tm+mt
source-wordcount: '1367'
ht-degree: 1%

---


# Andere Metriken, die für die Lieferbarkeit wichtig sind

Eine der besten Methoden, um ein Problem mit dem Ruf des Senders zu identifizieren, sind die Metriken. Sehen wir uns einige wichtige Leistungsmetriken an, die überwacht werden sollen, und wie diese zur Identifizierung eines Reputationsproblems verwendet werden können.

## Bounces

Absprünge sind das Ergebnis eines Versand-Versuchs und -Fehlers, bei dem der ISP Rückmeldungen zur Fehlerbehebung angibt. Die Absprungbehandlung ist ein wichtiger Bestandteil der Hygiene in der Liste. Nachdem eine bestimmte E-Mail mehrmals hintereinander abgeschnitten wurde, markiert dieser Prozess sie zur Unterdrückung. Die Anzahl und Art der Absprünge, die zur Auslösung der Unterdrückung erforderlich sind, variieren von System zu System. Dieser Prozess verhindert, dass Systeme weiterhin ungültige E-Mail-Adressen senden. Absprünge sind eine der Schlüsseldaten, die ISPs zur Ermittlung des Rufs der IP verwenden. Diese Metrik im Auge zu behalten, ist sehr wichtig. &quot;Ausgeliefert&quot;im Vergleich zu &quot;Abgebrochen&quot;ist wahrscheinlich die häufigste Methode zur Messung des Versands von Marketingmeldungen: Je höher der gelieferte Prozentsatz ist, desto besser. Wir werden zwei verschiedene Arten von Absprüngen untersuchen.

## Hardbounces

Hard Bounces sind dauerhafte Ausfälle, die erzeugt werden, nachdem ein ISP feststellt, dass ein Mailingversuch an eine Abonnentenadresse nicht auslieferbar ist. Innerhalb des Adobe Campaigns werden feste Absprünge, die als nicht auslieferbar eingestuft werden, der Quarantäne hinzugefügt, was bedeutet, dass sie nicht erneut versucht werden. Es gibt Fälle, in denen ein harter Absprung ignoriert wird, wenn die Ursache des Fehlers unbekannt ist. Hier sind einige häufige Beispiele für harte Absprünge:

* Adresse nicht vorhanden
* Konto deaktiviert
* Ungültige Syntax
* Ungültige Domäne

## Softbounces

Weiche Absprünge sind vorübergehende Ausfälle, die von ISPs erzeugt werden, wenn sie Probleme bei der Zustellung von E-Mails haben. Bei Soft-Fehlern wird der Versuch wiederholt (je nach Verwendung von benutzerdefinierten oder vordefinierten Adobe Campaign-Versand-Einstellungen), um einen erfolgreichen Versand zu versuchen. Adressen, die kontinuierlich weichen Absprung aufweisen, werden erst dann der Quarantäne hinzugefügt, wenn die maximale Anzahl von weiteren Zustellversuchen versucht wurde (die wiederum je nach Einstellungen variieren). Zu den häufigen Ursachen für weiche Absprünge zählen die folgenden:

* Postfach voll
* Abrufen des E-Mail-Servers
* Probleme mit dem Ruf des Absenders

![Absprungarten](assets/bounce-types.png)

>[!NOTE]
>
>Absprünge sind ein wichtiger Indikator für ein Reputationsproblem, da sie eine schlechte Datenquelle (Absprung) oder ein Reputationsproblem mit einem ISP (Absprung) hervorheben können.
>
>Weiche Absprünge treten oft beim Senden von E-Mails auf und sollten während der Wiederholung der Verarbeitung gelöst werden können, bevor sie als echte Bereitstellungsprobleme erkannt werden. Wenn Ihre Soft-Absprungrate bei einem einzelnen ISP über 30 Prozent liegt und nicht innerhalb von 24 Stunden aufgelöst wird, ist es eine gute Idee, bei Ihrem Adobe Campaign-Bereitstellungsberater Bedenken zu äußern.

## Beschwerden

Beschwerden werden registriert, wenn ein Benutzer anzeigt, dass eine E-Mail unerwünscht oder unerwartet ist. Diese Abonnentenaktion wird in der Regel entweder über den E-Mail-Client des Abonnenten protokolliert, wenn er auf die Spam-Schaltfläche klickt, oder über ein Spam-Berichte-System eines Drittanbieters.

### ISP-Beschwerde

Die meisten Tier-1- und einige Tier-2-ISPs bieten ihren Benutzern eine Spam-Berichte-Methode, da Abmelde- und Abmeldeprozesse früher böswillig zur Validierung einer E-Mail-Adresse verwendet wurden. Adobe Campaign erhält diese Beschwerden über ISP FBLs. Dies wird während des Setups für alle ISPs festgelegt, die FBLs bereitstellen und es Adobe Campaign ermöglichen, automatisch E-Mail-Adressen hinzuzufügen, die zur Unterdrückung an die Quarantäne-Tabelle gemeldet wurden. Spitzen bei ISP-Beschwerden können ein Indikator für schlechte Qualität der Liste, weniger als optimale Erfassungsmethoden für Listen oder eine schwache Interaktionsstrategie sein. Sie werden häufig auch dann vermerkt, wenn Inhalte nicht relevant sind.

### Beschwerden von Drittanbietern

Es gibt mehrere Anti-Spam-Gruppen, die Spam-Berichte auf einer breiteren Ebene ermöglichen. Die von diesen Drittanbietern verwendeten Beschwerdemetriken werden verwendet, um E-Mail-Inhalte zur Identifizierung von Spam-E-Mails zu taggen. Dieser Prozess wird auch als Fingerabdruck bezeichnet. Benutzer dieser Drittanbieter-Beschwerdeverfahren sind in der Regel über E-Mails auf dem Laufenden, sodass sie eine größere Wirkung haben können als andere Beschwerden, wenn sie nicht beantwortet werden.

>[!NOTE]
>
>ISPs sammeln Beschwerden und verwenden sie, um den allgemeinen Ruf eines Absenders zu ermitteln. Alle Beschwerden sollten unterdrückt und nicht mehr so schnell wie möglich und gemäß den örtlichen Gesetzen und Vorschriften kontaktiert werden.

## Spam-Fallen

Eine Spam-Falle ist eine Adresse, mit der eine nicht autorisierte oder nicht angeforderte E-Mail identifiziert werden kann. Spam-Fallen bestehen, um E-Mails betrügerischer Absender oder Absender zu identifizieren, die nicht den Best Practices für E-Mails folgen. Die Spam-Trap-E-Mail-Adresse ist in der Regel nicht öffentlich bekannt und lässt sich kaum identifizieren. Die Bereitstellung von E-Mails an Spam-Fallen kann Ihren Ruf in unterschiedlichem Ausmaß beeinträchtigen, je nach Trap- und ISP-Typ. Erfahren Sie mehr über die verschiedenen Arten von Spam-Traps in den folgenden Abschnitten.

### Recycling

Wiederverwertete Spam-Fallen sind Adressen, die einst gültig waren, aber nicht mehr verwendet werden. Eine wichtige Möglichkeit, Listen so sauber wie möglich zu halten, besteht darin, regelmäßig E-Mails an Ihre gesamte Liste zu senden und abgeschnittene E-Mails entsprechend zu unterdrücken. Dadurch können aufgegebene E-Mail-Adressen isoliert und von einer weiteren Verwendung ausgeschlossen werden.

In einigen Fällen kann eine Adresse innerhalb von 30 Tagen recycelt werden. Regelmäßige Entsendung ist ein entscheidender Aspekt guter Hygiene bei der Liste, und die regelmäßige Unterdrückung inaktiver Nutzer ist ein entscheidender Aspekt. Kampagnen zur Rückbindung sind in der Regel Bestandteil komplexer E-Mail-Marketing-Programm. Dieser Stil ermöglicht es dem Absender, Kampagnen zurückzugewinnen, die andernfalls nicht mehr per E-Mail versandt würden.

### Typo

Eine Tippfehler-Spam-Falle ist eine Adresse, die eine Rechtschreibfehler oder Fehlbildungen enthält. Dies tritt häufig bei bekannten Rechtschreibfehlern in wichtigen Domänen wie [!DNL Gmail] (z. B.: [!DNL gmail] ist ein häufiger Tippfehler). ISPs und andere Betreiber von Listen registrieren bekannte schlechte Domänen, die als Spam-Falle verwendet werden, um Spammer zu identifizieren und die Absendergesundheit zu messen. Die beste Möglichkeit, Tippfehler in Spam-Fallen zu verhindern, ist die Verwendung eines Anmeldeprozesses für Dubletten zur Liste.

### Pristin

Eine ungewöhnliche Spam-Falle ist eine Adresse, die keinen Endbenutzer hat und noch nie einen Endbenutzer hatte. Es handelt sich dabei um eine Adresse, die ausschließlich zur Identifizierung von Spam-E-Mails erstellt wurde. Dies ist der wirkungsvollste Spam-Trap-Typ, da es praktisch unmöglich ist, ihn zu identifizieren, und es erfordert erhebliche Anstrengungen, um Ihre Liste zu reinigen. Die meisten schwarzen Listen verwenden ungewöhnliche Spam-Fallen für nicht seriöse Absender von Listen. Die einzige Möglichkeit, ungewöhnliche Spam-Fallen daran zu hindern, Ihre umfassendere Marketing-E-Mail-Liste zu infizieren, besteht darin, einen Dubletten-Anmeldeprozess für die Erfassung von Listen zu verwenden.

## Bulking

Bulking ist der Versand von Mails in den Spam- oder Junk-Ordner eines ISP. Sie lässt sich identifizieren, wenn eine nicht normale offene Rate (und manchmal auch eine Klickrate) mit einer hohen Bereitstellungsrate gepaart wird. Die Ursachen für das Aufzählen von E-Mails variieren je nach ISP. Im Allgemeinen ist jedoch eine erneute Überprüfung erforderlich, wenn Meldungen im Massenordner abgelegt werden, die den Ruf (z. B. die Hygiene der Liste) beeinflussen. Es ist ein Zeichen dafür, dass der Ruf nachlässt, was ein Problem ist, das sofort korrigiert werden muss, bevor es weitere Kampagnen betrifft. Arbeiten Sie mit Ihrem Adobe Campaign-Berater zusammen, um Probleme zu beheben, die je nach Situation auftreten.

## Blockieren

Ein Block tritt auf, wenn Spam-Indikatoren proprietäre ISP-Schwellenwerte erreichen und der ISP beginnt, E-Mails (erkennbar durch gestoppte Mailingversuche) von einem Absender zu blockieren. Es gibt verschiedene Arten von Blöcken. Im Allgemeinen treten Blöcke spezifisch für eine IP-Adresse auf, können aber auch auf der Ebene der sendenden Domäne oder Entität auftreten. Für die Lösung eines Adobe Campaigns ist spezifisches Fachwissen erforderlich. Wenden Sie sich daher an Ihren Berater für die Zustellbarkeit.

## Blacklisting

Eine schwarze Liste tritt auf, wenn ein Blacklist-Manager eines Drittanbieters ein mit einem Absender verknüpftes Verhalten registriert. Die Ursache einer schwarzen Liste wird manchmal von der Partei veröffentlicht, die sie auf der schwarzen Liste hat. Eine Auflistung basiert in der Regel auf IP-Adressen, kann aber in schwereren Fällen nach IP-Bereich oder sogar nach einer sendenden Domäne erfolgen. Die Lösung einer schwarzen Liste sollte die Unterstützung Ihres Adobe Campaign-Bereitstellungsberaters beinhalten, um weitere Auflistungen vollständig zu lösen und zu verhindern. Einige Auflistungen sind extrem schwer und können langfristige Reputationsprobleme hervorrufen, die schwer zu lösen sind. Das Ergebnis einer schwarzen Liste variiert je nach Blacklist, hat aber das Potenzial, den Versand aller E-Mails zu beeinflussen.

## Zusätzliche Ressourcen

* [Typen und Ursachen für fehlgeschlagene Sendungen](https://docs.adobe.com/content/help/en/campaign-standard/using/testing-and-sending/monitoring-messages/understanding-delivery-failures.html#delivery-failure-types-and-reasons)
