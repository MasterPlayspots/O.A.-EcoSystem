# Target architecture

```text
Application / user / optional agent tool
              |
        API contract + policy
              |
   Gateway on an explicitly chosen host
              |
      verified backend adapter
              |
   one configured text inference worker
```

One device may carry several roles. A single host needs no tunnel.
In a home network, roles can be separated. Remote gateways and private tunnels are optional.
For the PS5, the experimental reference profile describes the path via a home-network relay,
reverse SSH, a VPS and an optional HTTPS edge. A PC does not need this console bootstrap.

## Roles

Client: makes requests and displays results. Gateway: auth, validated fields, limits and cancellation.
Relay: transport; no automatic inference process. Worker: computes a declared capability.
Coordinator: a later optional module for assigning whole independent tasks.
Storage/index service: a later separate capability, not an inherent part of the text worker.

## Contract and failures

First candidate: GET /health, GET /v1/models, POST /v1/chat/completions for text, optionally SSE.
Model aliases instead of private file paths; no freely selectable request upstream URLs.
Unsupported features are rejected. Missing usage remains unknown.
Header time, first visible text and full response duration are separate measurement points.
No later switch to HTTP 504 after a 200 stream has started; a cancellation stays incomplete.
After an unconfirmed worker cancellation, do not hastily reassign the single slot.

## Trust boundaries

Endpoint registration is an operator action, not a network scan and not hardware verification.
Do not present TLS/SSH as protection of an unencrypted last LAN hop.
Authentication at the gateway does not secure a directly reachable console administration.
Do not send confidential prompts into cloud/fallback paths unasked. No global
memory aggregation, no promise of direct use of other devices' GPUs through a tunnel.
