# Werkraum – Updates und Erweiterungen

Dieses öffentliche Repository verteilt geprüfte Werkraum-Versionen und signierte Erweiterungen. Die Entwicklung in `Seele737/Werkraum` bleibt privat. Nutzerprojekte, Zugangsdaten und private Signaturschlüssel gehören nicht hierher.

- [Downloadseite](https://seele737.github.io/Werkraum-Updates/)
- [Programmdateien und ältere Versionen](https://github.com/Seele737/Werkraum-Updates/releases)
- [Erweiterungskatalog](https://seele737.github.io/Werkraum-Updates/store/)

## In Werkraum verwenden

Werkraum 2.3.0 ergänzt fünf gezielt herunterladbare lokale Rollenspielmodelle mit Hardwareeinschätzung: Huihui Qwen3 1,7B (abliterated/uncensored), Huihui Qwen3 4B Instruct 2507 (abliterated/uncensored), Stheno 3.2 8B (SFW-/NSFW-Finetuning, nicht kommerziell), Dolphin 3.0 8B (uncensored) und NemoMix Unleashed 12B (RP-Merge ohne belegte Uncensored-Zusage). Originalkarten, Lizenzen und Downloadquellen sind direkt in der Auswahl verlinkt. Speicher und Tempo werden für den ausführenden Rechner geschätzt; kein Modell garantiert grenzenlose Antworten. Gewichte werden separat nur auf Nutzerklick geladen; das Programmupdate enthält keine Modellgewichte.

Werkraum 2.2.0 bietet eine ausdrücklich aktivierte automatische private GitHub-Sicherung neuer Wünsche. Jede Aufgabe zeigt einen Beleg für die zuletzt übertragene Fassung und ihre Ergänzungen. „Nur lokal“ bleibt je Wunsch möglich; alte Einträge werden nicht rückwirkend geteilt. Einrichtung und Anmeldung erfolgen je Rechner. Private Issues sind keine Ende-zu-Ende-Verschlüsselung.

Werkraum 2.1.0 ergänzt KI → Rollenspiel: 16 anpassbare Szenarien, acht Figurenprofile und eigene lokale Geschichten. Anbieter, Modell und Spielregeln gelten je Geschichte; Projektdateien und Werkzeuge bleiben außerhalb des Rollenspiels. Lokale Speicherung und JSON-Exporte sind unverschlüsselt. Ein lokales Modell muss vorher installiert sein; das gekoppelte Handy nutzt weiterhin den Rechner.

Ab Werkraum 0.14.1 sind beide Quellen voreingestellt. Neue Einstellungen prüfen beim Start und alle sechs Stunden nach Programmupdates. Eigene Quellen und deaktivierte Suche bleiben erhalten. Die Quellen lassen sich im Programm ändern:

**Store → Woher Erweiterungen kommen → Online-Store:**

```text
https://seele737.github.io/Werkraum-Updates/store/
```

**Einstellungen → Programmupdates → Updates aus dem Internet:**

```text
https://seele737.github.io/Werkraum-Updates/current/updates.json
```

Es ist keine GitHub-Anmeldung und kein Token im Programm nötig. Werkraum prüft die Signatur der Listen sowie Signaturen und Prüfsummen der Pakete. Die automatische Suche nach Programmupdates ist optional. Ohne „Updates automatisch durchführen“ startest du Download und Installation selbst; mit diesem ausdrücklich eingeschalteten Schalter wartet Werkraum auf eine sichere Arbeitspause.

Neue kompatible Apps und App-Updates werden unabhängig vom Hauptprogramm aus dem Store angeboten. Eine App, die neue Kernfunktionen benötigt, nennt ihre Mindestversion. Bereits veröffentlichte Paketversionen bleiben unverändert erhalten; Hintergrundaufträge überschreiben keine zwischenzeitlich installierte neuere App.

Werkraum Studio 2.0 bringt einen anpassbaren Arbeitsplatz, neue Navigation und Animationen, Projektschlagwörter, eine Dateiimportvorschau mit Inhaltsvergleich und übertragbare Darstellungseinstellungen. Der Web-App-/iPhone-Ausbauplan steht unter Entwicklung; die Handyoberfläche ist weiterhin mit dem laufenden Rechner verbunden.

## Passende Datei wählen

- Windows ab 0.14.1: kleine `…-code.wrup`, nur Programmcode bei unveränderter Electron-Laufzeit. Bis 0.14.0 einmal die größere `Werkraum-Update-0.14.1.wrup` installieren.
- Mac mit Apple-Chip: `…mac-arm64.wrup`; Intel: `…mac-x64.wrup`. Werkraum ab 0.10.3 benötigt Internet und Bauwerkzeuge, um daraus auf dem Mac eine neue App vorzubereiten.
- Älterer Mac oder erste Einrichtung: Mac-Bausatz entpacken und dessen Anleitung lesen. `Werkraum-aktualisieren.command` aktualisiert eine vorhandene App mit Sicherung.
- Erweiterungen: aus dem Online-Store installieren oder die separate Erweiterungen-ZIP verwenden.

Die Mac-Dateien sind signierte Bausätze, keine bei Apple beglaubigten fertigen DMGs. Gerätespezifische Einschränkungen stehen in den jeweiligen Release-Beschreibungen.

Die ältere Quelle `/updates.json` bleibt als Erstwechsel auf 0.14.1 erhalten; neue Versionen werden unter `/current/updates.json` angeboten. Bei einem Wechsel der Electron-Laufzeit ist erneut ein vollständiges Laufzeit-Update erforderlich.

## Veröffentlichungsverfahren

Pakete werden im privaten Entwicklungsordner gebaut, geprüft und lokal signiert. Der private Signaturschlüssel bleibt dort. Ein Release zunächst als Entwurf vollständig hochladen und SHA-256-Prüfsummen abgleichen, dann freigeben. Erst danach Store und signierte `updates.json` aktualisieren. Eine veröffentlichte Versionsnummer nicht für andere Dateien wiederverwenden.

GitHub Pages liefert den Zweig `main` aus `/` aus. `.nojekyll` verhindert Veränderungen an den Verteilungsdateien. Die großen Installer und Updates liegen in Releases, nicht in der Git-Historie. Direkte `raw.githubusercontent.com`-Adressen sind wegen des Text-Inhaltstyps für Werkraums Update-Liste ungeeignet.
