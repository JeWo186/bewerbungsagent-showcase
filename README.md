# Recherche- und Outreach-Pipeline – n8n-Workflow-Beispiele

Dieses Repository zeigt drei bereinigte n8n-Workflows aus meinem größten Praxisprojekt: einer Pipeline, die passende Unternehmen findet, recherchiert, einordnet und eine persönliche Ansprache vorbereitet. Gebaut habe ich sie für meinen eigenen Berufseinstieg – die Logik entspricht Leadgenerierung oder Outreach-Kampagnen im Marketing.

## Die Workflows

- **[M2 – Qualifizierung](workflows/M2-Qualifizierung.json):** Prüft jedes gefundene Unternehmen nach festen Kriterien mit einem Sprachmodell, deckelt die Bewertung bei klaren Ausschlussgründen (zum Beispiel kein Agenturgeschäft oder Präsenzpflicht) und schreibt das Ergebnis nachvollziehbar zurück. Fehler werden separat festgehalten, statt den Lauf abzubrechen.
- **[M6 – Berater](workflows/M6-Berater.json):** Fasst Recherche und Bewertungen zu einer Einschätzung zusammen. Belegte Fakten und Ableitungen werden strikt getrennt; Fachbegriffe und Jobtitel werden in einfachen Worten erklärt. Eine Längenprüfung korrigiert zu lange Antworten automatisch.
- **[M7 – Versand](workflows/M7-Versand-Gmail.json):** Versendet ausschließlich freigegebene Nachrichten, prüft vorher Empfänger, Anrede, Platzhalter und Anhang und protokolliert jeden Versuch – als Schutz vor unkontrolliertem oder doppeltem Versand. In dieser Fassung ist der Echtversand ausgeschaltet.

## Grundsätze

- **Der Mensch entscheidet:** Nichts geht ohne manuelle Freigabe hinaus.
- **KI nur, wo sie hilft:** Eindeutige Aufgaben wie Dubletten, Statuswechsel und Versandprüfungen laufen regelbasiert.
- **Kosten im Blick:** Bei der Überarbeitung im November 2026 habe ich die Modelle neu gewählt und rund die Hälfte der Abläufe stillgelegt. Der Modellwechsel senkt die Kosten pro KI-Aufruf um rund 85–90 %.

## Hinweise

Für diese öffentliche Fassung wurden Zugangsdaten, Tabellen-IDs, E-Mail-Adressen, lokale Pfade und weitere interne Angaben entfernt oder durch Platzhalter ersetzt. Die Workflows sind deaktiviert und brauchen vor einer eigenen Nutzung eine eigene Konfiguration (Google Sheets, OpenAI, Gmail).

Portfolio und klickbare Demo: [jerome-wolfarth-portfolio.vercel.app](https://jerome-wolfarth-portfolio.vercel.app)
