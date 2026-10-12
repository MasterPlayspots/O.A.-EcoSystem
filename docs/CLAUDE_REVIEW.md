# Erster fachlicher Claude-Review

Untersuche README, MASTERPLAN, ARCHITECTURE, CAPABILITIES, PROFILES, ROADMAP,
COMMUNICATION und Credits. Nutze nur tatsächlich zugängliche Quellen. Ein öffentlicher
Reviewer benötigt keine privaten Drive-Dokumente.

Prüffragen: Ist der Kern geräteunabhängig? Sind CPU/GPU/OS/Firmware/Runtime und Policy sauber
getrennt? Kann man ohne PS5 mitarbeiten? Welche Profile sind nur geplant? Welche Tests fehlen
für Single-Worker-Abbruch, SSE, Limits, sichere Modellaliase und Auth? Sind Herkunft und
Fremdlizenzen sichtbar? Welche Online-Einstellungen sind tatsächlich aktiv?

Liefere Befunde mit ID, Schwere, Datei/Zeile/Commit, Quelle, Wirkung, Verbesserung und Abnahmetest.
P0 blockiert die betroffene Freigabe; P1 muss vor der entsprechenden Fähigkeit geschlossen sein;
P2 bleibt sichtbar offen. Positive Aussagen benötigen ebenfalls Nachweise.

Ohne eigenen Implementierungsauftrag keine Runtimeänderung, Geräteaktion oder Deployment.
Der Review kann als Issuekommentar oder auf eigenem Reviewbranch/PR abgelegt werden;
keinen selbst erzeugten PR selbst als unabhängig geprüft darstellen oder automatisch mergen.
