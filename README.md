# O.A.-EcoSystem

**Vorhandene Geräte sinnvoll verbinden — passende Aufgaben, eigene Infrastruktur, überprüfbare Ergebnisse.**

**Phase: Community-Bootstrap / Planungs- und Dokumentationsstand.**
Dieses Repository ist ein Mitmach-Ort. Es enthält noch keinen installierbaren Inferenz-Kern,
keine getestete automatische Geräteerkennung und keine allgemeine Hardwarefreigabe.
Die Dateien wurden für den ersten öffentlichen Stand vorbereitet; der tatsächliche Online-Stand
ist am Repository und seinen Commits zu prüfen.

## Was wir entwickeln

Eine modulare Integrationsschicht, die sich an den **nachgewiesenen Fähigkeiten** der vorhandenen
Geräte orientiert. Ein Rechner kann Client, Gateway, Vermittler oder Inferenzworker sein;
nicht jedes Gerät muss oder kann jede Rolle übernehmen. Das gilt auch für spätere Spezialworker.
PS5 & Hetzner ist unser historisches experimentelles Referenzprofil, nicht das verpflichtende Grundsystem.

Kein OurArk-Konto, keine eigene PS5, kein bestimmter Hostinganbieter und kein permanenter Cloudzugang
sollen Voraussetzungen für den allgemeinen Einstieg sein. Andere Laufzeiten und Geräte benötigen jeweils
Adapter-, Lizenz-, Sicherheits- und Funktionstests. Modellgewichte und Hardwaregrenzen bleiben am jeweiligen Knoten;
ein Netzwerktunnel addiert nicht die Arbeitsspeicher oder GPUs verschiedener Geräte.

## Zuerst lesen und mitarbeiten

[Projektindex](docs/PROJECT_INDEX.md) · [Plan](docs/MASTERPLAN.md) · [Geräteprofile](docs/PROFILES.md) ·
[Architektur](docs/ARCHITECTURE.md) · [Roadmap](docs/ROADMAP.md) · [Kommunikation](docs/COMMUNICATION.md)

Konkrete Arbeit gehört in Issues, Änderungen in kleine Pull Requests, Fragen/Ideen in Discussions —
Einstieg: [Hier anfangen / Mitmachen](https://github.com/MasterPlayspots/O.A.-EcoSystem/discussions/14). Dokumentation, API-Verträge, Quellenprüfung, Mock-Tests und Übersetzungen
ermöglichen Mitarbeit ohne Konsole. [Beitragsregeln](CONTRIBUTING.md) und [Reviewauftrag](docs/CLAUDE_REVIEW.md)
erklären den Einstieg.

## Geplante Einstiege

| Profil | Nutzen | Status dieses Repositorys |
|---|---|---|
| Mock | Schnittstellen ohne Gewichte, Cloud und Inferenzgerät prüfen | Geplant |
| Ein lokaler Host | Client, Gateway und passender Worker auf einem Rechner | Geplant; Laufzeit separat validieren |
| Heimnetz | Ein oder mehrere eigene Geräte über explizite Konfiguration | Geplant; zunächst genau ein ausgewählter Worker |
| Privater Fernzugriff | Eigenes Gateway und kontrollierter Transport | Geplant; keine automatische Cloudbereitstellung |
| PS5-Referenz | Dokumentierten PS5–Vermittler–VPS-Weg reproduzieren | Historisches Experiment, hier noch nicht neu abgenommen |

GPU, MoE, PS4, frei ausführbare Jobs, Mandantenbetrieb und Simulation sind keine belegten Fähigkeiten
unseres Starts. Auch NAS, ARM-Mini-PC, Windows, macOS und Linux erhalten nur nach konkreten Prüfungen
passende Unterstützungsangaben. Ein Mobilgerät beginnt als Client; lokale mobile Inferenz ist eine eigene Forschungsaufgabe.

## Transparenz und Credits

Wir entwickeln Integration und Nachbaubarkeit, nicht eine neue LLM-Engine. Das PS5-Referenzexperiment
basiert auf **PS5LM / cobanov**, **llama.cpp / ggml**, der Arbeit von **Relapse** und
**ps5-payload-dev / John Törnblom** sowie **Qwen**-Modellen in **Unsloth**-GGUF-Quantisierungen.
Weitere direkte, indirekte und optionale Beiträge stehen in [CREDITS.md](CREDITS.md).

Eigene Bootstrap-Dokumente: [MIT](LICENSE). Fremde Projekte behalten ihre Lizenzen;
[THIRD_PARTY_NOTICES.md](THIRD_PARTY_NOTICES.md) ist keine pauschale Freigabe fremder Binärdateien.
Keine Firmware, Gewichte, Payload-/SDK-Bundles, Herstellerfonts oder Betreiber-Secrets sind enthalten.

Projektverantwortlicher: **Kevin Fröba**. Unabhängiges Communityprojekt, keine Partnerschaftszusage
oder offizielle Unterstützung durch erwähnte Hersteller/Upstreams. [Sicherheitsmeldungen](SECURITY.md).
