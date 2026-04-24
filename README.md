# Pollentagebuch

Einfaches mobiles Allergie-/Pollentagebuch als einzelne HTML-Datei.

## Nutzung

Öffne die veröffentlichte URL im Browser. Die App läuft vollständig im Browser — es gibt keinen Server und keine Datenübertragung.

Alle Einträge werden ausschließlich lokal im `localStorage` des Geräts gespeichert. Sie verlassen das Gerät nicht.

## Funktionen

- Tägliche Erfassung von Symptomen, Medikamenteneinnahme und Notizen
- Wöchentliche Pollenbelastungsdaten (mehrere Pollenarten, skaliert keine/niedrig/mittel/hoch)
- Kalenderansicht der Einträge
- Zusammengefasster Arztbericht (druck-/PDF-fähig)
- **Datenbackup:** Export aller Daten als JSON-Datei, Import aus JSON-Datei

## Datenbackup

Im Abschnitt „Datenbackup" am unteren Ende der App:

- **Daten exportieren** speichert alle lokalen Daten als JSON-Datei (Dateiname `pollentagebuch-backup-YYYY-MM-DD.json`).
- **Daten importieren** lädt eine zuvor exportierte JSON-Datei zurück in den Browser. Vor dem Überschreiben kommt eine Sicherheitsabfrage.

Es wird empfohlen, regelmäßig ein Backup zu erstellen — z.B. einmal pro Woche per E-Mail an sich selbst.

## Technik

- Einzelne `index.html` (HTML + CSS + JS in einer Datei)
- Keine externen Scripts, keine Abhängigkeiten
- Keine Netzwerkanfragen
- PWA-fähig (als Icon auf dem Startbildschirm installierbar)

## Datenschutz

Die App speichert **ausschließlich im lokalen Browser-Speicher** des Endgeräts. Es gibt keinerlei Datenübertragung an einen Server oder Dritte. Die hier im Repository liegende `index.html` enthält keine personenbezogenen Daten — nur die App-Logik mit Medikamenten-Labels als UI-Voreinstellungen.
