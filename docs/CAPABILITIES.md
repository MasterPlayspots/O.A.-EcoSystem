# Fähigkeiten und Gerätevertrag — Entwurf

Ein Gerätetyp ist keine Fähigkeit. Betriebssystem, Architektur, Firmware, Runtime, Backend,
Modell, Zustand und ausgeführter Kontrakttest entscheiden zusammen.

| Vertragsfeld | Bedeutung |
|---|---|
| node_id / profile_id | Lokaler Alias und Profil, keine Seriennummer oder öffentliche IP |
| roles | client, relay, gateway, inference_worker; spätere Rollen separat |
| platform | OS, Architektur, bei Bedarf Firmware; unbekannt ausdrücklich offen |
| runtime / backend | Name und feste Version; GPU nur mit Laufzeitnachweis |
| capabilities | z. B. text_chat, streaming; wahr/falsch/unbekannt mit Evidenz |
| limits | tatsächlich bekannte Kontext-/Token-/Parallelgrenzen; unknown nicht null Leistung |
| memory | Dateigröße, Mapping, Residency, Peak, Lock, Buffer getrennt |
| evidence | Art, Quelle, Zeitpunkt, Software-/Modellstand und Prüfumfang |
| policy | erlaubte Datenklasse, Netzwerkgrenze, Auftrags-/Energiebudget, kein automatisches Cloud-Fallback |
| availability | beobachtete Bereitschaft plus Aktualität, nicht ewiges online=true |

## Geplanter Auswahlablauf

Anwender wählt Rolle und Profil → liest Voraussetzungen → registriert ausdrücklich den Endpunkt →
prüft lokale Konfiguration → genehmigt separat eine begrenzte Netzwerkprüfung → genehmigt einen
kleinen Funktionstest → akzeptiert die belegten Fähigkeiten. Ohne erfolgreichen Test kein Label „unterstützt“.

Ein späterer Router weist Jobs erst nach Fähigkeits- und Policyprüfung zu. Fehlende Daten
führen zu einer erklärbaren Ablehnung, nicht zu einer geratenen Ressourcenzahl.
Beim ersten Runtimeumfang ist genau ein Worker ausgewählt; kein automatisches Routing implementiert.
