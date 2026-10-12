# Security

## Status

Documentation/community bootstrap; no supported runtime version yet.
The planned operation connects heterogeneous, partly experimental devices.
Do not test other people's systems and do not derive homebrew, firmware or model actions from an issue.

## Reporting confidentially

GitHub's private vulnerability reporting is enabled for this repository (last checked
on 12 Oct 2026). Please report vulnerabilities via Security → Report a vulnerability:
<https://github.com/MasterPlayspots/O.A.-EcoSystem/security/advisories/new>.
The menu entry is publicly visible; submitting requires a signed-in GitHub account.
This file itself enables nothing — the repository setting is what counts. Do not write secrets or exploitable details in public issues.
We do not promise a fixed response time as long as no staffed on-call process has been set up.

## Security boundaries

No hardware/production access in public CI. Do not run untrusted PRs on personal machines
or on a self-hosted runner with home network access. In the initial start, only document/schema checks
on GitHub-hosted standard runners, minimal permissions and no operator secrets.
Private operating documents are not a public bug report. An accidentally published secret
must be treated as compromised; escalation and rotation are coordinated with the owner —
do not just delete the text and declare the incident closed.
