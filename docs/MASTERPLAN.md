# Masterplan — geräteunabhängiger Einstieg

## Ziel

Ein Anwender verwendet passende Rollen auf den Geräten, die er bereits besitzt. Die geplante
Integrationsschicht verbindet Anwendungen mit ausdrücklich konfigurierten Rechenendpunkten.
Geräteprofile ergänzen den Kern, sie definieren ihn nicht. PS5 & Hetzner bleibt eine historische
Forschungsbasis und ein künftiger Nachbaupfad, kein Pflichtbestandteil.

## Erstes umsetzbares Teilziel

Zuerst Community-Dokumentation online, dann Fähigkeiten-/API-Vertrag, dann ein hardwarefreier Mock.
Anschließend ein generischer HTTP-Textworker, clientseitige Beispiele und ein geprüfter Einzelhostpfad.
Danach die bekannte PS5-Strecke schrittweise abnehmen. Der erste Runtimeumfang bleibt ein Betreiber,
ein ausgewählter Worker, eine gleichzeitig zugelassene Anfrage. Kein Scheduler wird dafür benötigt.

## Adapter statt universeller Installer

Ein Geräteprofil beschreibt OS/Architektur/Firmware, Runtime/Backend, Modellherkunft, zulässige
Rollen, installierte und nachgewiesene Funktionen sowie Testdatum. Ein Adapter übersetzt lediglich
zwischen dem überprüften Backendvertrag und dem Kern. Keine automatische Installation fehlender Treiber,
keine Hardwareübernahme und keine beliebige Programmausführung aus Communityprofilen.

Der konfigurierende Anwender entscheidet lokal, im LAN oder über einen eigenen entfernten Zugang.
Alle Konten, Domains und Schlüssel gehören ihm. Eine lokale Policy verhindert ungefragtes
Cloud-Ausweichen oder Senden von Daten an andere Betreiber.

## Erweiterungen

Mehrere Geräte, Jobwarteschlange, Modellrouting und Failover folgen erst nach Definition von
Identität, Leases, Deadlines, Abbruch, Idempotenz und Datenschutz. Rendering, Simulation, Audio,
Embeddings, GPU, MoE und lokale mobile Inferenz sind eigenständige Fähigkeiten mit eigenen Tests.
Das Projekt ist offen für diese Pfade, behauptet sie aber nicht als schon verfügbar.

## Veröffentlichung

Der erste öffentliche Stand enthält neue eigene Dokumentation, Profile als Entwürfe und Reviews.
Runtimecode wird später selektiv auf einem eigenen Branch vorbereitet; kein privates Monorepo
und keine dessen Git-Historie veröffentlichen. Jede tatsächliche Hardwarefreigabe braucht Nachweise.
Eine unbekannte absolute RAM-Kapazität blockiert keine ehrlich begrenzte Dokumentationsöffnung.

Siehe [Roadmap](ROADMAP.md), [Profile](PROFILES.md), [Sicherheitsrichtlinie](../SECURITY.md)
und [Credits](../CREDITS.md). Keine Betriebsaktion aus diesem Plan ableiten.
