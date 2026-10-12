# Communication structure — O.A.-EcoSystem

## Leading places

| Place | Content | Do not put here |
|---|---|---|
| README + docs/PROJECT_INDEX.md | Entry point, actual status, link to the next task | Private operator information |
| GitHub Discussions | Questions, ideas/RFCs, device exchange and progress | Secrets, confidential vulnerabilities, binding decisions without adoption |
| GitHub Issues | Scoped work, bugs, acceptance and blockers | Unstructured catch-all requests to "build everything" |
| Pull requests | Concrete changes, review, test evidence | Unreviewed private sources and binary packages |
| docs/decisions/ | Accepted decisions with rationale and counter-arguments | Chat opinions disguised as decisions |
| Private security channel | Non-public clarification of vulnerabilities | Public detailed discussion before coordinated disclosure |
| Internal Drive | Originals, raw evidence, operator plans, approvals, dated export snapshots | Keeping publicly required specifications private only |

Discord, messengers or other community channels are optional. They are neither created
nor connected in this start. Decisions made there must be brought back, redacted and with consent, into an issue/ADR.

## Discussions

Intended categories: **Announcements** (maintainers), **Q&A** (questions and getting started),
**Ideas** (ideas and RFCs), **Device Reports**, **Show and tell**. Reuse existing categories;
create new categories according to the rights/API actually available. Do not guess category IDs.
Status on 12 Oct 2026: Announcements, Q&A, Ideas, Show and tell, General and Polls exist;
**Device Reports is proposed and does not exist yet** (owner task in the GitHub UI).
Two threads at the start: "start here / get involved" and "which devices and roles would you like to contribute?".
Private vulnerability reports are not a discussion topic.

## Task flow

Idea → concrete task ID → issue → scope/acceptance criteria → branch/PR → review → merge by an
authorised maintainer → update evidence/ADR/profile status. The GitHub issue number is only known after
actual creation. For example, OA-REVIEW-01 is a task ID, not issue #1.
Before creating anything new, search by task ID and title, including closed issues.

Every issue has goal, non-goals, delivery, acceptance tests, dependencies, risk and sources.
Small PRs reference the issue and state tests run/not run. No automatic merges.
Labels: type:docs/review/feature/research/bug; area:core/profiles/security/community;
priority:p0/p1/p2; status:triage/ready/in-progress/review/blocked. Done is a closed, accepted issue.
"good first issue" only on small, genuinely accessible tasks; do not label permission/device work that way.

## Roles and approvals

Kevin Fröba prioritises, moderates and decides on external releases and maintainer access.
ChatGPT consolidates evidence and handoffs. Claude reviews and implements the specifically requested scope.
Community contributions start via fork/PR. Nobody automatically receives write/admin access.
A review by another model under the same GitHub account does not replace an independent human approval.
If a required reviewer is missing, the PR stays open; do not quietly weaken the rules.

## Rhythm without invented automation

Proposal: a short weekly maintainer status; event-based updates after an accepted PR,
a profile acceptance or an important blocker. This is not configured automation and not a support SLA.
After every agent session: head, tasks, findings, tests, actions/non-actions, blockers, next request.
Report back on the issue/PR in redacted public form; private operating details go into the internal log.

## Language and conduct

Maintained public project material — README, documentation, contribution/conduct/security rules,
agent instructions, templates and project-maintained GitHub entry texts — and new project-authored updates
are written in English. Internal coordination and historical originals may remain in German;
originals and historical evidence are not retroactively translated or rewritten.
Community members are not excluded solely for using another language.
Technical identifiers stay consistent. Criticise factually, credit upstreams,
make no unverified security, performance, sustainability or compatibility promises.
