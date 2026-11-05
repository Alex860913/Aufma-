# Aufmaßbericht

Web-App zur Aufnahme von Aufmaßen für Terrassenüberdachungen – läuft im Browser auf Handy, Tablet und PC, ohne Server und ohne Installation.

## Funktionen

- **Bauvorhaben:** Kundenname, Adresse, Aufmaßdatum, Aufmaß durch
- **Aufmaßdaten:** Breite, Tiefe, Höhe Hauswand, Höhe Regenrinne (mm), Sonstiges
- **Bedachung:** Klarglas / Milchglas / Steg klar / Steg matt
- **Licht:** Anzahl Spots und LED-Leisten
- **Keilfenster:** Links/Rechts, Glas/Steg, klar/matt, Tiefe, Höhe hinten, Höhe vorne
- **Seiten:** Links, Rechts, Vorne 1–4, Hinten oder freie Bezeichnung – beliebig viele Felder
  - Schiebetüren (Flügel, Griffe, Zugluftstopper), Alu-Planken, Stegplatten, VSG-Glaswand, offen
  - Abmessungen Breite × Höhe, Bemerkung
- **Markise:** Aufdach / Unterdach / Senkrecht, Breite, Ausfall/Tiefe, Anschlusskabel links/rechts
- **Fotos:** direkt mit der Kamera aufnehmen oder hochladen, mit Beschreibung
- **PDF exportieren:** fertiger Aufmaßbericht inkl. Fotos; auf jeder Seite liegt eine CAD-Skizze der Überdachung als Wasserzeichen, bemaßt mit den eingegebenen Werten
- **App-Icon „AD“** für Browser-Tab, Desktop-Verknüpfung und Smartphone-Startbildschirm
- **Sichern / Laden:** Aufmaß als `.json`-Datei speichern und später wieder öffnen
- Automatisches Zwischenspeichern im Browser

## Veröffentlichen mit GitHub Pages

1. Neues Repository auf GitHub anlegen (z. B. `aufmass`).
2. Alle Dateien hochladen („Add file“ → „Upload files“):
   `index.html`, `manifest.webmanifest`, `icon.svg`, `icon-180.png`, `icon-192.png`, `icon-512.png`, `favicon-32.png`, `README.md`
3. Unter **Settings → Pages** bei „Source“ den Branch `main` und Ordner `/ (root)` wählen, speichern.
4. Nach ca. 1 Minute ist die App erreichbar unter
   `https://<dein-benutzername>.github.io/aufmass/`

Tipp: Auf dem Handy die Seite öffnen und „Zum Home-Bildschirm hinzufügen“ – dann startet sie wie eine App.

## Hinweise

- Für den PDF-Export wird die Bibliothek [jsPDF](https://github.com/parallax/jsPDF) von cdnjs geladen; dafür ist beim Öffnen der Seite eine Internetverbindung nötig.
- Alle Daten bleiben auf dem eigenen Gerät. Der Zwischenspeicher des Browsers ist begrenzt – bei vielen Fotos vor dem Schließen das PDF exportieren oder „Sichern“ nutzen.
