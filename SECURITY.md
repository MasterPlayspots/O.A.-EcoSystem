# Sicherheit

## Status

Dokumentations-/Community-Bootstrap, noch keine unterstützte Runtimeversion.
Der geplante Betrieb verbindet heterogene, teilweise experimentelle Geräte.
Keine fremden Systeme testen und keine Homebrew-, Firmware- oder Modellaktionen aus einem Issue ableiten.

## Vertraulich melden

Nach bestätigter Aktivierung der privaten Schwachstellenmeldung: im Repository unter
Security → Report a vulnerability melden. Die Aktivierung muss vor der Community-Ankündigung
in GitHub geprüft und im Bootstrap-Bericht bestätigt werden; diese Datei aktiviert nichts.
Ist die Option nicht verfügbar, zunächst nur ohne technische Details den Maintainer um einen
vertraulichen Kanal bitten. Keine Secrets oder ausnutzbaren Einzelheiten in öffentliche Issues schreiben.
Wir versprechen keine feste Reaktionszeit, solange kein betreuter Bereitschaftsprozess eingerichtet ist.

## Sicherheitsgrenzen

Keine Hardware-/Produktionszugänge in öffentlicher CI. Keine untrusted PRs auf persönlichen Rechnern
oder einem Self-Hosted-Runner mit Heimnetzzugriff ausführen. Im ersten Start nur Dokument-/Schema-Checks
auf GitHub-gehosteten Standardrunnern, minimale Rechte und keine Betreiber-Secrets.
Private Betriebsunterlagen sind kein öffentlicher Bugreport. Ein versehentlich veröffentlichtes Secret
ist als kompromittiert zu behandeln; Eskalation und Rotation koordiniert mit dem Eigentümer,
nicht nur Text löschen und den Vorfall als erledigt erklären.
