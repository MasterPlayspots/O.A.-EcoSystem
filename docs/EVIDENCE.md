# Evidenz, Messberichte und erste RAM-Untersuchung

## Nachweisarten

Eigene Messung (mit ausführender Person/Rücklauf), Repository-Prüfung, Herstellerangabe,
fremde Projektmessung, Hypothese und unbekannt werden getrennt geführt.
Das heutige Lesen eines alten Reports erneuert sein Messdatum nicht. Ein CI-Test mit Fixture misst keine PS5.
HTTP 200 beweist weder sichtbaren Text noch die Hardware oder den Backend. Neue Fähigkeiten werden erst nach Abnahme markiert.

## Minimaler redigierter Bericht

Quelle; Messzeit in UTC und Zeitzone; Gerätefamilie/CFI und Firmware; Host-/Runtime-/Modellrevision;
Hash und Hashprovenienz; Profil/Route ohne privaten Host; Parameter einschließlich Thinking, Kontext und Limit;
Cachezustand; tatsächliche Tokenzahl; Endegrund; erster sichtbarer Text; Headerzeit; Gesamtzeit;
Serverzeiten separat; Einheit und Messpunkt; Fehler und Endzustand.

Keine Secrets, Seriennummern, Host-IDs, privaten Prompts oder Antwortinhalte verlangen.
Fehlende Werte sind null mit Begründung, nicht 0 Leistung oder 0 Byte.
Dauern pro Messpunkt mit monotoner Uhr, keine Differenz unsynchronisierter Hostzeitstempel.
Rohdaten begrenzt und redigiert mit Prüfsumme erhalten. Kleine Stichproben nicht als Dauerlast/p95 vermarkten.

## RAM-01: erst beobachten, nicht bis zum Crash allokieren

Ziel ist zunächst ein stabiles Arbeitsprofil eines definierten Inferenzlaufs, keine behauptete absolute Obergrenze.
Zuerst vorhandene Logs und unterstützte Counter des tatsächlichen Inferenzprozesses prüfen.
Ein neuer Diagnosepayload ist ein Eingriff und braucht eine separate Freigabe; sein Name beweist keine Passivität.
Linux-/BSD-Zähler nicht ohne bestätigte Plattformsemantik auf der PS5 voraussetzen.

Getrennte Größen: Modelldateibytes, Mapping, aktuelle Residency/RSS, Peak, angeforderte/erfolgreiche Sperrbytes,
KV-/rekurrente Zustandsbuffer, Arbeitsbuffer, Runtimeoverhead, Fault-/I/O-Deltas und Systemdruck.
Überlappende Speicheranteile nicht doppelt zählen. mlock-Anforderung ist kein Erfolg.
Minor Faults beweisen keinen Datenträgerzugriff; Major Faults/File-Page-ins nicht automatisch Swap.

Erst nach Instrumentierungsreview und Betriebsfreigabe: kleines 0.8B-Profil, ein Modell,
kurze sequenzielle Anfragen, begrenzte Telemetrie und Idle-/Wiederaufnahmebeobachtung.
Messbudget, Abtastrate, Rückweg und Stopregeln vorher festlegen; keine Priorität/Threads/Dateigrenze erhöhen.
Bei Warnungen, API-Verlust, UI-Blockade oder Budgetüberschreitung keine weiteren Aufträge.
2B und Kontextvariationen folgen getrennt. Keine Vollhash-/Full-Page-Touch-Aktion unmittelbar vor
Residencyversuchen als vermeintlich zustandsneutrale Messung.

Fremde Messungen aus [PS5LM CONSOLE.md](https://github.com/cobanov/PS5LM/blob/4173291e0554ff60945f3ed3b0a2d9dcc5190168/docs/CONSOLE.md)
gehören zu dessen Testgerät, nicht zu jeder Konsole. Die dort beschriebenen Grenzen sind keine eigenen Sicherheitsbudgets.
Keine neue Geräteprüfung wurde durch das Verfassen dieses Dokuments ausgeführt.


## Einordnung im neuen Dachprojekt

Die PS5-spezifische RAM-Untersuchung ist ein einzelnes Profil. Andere Geräte benötigen
entsprechende eigene Zähler und Tests; API-, Betriebssystem- und Ressourcensemantik nicht übertragen.
Die allgemeinen Evidenzregeln gelten unabhängig von einem bestimmten Gerät.
