# Repository-Administration — Zielkonfiguration, nicht Aktivierungsnachweis

Nach dem ersten redigierten Bootstrapcommit Einstellungen tatsächlich lesen und im Ergebnisbericht
belegen. Eine Datei namens CODEOWNERS/SECURITY.md ist keine Plattformkonfiguration.

| Bereich | Ziel |
|---|---|
| Owner / Name | MasterPlayspots / O.A.-EcoSystem |
| Sichtbarkeit | Public; nur dieses neue Repo, keine Sichtbarkeitsänderung anderer Repos |
| Default branch | main |
| Community | Issues und Discussions an; kein separates Wiki als zweite Dokumentationsquelle |
| Merge | Kein Auto-Merge; nach Bootstrap nur PRs |
| main | Kein Force-Push, keine Löschung, Gespräche auflösen, 1 erforderliches Approval |
| Checks | Nur wirklich vorhandene erfolgreiche Checknamen als Pflicht konfigurieren |
| Security | Private Schwachstellenmeldung aktivieren/verifizieren, Secret-Scanning/Pushschutz prüfen |
| Actions | Keine Betreiber-Secrets, read-only contents, kein privilegierter PR-Checkout, keine Heimrunner |
| Kosten | Keine kostenpflichtigen Zusatzprodukte, große Runner, Cloudkonten oder Domains anlegen |

Fehlt ein zweiter Reviewer, bleiben eigene Änderungen in PRs offen. Das ist kein Anlass, sich mit
 demselben Konto ein unabhängiges Approval zu erteilen oder Schutz abzuschalten. Einschränkungen
 der Rechte/API genau berichten; UI-Schritt des Owners als offenen Punkt benennen.

Zum Start reichen lokal überprüfte Dokumente und JSON. Eine neue docs/schema-CI ist ein eigener
 kleiner PR; kein grünes Badge und kein Runtime-Testversprechen vor tatsächlichem CI-Lauf.
Community-Ankündigung erst nach anonymer Ansicht und Prüfung der Mitmach-/Meldewege.
