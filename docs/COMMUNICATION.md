# Kommunikationsstruktur — O.A.-EcoSystem

## Führende Orte

| Ort | Inhalt | Nicht dort ablegen |
|---|---|---|
| README + docs/PROJECT_INDEX.md | Einstieg, echter Status, Link zu nächster Aufgabe | Private Betreiberinformationen |
| GitHub Discussions | Fragen, Ideen/RFCs, Geräteaustausch und Fortschritt | Secrets, vertrauliche Schwachstellen, verbindliche Entscheidungen ohne Übernahme |
| GitHub Issues | Abgrenzbare Arbeit, Fehler, Abnahme und Blocker | Unstrukturierte Sammelaufträge „alles bauen“ |
| Pull Requests | Konkrete Änderungen, Review, Testnachweise | Ungeprüfte private Quellen und Binärpakete |
| docs/decisions/ | Akzeptierte Entscheidungen mit Begründung und Gegenargumenten | Chatmeinungen als beschlossen tarnen |
| Privater Security-Kanal | Nicht öffentliche Schwachstellenklärung | Öffentliche Detaildiskussion vor koordinierter Meldung |
| Internes Drive | Originale, Rohbelege, Betreiberpläne, Freigaben, datierte Exportsnapshots | Öffentlich erforderliche Spezifikation ausschließlich privat halten |

Discord, Messenger oder andere Communitykanäle sind optional. Sie werden in diesem Start weder angelegt
noch verbunden. Dortige Entscheidungen müssen mit Zustimmung redigiert in Issue/ADR zurückgeführt werden.

## Discussions

Vorgesehene Kategorien: **Ankündigungen** (Maintainer), **Fragen & Einstieg** (Q&A),
**Ideen & RFCs**, **Geräteberichte**, **Zeig deinen Aufbau**. Vorhandene Kategorien wiederverwenden;
neue Kategorien anhand der tatsächlich vorhandenen Rechte/API anlegen. Keine Kategorie-IDs erraten.
Zum Start zwei Threads: „Hier anfangen / Mitmachen“ und „Welche Geräte und Rollen möchtet ihr einbringen?“.
Private Schwachstellenmeldung ist kein Discussionsthema.

## Aufgabenfluss

Idee → konkrete Task-ID → Issue → Scope/Abnahmekriterien → Branch/PR → Review → Merge durch
berechtigten Maintainer → Nachweis/ADR/Profilstatus aktualisieren. Die GitHub-Issuenummer ist erst nach
tatsächlicher Anlage bekannt. Beispielsweise ist OA-REVIEW-01 eine Task-ID, nicht Issue #1.
Vor jeder neuen Anlage nach Task-ID und Titel suchen, auch geschlossene Issues beachten.

Jedes Issue hat Ziel, Nicht-Ziele, Auslieferung, Abnahmetests, Abhängigkeiten, Risiko und Quellen.
Kleine PRs referenzieren das Issue und nennen ausgeführte/nicht ausgeführte Tests. Keine automatischen Merges.
Kennzeichnung: type:docs/review/feature/research/bug; area:core/profiles/security/community;
priority:p0/p1/p2; status:triage/ready/in-progress/review/blocked. Done ist ein geschlossenes abgenommenes Issue.
„good first issue“ nur auf kleine tatsächlich zugängliche Aufgaben; Rechte-/Gerätearbeit nicht so etikettieren.

## Rollen und Freigaben

Kevin Fröba priorisiert, moderiert und entscheidet über externe Freigaben und Maintainerzugänge.
ChatGPT konsolidiert Evidenz und Übergaben. Claude prüft und implementiert den konkret beauftragten Umfang.
Communitybeiträge beginnen per Fork/PR. Niemand erhält automatisch Schreib-/Adminzugriff.
Ein Review eines anderen Modells unter demselben GitHub-Konto ersetzt kein unabhängiges menschliches Approval.
Fehlt ein erforderlicher Reviewer, bleibt der PR offen; Regeln nicht still schwächen.

## Rhythmus ohne erfundene Automatisierung

Vorschlag: wöchentlicher kurzer Maintainerstatus; ereignisbezogene Updates nach akzeptiertem PR,
Profilabnahme oder wichtigem Blocker. Dies ist keine eingerichtete Automation und kein Support-SLA.
Nach jeder Agentensitzung: Head, Tasks, Befunde, Tests, Aktionen/Nicht-Aktionen, Blocker, nächster Auftrag.
Rücklauf am Issue/PR öffentlich redigiert; private Betriebsdetails im internen Protokoll.

## Sprache und Umgang

Erststart Deutsch; englische Beiträge willkommen, englischer Einstieg als eigene Aufgabe.
Technische Kennungen bleiben konsistent. Sachlich kritisieren, Upstreams würdigen,
keine ungeprüften Sicherheits-, Leistungs-, Nachhaltigkeits- oder Kompatibilitätsversprechen.
