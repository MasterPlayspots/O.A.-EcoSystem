# Öffentliche Primärquellen

Abruf der Plattformdokumentation: 12. Oktober 2026. Software-/Hardwarequellen siehe zusätzlich [Credits](../CREDITS.md).

**S01 — [GitHub CLI: Repository anlegen](https://cli.github.com/manual/gh_repo_create)**. Syntax von --public, --source, --remote, --push; am 12.10.2026 gelesen.

**S02 — [GitHub CLI: Repository konfigurieren](https://cli.github.com/manual/gh_repo_edit)**. Issues, Discussions, Wiki, Defaultbranch und Mergeoptionen; aktuelle Flags vor Ausführung lokal prüfen.

**S03 — [GitHub: Rulesets](https://docs.github.com/en/repositories/configuring-branches-and-merges-in-your-repository/managing-rulesets/about-rulesets)**. Öffentliche Repositories unterstützen Rulesets; tatsächliche Rechte separat prüfen.

**S04 — [GitHub: CODEOWNERS](https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/customizing-your-repository/about-code-owners)**. Datei legt Zuständigkeit fest; erforderliche Reviews benötigen Plattformregeln.

**S05 — [GitHub: Private Vulnerability Reporting](https://docs.github.com/en/code-security/how-tos/report-and-fix-vulnerabilities/configure-vulnerability-reporting/configure-for-a-repository)**. Privaten Meldekanal für öffentliches Repository aktivieren und verifizieren.

**S06 — [GitHub Discussions](https://docs.github.com/en/discussions/quickstart)**. Kategorien, Moderation und Discussionstruktur.

**S07 — [GitHub Actions: sichere Nutzung](https://docs.github.com/en/actions/reference/security/secure-use)**. Minimale Rechte, gepinnte Actions, keine untrusted PRs auf Heimrunnern.

**S08 — [Claude Code: Projektanweisungen](https://code.claude.com/docs/en/memory)**. CLAUDE.md mit @AGENTS.md als dokumentierte Importlösung.

**S09 — [GitHub CLI: Anmeldung prüfen](https://cli.github.com/manual/gh_auth_status)**. Keine --show-token-Option im Arbeitsauftrag verwenden.

**S10 — [GitHub CLI: Repository lesen](https://cli.github.com/manual/gh_repo_view)**. Metadaten-/Sichtbarkeitsprüfung; nicht als unauthentifizierte Gegenprobe missverstehen.

**S11 — [GitHub CLI: Issue anlegen](https://cli.github.com/manual/gh_issue_create)**. Taskdateien und tatsächliche URLs; vor Anlage deduplizieren.

**S12 — [GitHub CLI: Discussion anlegen](https://cli.github.com/manual/gh_discussion_create)**. Versionabhängig verfügbare CLI prüfen; sonst dokumentierte API/UI nutzen.

**S13 — [GitHub: Lizenzierung](https://docs.github.com/articles/licensing-a-repository)**. Öffentliche Sichtbarkeit und Open-Source-Lizenz sind getrennte Eigenschaften.

**S14 — [GitHub: PR-Reviews](https://docs.github.com/en/pull-requests/reference/pull-request-reviews)**. Kommentare, Approvals und erforderliche Reviews auseinanderhalten.

Diese Quellen belegen Plattformfunktionen und dokumentierte Integrationen, nicht deren Aktivierung
im eigenen Repository. Hardware-/Upstreamangaben aus dem Credits-Register benötigen weiterhin
versionierte Nachweise für das jeweilige Geräteprofil.
