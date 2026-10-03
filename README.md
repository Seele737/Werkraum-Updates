# Werkraum – Updates und Erweiterungen

Dieses öffentliche Repository verteilt die veröffentlichten Werkraum-Versionen und signierten Erweiterungen. Die Entwicklung bleibt im privaten Repository Seele737/Werkraum. Es enthält keine Nutzerprojekte, Zugangsdaten oder privaten Signaturschlüssel.

## Bezugsquellen

- Programmdateien: [GitHub Releases](https://github.com/Seele737/Werkraum-Updates/releases).
- Online-Store für Werkraum: `https://raw.githubusercontent.com/Seele737/Werkraum-Updates/main/store/`
- Signierte Update-Liste: `https://raw.githubusercontent.com/Seele737/Werkraum-Updates/main/updates.json`

Die Quellen werden erst freigegeben, sobald die zugehörigen Dateien vollständig veröffentlicht und geprüft sind. Zum Herunterladen ist keine GitHub-Anmeldung und kein Token nötig. Werkraum prüft Signaturen und Prüfsummen; eine neue Version wird nicht ungefragt installiert.

## Einrichtung in Werkraum ab 0.14.0

Im Store unter „Woher Erweiterungen kommen“ die Online-Store-Adresse speichern. Im Entwicklerbereich unter „Updates aus dem Internet“ die vollständige Adresse der signierten Update-Liste speichern. Die automatische Suche nach Programmupdates ist optional; Herunterladen und Installieren bleiben getrennte Schritte.

## Hinweise zum Mac

Die Mac-Update-Dateien sind signierte Bausätze, keine fertig beglaubigten DMGs. Werkraum ab 0.10.3 kann damit auf dem Mac eine neue App vorbereiten; Internet und Bauwerkzeuge sind erforderlich. Für ältere Installationen dient `Werkraum-aktualisieren.command` im Mac-Bausatz. Ein echter Mac-Gerätetest steht noch aus.

## Veröffentlichung

Nur geprüfte, lokal signierte Verteilungsdateien veröffentlichen. Ein Release zunächst als Entwurf vollständig hochladen und prüfen, dann freigeben. Erst anschließend die signierte Update-Liste und den passenden Store gemeinsam aktualisieren. Vorhandene Release-Dateien nicht unter derselben Versionsnummer ersetzen.
