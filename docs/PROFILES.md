# Geräteprofile und Nachweisstatus

**Alle folgenden Kombinationen sind zunächst Designkandidaten, keine aktuelle Supportmatrix.**
Historische PS5-Messungen sind getrennt von einer unabhängigen Abnahme dieses Repositories.

| Familie / Profil | Vorgesehene Rollen | Was vor Support zu prüfen ist |
|---|---|---|
| Mock ohne Inferenzhardware | Client, Fixture, Vertragsprüfung | Simulierte Antworten eindeutig; keine echten Benchmarks |
| Linux x86-64 | Gateway/Relay; Inferenz bei passender Runtime | OS/CPU-Backend, konkrete GPU-/Treiberkombinationen separat |
| macOS / Apple Silicon | Client/Gateway/Relay; passende lokale Inferenz | OS/Runtime/Backend, Start-/Stopp- und Speicherprofil |
| Windows | Client; weitere Rollen als eigenes Hostprofil | Pfade, Dienstverwaltung, CPU/GPU-Backend einzeln |
| Linux ARM / Mini-PC / NAS | Relay/Gateway, ggf. Speicher; Inferenz nur nach Test | Betriebssystem, Paketarchitektur, RAM, Rechte und Dauerbetrieb |
| Mobilgerät / Browser | Client im ersten Umfang | Auth, Streamdarstellung und Bedienung; keine zugesagte mobile Inferenz |
| Eigener VPS | Gateway/Koordination; ggf. eigener Worker | Anbieterunabhängige Konfiguration und konkrete Ressourcen |
| PS5 | Experimenteller Inferenzworker | CFI/Firmware/Loader/PS5LM/Modell, LAN-Grenzen, Wiederanlauf und RAM |
| PS4 / andere Konsolen | Forschung | Kein nachgewiesener Runtime- oder Leistungsstatus |

Bewertungsstufen: geplant → Fixture-verifiziert → auf eigenem Gerät gemessen → unabhängig
nachgebaut. „Nicht unterstützt“ und „veraltet“ sind zusätzliche Zustände. Jedes Label benötigt
Profilversion, Testdatum, Runtime und Evidenz; eine alte erfolgreiche Messung ist kein heutiger Betriebscheck.

Rollen werden nicht aus Marke, nominellem RAM oder Grafikleistung automatisch vergeben.
Cloud-/Remoteprofile sind optional. Keine Pflicht zu PS5, Hetzner, Cloudflare oder einem OurArk-Konto.
