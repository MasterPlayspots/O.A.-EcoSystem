# Repository administration — target configuration, not proof of activation

After the first redacted bootstrap commit, actually read the settings and document them in the result
report. A file named CODEOWNERS/SECURITY.md is not a platform configuration.

| Area | Target |
|---|---|
| Owner / name | MasterPlayspots / O.A.-EcoSystem |
| Visibility | Public; only this new repo, no visibility change of other repos |
| Default branch | main |
| Community | Issues and Discussions on; no separate wiki as a second documentation source |
| Merge | No auto-merge; after the bootstrap only PRs |
| main | No force-push, no deletion, resolve conversations, 1 required approval |
| Checks | Only configure check names that actually exist and succeed as required |
| Security | Enable/verify private vulnerability reporting, check secret scanning/push protection |
| Actions | No operator secrets, read-only contents, no privileged PR checkout, no home runners |
| Costs | Do not create paid add-ons, large runners, cloud accounts or domains |

If a second reviewer is missing, your own changes stay open in PRs. That is no reason to give
 yourself an independent approval with the same account or to switch off protection. Report limitations
 of permissions/API precisely; name the owner's UI step as an open item.

For the start, locally checked documents and JSON are sufficient. A new docs/schema CI is its own
 small PR; no green badge and no runtime test promise before an actual CI run.
Community announcement only after an anonymous view and a check of the contribution/reporting paths.
