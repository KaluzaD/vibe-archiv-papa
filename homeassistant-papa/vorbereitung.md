# Vorbereitung „Tag bei Papa" – Arbeits- und Checkliste

Stand: 11.11.2026 · Beschluss: Green wird ZU HAUSE komplett vorbereitet (Daniels Wahl),
bei Papa bleiben nur Onboarding, Geräte, Nabu Casa, Feinschliff. LAN-Kabel möglich.

## A. Zuhause vorbereiten (mit Vibe Code)

### A1. Vor dem Leeren des Green (Sicherheit)
- [ ] M70q-System prüfen: läuft ALLES (besonders Zigbee/USB-Stick!) seit dem Container-Umzug stabil?
- [ ] Frisches HA-Backup auf dem M70q + zweite Kopie außerhalb (Backup-Konzept beachten)
- [ ] Dann erst: Green zurücksetzen (Werkseinstellungen)

### A2. Green-Grundsetup (daheim im LAN)
- [ ] Green per LAN ans heimische Netz, frisches Onboarding
- [ ] Neueste HA-Version, Sprache Deutsch, Zeitzone Europe/Berlin
- [ ] Keine Geräte von Daniel einbinden, KEIN Backup einspielen (jungfräulich)
- [ ] Benutzer-Konzept vorbereiten: 1 Admin-Konto für Papa + ggf. Technik-Konto für Daniel
- [ ] HACS installieren (Voraussetzung Simon42-Dashboard)
- [ ] Simon42-Dashboard-Bausteine vorinstallieren (Mushroom Cards, custom button-card, clock-weather-card, Kiosk Mode o. ä. – final mit Vibe Code klären)
- [ ] Grund-Dashboard einmal aufbauen (Struktur: Wohnen, Schlafen, Küche, Balkonkraftwerk, Multimedia)

### A3. Support-Paket für den Tag X
- [ ] Checkliste „Vor Ort" ausdrucken/ins Handy (siehe B)
- [ ] Zugangsdaten-Blatt: WLAN-Passwort Papa, Fritzbox/Router-Zugang, E-Mail-Konten für HA-Cloud
- [ ] Ersatz-LAN-Kabel + ggf. Powerbank/Stromkabel einpacken
- [ ] MacBook mit Vibe Code (für Feinschliff vor Ort)

## B. Vor Ort bei Papa (Reihenfolge)

1. [ ] Green per LAN-Kabel an den Router, Strom – Onboarding mit Papas Daten
2. [ ] Papas Handy: HA-Companion-App installieren (Push-Benachrichtigungen!)
3. [ ] **Nabu Casa:** Papas eigenes Abo (~5 €/Monat) unter Papas Konto/Kreditkarte anlegen,
       Remote UI aktivieren → Daniel hat sofort Fernzugriff
4. [ ] **MCP-Server-Integration** in Papas HA aktivieren
5. [ ] **Eigener HA-Connector in Daniels Vibe** anlegen (Custom MCP Connector, eigene URL) –
       Lesen: Always allow · Schreiben/Löschen: manuelle Bestätigung (wie bei Max)
6. [ ] Geräte einbinden (siehe C – Brands vorab klären!)
7. [ ] Simon42-Dashboard an echte Geräte anpassen (Vibe Code)
8. [ ] Erste Automatisierungen nur die simplen, offensichtlichen (Rest später remote)
9. [ ] Backup-Konzept für Papa festlegen (z. B. HA-Backup-Add-on auf USB-Stick oder monatlich manuell)
10. [ ] Papas Vibe-Account anlegen (später, mit ihm zusammen) + eigener Connector

## C. Geräte bei Papa – VOR der Fahrt klären (Marke/Modell!)

| Bereich | Was klären? | Integration vermutlich |
|---|---|---|
| Lampen | Marke? (z. B. Zigbee/Tuya/TP-Link/Hue) | tbd |
| Rollos | Marke? (z. B. Zigbee/Shelly/Tuya) | tbd |
| Balkonkraftwerk | Wechselrichter-Marke? (Hoymiles/Deye/APsystems/Solarman …) | MQTT/OpenDTU, Solarman, APsystems Local API |
| Spülmaschine | Marke? (Bosch/Siemens = Home Connect?) | Home Connect |
| Fernseher | Marke? (Samsung = Daniels TV-Know-how!) | Samsung TV / LG / Android TV |
| Steckdosen | Marke? (Shelly/Tuya/TP-Link …) | tbd |

## D. Langfristig / danach (remote von zu Hause)
- [ ] Papas System als eigenes SYSTEME-System-Chip in Nuntius anlegen (eigene Farbe, NICHT Salbeigrün)
- [ ] HA-Fehler-Assistent für Papas Instanz erweitern (eigene HA_URL/HA_TOKEN-Umgebung)
- [ ] Nuntius-Tagesbericht für Papa testen
- [ ] Backup-Erinnerung einrichten
