---
copyright:
  years: 1994, 2017
lastupdated: "2017-12-01"
---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Häufig gestellte Fragen (FAQs)

## Wie kann ich die Besitzinformationen für meine IPs aktualisieren? (SWIP)

Über Shared WhoIs Project (SWIP) von ARIN (American Registry for Internet Numbers) können Sie Besitzinformationen für IP-Adressen zu Ihrem Konto bereitstellen. Dieses Tool arbeitet mit dem {{site.data.keyword.BluSoftlayer_notm}}-System 'Reverse WHOIS'. Es empfiehlt sich, beide Tools zu verwenden, da nicht alle WHOIS-Tools das System 'Reverse WHOIS' zum Suchen nach dem Eigner eines Blocks von IPs (eines Teilnetzes) verwenden. Beachten Sie, dass nur Teilnetze mit 8 oder mehr IP-Adressen (Teilnetze mit einer Teilnetzmaske kleiner als 30) das SWIP-System verwenden können.

Sie können SWIP für ein Teilnetz ausführen, indem Sie im Kundenportal die Optionen für **Öffentliches Netz -> SWIP** und anschließend die Option zum **Ausführen von Swip für Teilnetz** neben dem Zielbereich auswählen.

Auf der SWIP-Seite können Sie die folgenden Tasks ausführen:

 * **Swip für Teilnetz ausführen:** Eine Anforderung an ARIN zum Aktualisieren Ihrer IP-Informationen mit Ihren Reverse WHOIS-Daten senden.<br/>
 * **Teilnetz aktualisieren:** ARIN aktualisieren, wenn Sie Ihre Reverse WHOIS-Daten ändern.<br/>
 * **Teilnetz löschen:** Ihre Informationen aus ARIN entfernen und sie durch Standardinformationen von IBM Cloud ersetzen.

Sie können den Status einer SWIP-Anforderung auch in der Statusspalte auf der SWIP-Seite ersehen:

 * **Kein SWIP ausgeführt:** Die SWIP-Anforderung für dieses Teilnetz wurde noch nicht abgesetzt. In den WHOIS-Daten wird {{site.data.keyword.BluSoftlayer_notm}} als Eigner des Teilnetzes aufgelistet.
 * **Anforderung wartet auf ARIN...:** Es wurde eine Anforderung gesendet, auf eine Antwort wird jedoch noch gewartet. Antworten können bis zu drei Tage dauern.
 * **Warten auf Löschen in ARIN...:** Wie bei einer SWIP-Anforderung kann das Löschen der WHOIS-Informationen bis zu 3 Tage dauern.
 * **Manuelle Verarbeitung durch IBM läuft...:** In manchen Fällen kann eine SWIP-Anforderung nicht automatisch verarbeitet werden. In diesem Fall wird der Fehler an {{site.data.keyword.BluSoftlayer_notm}} berichtet und der Fehler in der Transaktion muss manuell behoben werden.
 
