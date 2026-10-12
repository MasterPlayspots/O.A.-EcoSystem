# O.A.-EcoSystem

**Connect the devices you already own in a meaningful way: suitable tasks, your own infrastructure, verifiable results.**

**Phase: community bootstrap / planning and documentation stage.**
This repository is a place to contribute. It does not yet contain an installable inference core,
tested automatic device discovery or any general hardware approval.
The repository has been public since 12 Oct 2026. Current task, review and merge status
lives in the linked issues and pull requests, not in this overview.

## What we are building

A modular integration layer guided by the **demonstrated capabilities** of the devices people
already have. A machine can be a client, gateway, relay or inference worker;
not every device has to, or can, take on every role. The same applies to later specialised workers.
PS5 & Hetzner is our historical experimental reference profile, not the mandatory base system.

An OurArk account, your own PS5, a particular hosting provider or permanent cloud access
should not be prerequisites for the general entry path. Other runtimes and devices each require
adapter, licence, security and functional tests. Model weights and hardware limits stay on the respective node;
a network tunnel does not add up the memory or GPUs of different devices.

## Read first and contribute

[Project index](docs/PROJECT_INDEX.md) · [Plan](docs/MASTERPLAN.md) · [Device profiles](docs/PROFILES.md) ·
[Architecture](docs/ARCHITECTURE.md) · [Roadmap](docs/ROADMAP.md) · [Communication](docs/COMMUNICATION.md)

Concrete work belongs in issues, changes in small pull requests, questions/ideas in Discussions —
entry point: [Start here / get involved (discussion #14)](https://github.com/MasterPlayspots/O.A.-EcoSystem/discussions/14). Documentation, API contracts, source review, mock tests and translations
make contributing possible without a console. The [contribution guidelines](CONTRIBUTING.md) and the [review brief](docs/CLAUDE_REVIEW.md)
explain how to get started.

## Planned entry paths

| Profile | Purpose | Status in this repository |
|---|---|---|
| Mock | Check interfaces without weights, cloud or an inference device | Planned |
| One local host | Client, gateway and a suitable worker on one machine | Planned; runtime to be validated separately |
| Home network | One or more of your own devices via explicit configuration | Planned; initially exactly one selected worker |
| Private remote access | Your own gateway and controlled transport | Planned; no automatic cloud provisioning |
| PS5 reference | Reproduce the documented PS5–relay–VPS path | Historical experiment, not yet re-accepted here |

GPU, MoE, PS4, freely executable jobs, multi-tenant operation and simulation are not demonstrated capabilities
of our start. NAS, ARM mini PCs, Windows, macOS and Linux likewise only receive
matching support statements after concrete tests. A mobile device starts as a client; local mobile inference is a separate research task.

## Transparency and credits

We are building integration and reproducibility, not a new LLM engine. The PS5 reference experiment
is based on **PS5LM / cobanov**, **llama.cpp / ggml**, the work of **Relapse** and
**ps5-payload-dev / John Törnblom**, as well as **Qwen** models in **Unsloth** GGUF quantisations.
Further direct, indirect and optional contributions are listed in [CREDITS.md](CREDITS.md).

Our own bootstrap documents: [MIT](LICENSE). Third-party projects keep their licences;
[THIRD_PARTY_NOTICES.md](THIRD_PARTY_NOTICES.md) is not a blanket approval of third-party binaries.
No firmware, weights, payload/SDK bundles, vendor fonts or operator secrets are included.

Project lead: **Kevin Fröba**. Independent community project; no partnership commitment
or official support by the manufacturers/upstreams mentioned. [Security reports](SECURITY.md).
