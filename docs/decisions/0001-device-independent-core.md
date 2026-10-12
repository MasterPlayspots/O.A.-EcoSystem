# ADR-0001 — Geräteunabhängiger Kern, getrennte Profile

Datum: 12.10.2026. Richtungsentscheidung des Auftraggebers: Dachname **O.A.-EcoSystem**.
Konkrete technische Ausgestaltung: Vorschlag zur Gegenprüfung.

O.A.-EcoSystem ersetzt den geplanten Repositorynamen ourark-compute. Die bisherige Forschung
wird nicht verworfen: PS5 & Hetzner bleibt ein eigenes experimentelles Profil.

Kern, Hostplattform, Backend und Transport werden getrennt. Kleine Rollen können auf einem Rechner
zusammenfallen; andere Nutzer verteilen sie auf ihre Geräte. Kompatibilität folgt aus validierten
Fähigkeiten, nicht aus der Herstellermarke. Das erste Runtimeziel bleibt Textinferenz mit einem Worker.

Alternative: PS5-festes Gateway als Dachprodukt. Verworfen als Zielstruktur, weil das unnötige
Konsolen-/Providerpflichten für Nutzer ohne PS5 erzeugen würde.

Nicht beschlossen: universeller Treiber, automatische Geräteübernahme, verteilter RAM,
selbsttätiges Modellrouting oder funktionsfähige GPU-/PS4-/Simulationsmodule.
