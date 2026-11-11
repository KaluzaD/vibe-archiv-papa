---
name: homeassistant-papa
display_name: "🏠 Home Assistant Papa"
description: Daniels Projekt „Home Assistant Papa" – Papas eigene HA-Instanz auf dem freigewordenen HA Green. Jungfräuliche Einrichtung, keine Wiederherstellung von Daniels Backup, spätere Mitverwaltung über Nuntius/HA-Fehler-Assistent mit eigenem System-Chip.
---

# Home Assistant Papa

## Kontext & Beschlüsse (Stand 11.11.2026)
1. **HA Green geht an Papa:** Sobald Daniels Home Assistant komplett auf dem M70q (Docker-Container) läuft und alles reagiert, wird der Green zurückgesetzt und an Papa übergeben/verkauft.
2. **Jungfräuliche Einrichtung:** Papas Instanz wird komplett neu eingerichtet – ausdrücklich NICHT Daniels Backup einspielen.
3. **Nuntius/HA-Fehler-Assistent sollen Papas System später mitverwalten:** Daniel will auf einen Blick sehen, von welchem HA-System ein Tages-/Wochenbericht stammt. Seit Nuntius v5.1 gibt es System-Chips dafür; Papas System bekommt bei Anlegung einen eigenen SYSTEME-Eintrag + eigene CSS-Farbe (Salbeigrün bleibt allein Daniels System vorbehalten).

## Offene Punkte
- Konkrete Wünsche aus früheren Chats (Geräte, Automatisierungen, Rollos/Lampen etc.) sind noch nirgends dokumentiert – mit Daniel aufnehmen.
- Technische Anbindung: MCP-Server-Integration in Papas HA + eigener Connector in Vibe (Muster siehe ha-project-context-Skill, „Fremde Instanz"). Fernzugriff: Nabu Casa oder Tunnel – offen.
- Zeitpunkt: erst nach abgeschlossenem HA-Umzug auf den M70q (Green wird erst freigegeben, wenn alles auf dem Mini-PC reagiert).

## Pflege
Vibe Work aktualisiert diese Datei nach jeder Arbeitssession und pusht den Stand hierher (per GitHub-Connector). Keine Secrets in dieses Repo.
