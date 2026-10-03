# Werkraum – Updates und Erweiterungen

Dieses öffentliche Repository verteilt geprüfte Werkraum-Versionen und signierte Erweiterungen. Die Entwicklung in `Seele737/Werkraum` bleibt privat. Nutzerprojekte, Zugangsdaten und private Signaturschlüssel gehören nicht hierher.

- [Downloadseite](https://seele737.github.io/Werkraum-Updates/)
- [Programmdateien und ältere Versionen](https://github.com/Seele737/Werkraum-Updates/releases)
- [Erweiterungskatalog](https://seele737.github.io/Werkraum-Updates/store/)

## In Werkraum verwenden

Ab Werkraum 0.14.1 sind beide Quellen voreingestellt. Neue Einstellungen prüfen beim Start und alle sechs Stunden nach Programmupdates. Eigene Quellen und deaktivierte Suche bleiben erhalten. Die Quellen lassen sich im Programm ändern:

**Store → Woher Erweiterungen kommen → Online-Store:**

```text
https://seele737.github.io/Werkraum-Updates/store/
```

**Entwicklerbereich → Updates aus dem Internet:**

```text
https://seele737.github.io/Werkraum-Updates/current/updates.json
```

Es ist keine GitHub-Anmeldung und kein Token im Programm nötig. Werkraum prüft die Signatur der Listen sowie Signaturen und Prüfsummen der Pakete. Die automatische Suche nach Programmupdates ist optional. Herunterladen und Installieren bleiben getrennte Schritte.

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

