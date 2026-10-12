# Credits und nachvollziehbare Herkunft

Stand: 12. Oktober 2026. Anerkennung ist keine Behauptung direkter Mitarbeit, Partnerschaft oder
Unterstützung dieses Projekts. Das Register unterscheidet Grundlagen, indirekte Bestandteile und Forschung.
Die tatsächliche Zusammensetzung künftiger Softwarepakete muss je Release geprüft werden.

## Konsolen- und Inferenzgrundlagen

| Projekt / Urheber | Beitrag | Quellenstand / Lizenzhinweis |
|---|---|---|
| [PS5LM — cobanov und Mitwirkende](https://github.com/cobanov/PS5LM) | Portierung, Payload, Modellbibliothek, Einbettung der Inferenz | Historischer Referenzrelease v0.1.1; GPL-3.0-or-later laut [README](https://github.com/cobanov/PS5LM/blob/a7debaf060f8e1632ade04a841f4d89e2d2b51f9/README.md) |
| [llama.cpp / ggml](https://github.com/ggml-org/llama.cpp) | Eigentliche Modell-Inferenz, Server und GGUF-Verarbeitung | [MIT am Referenzcommit](https://github.com/ggml-org/llama.cpp/blob/552f18f912a32ea86edf82e2b76431cb7131538d/LICENSE) |
| [ps5-payload-dev / John Törnblom und Mitwirkende](https://github.com/ps5-payload-dev) | Offene Konsolenwerkzeuge | [SDK v0.43](https://github.com/ps5-payload-dev/sdk/tree/v0.43): GPLv3+ mit BSD- und dateibezogenen Ausnahmen |
| [ps5-payload-dev/elfldr](https://github.com/ps5-payload-dev/elfldr) | ELF-Loader | GPLv3+ laut [README](https://github.com/ps5-payload-dev/elfldr#license); konkreter Nachbau-Build noch festzulegen |
| [Relapse — ntfargo und Mitwirkende](https://github.com/ntfargo/Relapse-Exploit) | Konsolenzugang für passende autorisierte Geräte | [MIT](https://github.com/ntfargo/Relapse-Exploit/blob/main/LICENSE); konkreter Nachbau-Commit noch festzulegen |
| [Qwen Team / Alibaba](https://huggingface.co/Qwen) | Ursprüngliche Referenzmodelle | Modellkarten: [Qwen3.5 0.8B](https://huggingface.co/Qwen/Qwen3.5-0.8B), [2B](https://huggingface.co/Qwen/Qwen3.5-2B); Lizenz der konkreten Revision vor Bezug zuordnen |
| [Unsloth AI und Mitwirkende](https://huggingface.co/unsloth) | Vorgesehene GGUF-Quantisierungen | [0.8B-GGUF](https://huggingface.co/unsloth/Qwen3.5-0.8B-GGUF), [2B-GGUF](https://huggingface.co/unsloth/Qwen3.5-2B-GGUF); dies behauptet keine Nutzung der Unsloth-Trainingsbibliothek |
| Kevin Fröba / OurArk und künftige Mitwirkende | Projektplanung, Dokumentation und künftige Integration | Die Engine, Zugangstechnik und Gewichte werden nicht als eigene Erfindung dargestellt |

## Namentliche Relapse-Credits

Das [Upstream-README](https://github.com/ntfargo/Relapse-Exploit#credits) nennt:
**Sonic_Iso** (Kernel Exploit), **Jordy** (Webkit Exploit und Kernel Bug), **ntfargo** und **ufm42**
(Exploit Development) sowie **Dr. Yenyen** (Testing).
Zusätzlich werden **TheFlow, SlidyBat, Flatz, cow, nhk, bollarz, Sleirsgoevy, EchoStretch und EarthOnion** genannt.
Diese Zuordnung gilt für ihre Upstream-Arbeit, nicht für eine behauptete direkte OurArk-Mitwirkung.

## Indirekte Bibliotheken und Daten

| Bestandteil | Beitrag / Herkunft | Prüfgrenze |
|---|---|---|
| [cpp-httplib — Yuji Hirose](https://github.com/yhirose/cpp-httplib) | HTTP-Bibliothek, MIT; [vendorter Header](https://github.com/ggml-org/llama.cpp/blob/552f18f912a32ea86edf82e2b76431cb7131538d/vendor/cpp-httplib/httplib.h) | Nicht in diesem Dokumentationsstart gebündelt |
| [JSON for Modern C++ — Niels Lohmann](https://github.com/nlohmann/json) | JSON-Verarbeitung, MIT; [vendorter Header](https://github.com/ggml-org/llama.cpp/blob/552f18f912a32ea86edf82e2b76431cb7131538d/vendor/nlohmann/json.hpp) | Konkrete Datei-Notices bei Übernahme erhalten |
| [Mbed TLS](https://github.com/Mbed-TLS/mbedtls) | TLS; [3.6.7-Lizenz](https://github.com/Mbed-TLS/mbedtls/blob/mbedtls-3.6.7/LICENSE): Apache-2.0 OR GPL-2.0-or-later | Lizenzwahl und Buildbestand vor eigener Verteilung dokumentieren |
| Mozilla/NSS und [curl / mk-ca-bundle](https://curl.se/docs/caextract.html) | CA-Daten und Konvertierung | Datenlizenz und Notices getrennt prüfen; keine pauschale PS5LM-Lizenzzuordnung |
| [PS5Dev/PS5SDK](https://github.com/PS5Dev/PS5SDK), FreeBSD-Mitwirkende | Im SDK dokumentierte indirekte Herkunft | Tatsächlich übernommene Dateien und Ausnahmen bestimmen |
| LLVM/Clang/LLD, CMake, Ninja, GNU Make | Optionale Eigenbau-Werkzeuge | Kein SDK-/Toolchain-Neubau als Voraussetzung jedes Nutzers |

## Hosts, Netzwerk, Plattformen und Werkzeuge

**[Node.js](https://github.com/nodejs/node)** als vorgesehene Host-Laufzeit,
**[OpenSSH/OpenBSD](https://github.com/openssh/openssh-portable)** für den Reverse-Tunnel und
**[cloudflared](https://github.com/cloudflare/cloudflared)** für das optionale Tunnelprofil.
Die [cloudflared-Lizenz](https://github.com/cloudflare/cloudflared/blob/master/LICENSE) ist von den
Nutzungsbedingungen des Cloudflare-Dienstes zu unterscheiden.

Je nach tatsächlich gewähltem Profil kommen Python/Python Software Foundation, curl/libcurl,
Git, Bash, socat, systemd sowie Apple launchd/macOS-Dienste hinzu. Erwähnung ist kein Beleg ihrer
Installation. Betriebssysteme und ihre Pakete behalten eigene Bedingungen.

**Hetzner** ist der Hostinganbieter des Referenzentwurfs, **Cloudflare** ein optionaler Dienst,
**Hugging Face** Modellhosting und **GitHub** der geplante Kollaborationsort.
**Claude Code / Anthropic** und **ChatGPT / OpenAI** sind assistierende Entwicklungs-/Dokumentationswerkzeuge,
keine notwendigen Laufzeitkomponenten. Daraus werden keine fremden Urheberrechte oder Partnerschaften erfunden.

## Forschung, nicht eingesetzte Backends

PS5LM würdigt [PS5SX2](https://github.com/Swordpdf/PS5SX2),
[ProsperoAI](https://github.com/blackbearreloaded/ProsperoAI) und
[PS5_Vulkan](https://github.com/mihawk-99/PS5_Vulkan) für Speicher-/GPU-Erkenntnisse.
Weitere frühere Forschungsquellen sind [PS5CEMU-HAR](https://github.com/premohq/PS5CEMU-HAR) und
[PS5 RetroArch](https://github.com/mihawk-99/PS5_RetroArch).
Keines dieser Projekte wird hier als bereits nachgewiesener OurArk-GPU- oder Simulationsbackend ausgegeben.

[ftpsrv](https://github.com/ps5-payload-dev/ftpsrv), [shsrv](https://github.com/ps5-payload-dev/shsrv) und
[klogsrv](https://github.com/ps5-payload-dev/klogsrv) sind optionale Diagnosekandidaten, keine Pflichtinstallation.
Payload Manager, WebKit Autoloader, vLLM, Ollama und Orchestrierungsframeworks werden erst dann
als verwendete Abhängigkeiten geführt, wenn Auswahl, Revision, Einbindung und Tests vorliegen.

Fehlende Anerkennung oder falsche Zuordnung bitte als Quellenkorrektur melden.
Siehe [THIRD_PARTY_NOTICES.md](THIRD_PARTY_NOTICES.md): Dieses Register ist keine vollständige Build-SBOM.
