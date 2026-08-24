# Bewerbungsagent – n8n-Workflow-Showcase

Dieses Repository zeigt drei ausgewählte n8n-Workflows eines modularen Bewerbungsagenten. Im Mittelpunkt stehen die bereinigten Workflow-Definitionen im Ordner [`workflows`](workflows/).

- **[M3KI – KI-Recherche](workflows/M3KI-KI-Recherche-GitHub.json):** Ergänzt die Recherche ausgewählter Kandidaten durch eine KI-gestützte Prüfung und führt die Ergebnisse in ein einheitliches Format zurück.
- **[M6 – Freigabe](workflows/M6-Freigabe-GitHub.json):** Bildet den Human-in-the-loop-Schritt ab, in dem vorbereitete Bewerbungen und Vorschauunterlagen vor dem Versand geprüft und freigegeben werden.
- **[M7 – Versand](workflows/M7-Versand-Gmail-GitHub.json):** Verarbeitet ausschließlich freigegebene Bewerbungen, prüft Versandvoraussetzungen und dokumentiert Sendeversuche sowie Ergebnisse als Schutz vor unkontrolliertem oder doppeltem Versand.

Für diese öffentliche Version wurden Credentials, interne IDs, E-Mail-Adressen, lokale Pfade und weitere sensible oder produktive Angaben entfernt beziehungsweise anonymisiert. Alle Workflows sind deaktiviert und benötigen vor einer eigenen Nutzung eine individuelle Konfiguration.
