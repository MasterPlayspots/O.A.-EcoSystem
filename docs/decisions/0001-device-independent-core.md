# ADR-0001 — Device-independent core, separate profiles

Date: 12 Oct 2026. Direction decision by the project owner: umbrella name **O.A.-EcoSystem**.
Concrete technical design: proposal for cross-checking.

O.A.-EcoSystem replaces the planned repository name ourark-compute. The previous research
is not discarded: PS5 & Hetzner remains a separate experimental profile.

Core, host platform, backend and transport are separated. Small roles can coincide on one machine;
other users distribute them across their devices. Compatibility follows from validated
capabilities, not from the manufacturer's brand. The first runtime goal remains text inference with one worker.

Alternative: a PS5-bound gateway as the umbrella product. Rejected as the target structure because it would create unnecessary
console/provider obligations for users without a PS5.

Not decided: a universal driver, automatic device takeover, distributed RAM,
autonomous model routing or working GPU/PS4/simulation modules.
