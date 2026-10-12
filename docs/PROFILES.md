# Device profiles and evidence status

**All of the following combinations are initially design candidates, not a current support matrix.**
Historical PS5 measurements are separate from an independent acceptance in this repository.

| Family / profile | Intended roles | What must be checked before support |
|---|---|---|
| Mock without inference hardware | Client, fixture, contract check | Simulated responses clearly marked; no real benchmarks |
| Linux x86-64 | Gateway/relay; inference with a suitable runtime | OS/CPU backend; specific GPU/driver combinations separately |
| macOS / Apple Silicon | Client/gateway/relay; suitable local inference | OS/runtime/backend, start/stop and memory profile |
| Windows | Client; further roles as a separate host profile | Paths, service management, CPU/GPU backend individually |
| Linux ARM / mini PC / NAS | Relay/gateway, possibly storage; inference only after testing | Operating system, package architecture, RAM, permissions and continuous operation |
| Mobile device / browser | Client in the first scope | Auth, stream display and usability; no promised mobile inference |
| Own VPS | Gateway/coordination; possibly its own worker | Provider-independent configuration and concrete resources |
| PS5 | Experimental inference worker | CFI/firmware/loader/PS5LM/model, LAN limits, restart and RAM |
| PS4 / other consoles | Research | No demonstrated runtime or performance status |

Rating levels: planned → fixture-verified → measured on own device → independently
reproduced. "Not supported" and "deprecated" are additional states. Every label needs
a profile version, test date, runtime and evidence; an old successful measurement is not today's operational check.

Roles are not assigned automatically from brand, nominal RAM or graphics performance.
Cloud/remote profiles are optional. No obligation to use a PS5, Hetzner, Cloudflare or an OurArk account.
