# Capabilities and device contract — draft

A device type is not a capability. Operating system, architecture, firmware, runtime, backend,
model, state and the contract test actually executed decide together.

| Contract field | Meaning |
|---|---|
| node_id / profile_id | Local alias and profile, not a serial number or public IP |
| roles | client, relay, gateway, inference_worker; later roles separately |
| platform | OS, architecture, firmware if needed; unknown explicitly left open |
| runtime / backend | Name and fixed version; GPU only with runtime evidence |
| capabilities | e.g. text_chat, streaming; true/false/unknown with evidence |
| limits | actually known context/token/parallelism limits; unknown is not zero performance |
| memory | file size, mapping, residency, peak, lock, buffers kept separate |
| evidence | type, source, time, software/model version and scope of the check |
| policy | permitted data class, network boundary, job/energy budget, no automatic cloud fallback |
| availability | observed readiness plus freshness, not a permanent online=true |

## Planned selection flow

The user chooses role and profile → reads the prerequisites → explicitly registers the endpoint →
checks the local configuration → separately approves a limited network check → approves a
small functional test → accepts the demonstrated capabilities. Without a successful test, no "supported" label.

A later router assigns jobs only after a capability and policy check. Missing data
leads to an explainable rejection, not to a guessed resource figure.
In the first runtime scope exactly one worker is selected; no automatic routing is implemented.
