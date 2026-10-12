# Masterplan — device-independent entry

## Goal

A user employs suitable roles on the devices they already own. The planned
integration layer connects applications with explicitly configured compute endpoints.
Device profiles complement the core; they do not define it. PS5 & Hetzner remains a historical
research basis and a future reproduction path, not a mandatory component.

## First achievable sub-goal

First community documentation online, then the capability/API contract, then a hardware-free mock.
After that a generic HTTP text worker, client-side examples and a verified single-host path.
Then accept the known PS5 route step by step. The first runtime scope remains one operator,
one selected worker, one concurrently admitted request. No scheduler is needed for that.

## Adapters instead of a universal installer

A device profile describes OS/architecture/firmware, runtime/backend, model provenance, permitted
roles, installed and demonstrated functions, and the test date. An adapter merely translates
between the verified backend contract and the core. No automatic installation of missing drivers,
no hardware takeover and no arbitrary program execution from community profiles.

The configuring user decides: locally, in the LAN or via their own remote access.
All accounts, domains and keys belong to them. A local policy prevents unrequested
cloud fallback or sending data to other operators.

## Extensions

Multiple devices, a job queue, model routing and failover only follow after the definition of
identity, leases, deadlines, cancellation, idempotency and privacy. Rendering, simulation, audio,
embeddings, GPU, MoE and local mobile inference are separate capabilities with their own tests.
The project is open to these paths but does not claim them as already available.

## Publication

The first public state contains new documentation of our own, profiles as drafts and reviews.
Runtime code will later be prepared selectively on its own branch; no private monorepo
and none of its Git history will be published. Every actual hardware approval needs evidence.
An unknown absolute RAM capacity does not block an honestly limited documentation opening.

See [Roadmap](ROADMAP.md), [Profiles](PROFILES.md), [Security policy](../SECURITY.md)
and [Credits](../CREDITS.md). Do not derive any operational action from this plan.
