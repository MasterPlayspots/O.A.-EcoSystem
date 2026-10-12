# Sicherheit

## Status

Dokumentations-/Community-Bootstrap, noch keine unterstützte Runtimeversion.
Der geplante Betrieb verbindet heterogene, teilweise experimentelle Geräte.
Keine fremden Systeme testen und keine Homebrew-, Firmware- oder Modellaktionen aus einem Issue ableiten.

## Vertraulich melden

Die private Schwachstellenmeldung von GitHub ist für dieses Repository aktiviert (zuletzt geprüft
am 12.10.2026). Schwachstellen bitte über Security → Report a vulnerability melden:
<https://github.com/MasterPlayspots/O.A.-EcoSystem/security/advisories/new>.
Der Menüpunkt ist öffentlich sichtbar; zum Absenden ist ein angemeldetes GitHub-Konto nötig.
Diese Datei selbst schaltet nichts ein — maßgeblich ist die Repository-Einstellung. Keine Secrets oder ausnutzbaren Einzelheiten in öffentliche Issues schreiben.
Wir versprechen keine feste Reaktionszeit, solange kein betreuter Bereitschaftsprozess eingerichtet ist.

## Sicherheitsgrenzen

Keine Hardware-/Produktionszugänge in öffentlicher CI. Keine untrusted PRs auf persönlichen Rechnern
oder einem Self-Hosted-Runner mit Heimnetzzugriff ausführen. Im ersten Start nur Dokument-/Schema-Checks
auf GitHub-gehosteten Standardrunnern, minimale Rechte und keine Betreiber-Secrets.
Private Betriebsunterlagen sind kein öffentlicher Bugreport. Ein versehentlich veröffentlichtes Secret
ist als kompromittiert zu behandeln; Eskalation und Rotation koordiniert mit dem Eigentümer,
nicht nur Text löschen und den Vorfall als erledigt erklären.
