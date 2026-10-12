# Credits and traceable provenance

As of 12 October 2026. Acknowledgement is not a claim of direct collaboration, partnership or
endorsement of this project. The register distinguishes foundations, indirect components and research.
The actual composition of future software packages must be checked per release.

## Console and inference foundations

| Project / author | Contribution | Source state / licence note |
|---|---|---|
| [PS5LM — cobanov and contributors](https://github.com/cobanov/PS5LM) | Port, payload, model library, embedding of the inference | Historical reference release v0.1.1; GPL-3.0-or-later according to the [README](https://github.com/cobanov/PS5LM/blob/a7debaf060f8e1632ade04a841f4d89e2d2b51f9/README.md) |
| [llama.cpp / ggml](https://github.com/ggml-org/llama.cpp) | The actual model inference, server and GGUF processing | [MIT at the reference commit](https://github.com/ggml-org/llama.cpp/blob/552f18f912a32ea86edf82e2b76431cb7131538d/LICENSE) |
| [ps5-payload-dev / John Törnblom and contributors](https://github.com/ps5-payload-dev) | Open console tools | [SDK v0.43](https://github.com/ps5-payload-dev/sdk/tree/v0.43): GPLv3+ with BSD and file-specific exceptions |
| [ps5-payload-dev/elfldr](https://github.com/ps5-payload-dev/elfldr) | ELF loader | GPLv3+ according to the [README](https://github.com/ps5-payload-dev/elfldr#license); specific reproduction build still to be determined |
| [Relapse — ntfargo and contributors](https://github.com/ntfargo/Relapse-Exploit) | Console access for suitable authorised devices | [MIT](https://github.com/ntfargo/Relapse-Exploit/blob/main/LICENSE); specific reproduction commit still to be determined |
| [Qwen Team / Alibaba](https://huggingface.co/Qwen) | Original reference models | Model cards: [Qwen3.5 0.8B](https://huggingface.co/Qwen/Qwen3.5-0.8B), [2B](https://huggingface.co/Qwen/Qwen3.5-2B); assign the licence of the specific revision before obtaining it |
| [Unsloth AI and contributors](https://huggingface.co/unsloth) | Intended GGUF quantisations | [0.8B-GGUF](https://huggingface.co/unsloth/Qwen3.5-0.8B-GGUF), [2B-GGUF](https://huggingface.co/unsloth/Qwen3.5-2B-GGUF); this does not claim use of the Unsloth training library |
| Kevin Fröba / OurArk and future contributors | Project planning, documentation and future integration | The engine, access technique and weights are not presented as our own invention |

## Named Relapse credits

The [upstream README](https://github.com/ntfargo/Relapse-Exploit#credits) names:
**Sonic_Iso** (Kernel Exploit), **Jordy** (Webkit Exploit and Kernel Bug), **ntfargo** and **ufm42**
(Exploit Development) as well as **Dr. Yenyen** (Testing).
In addition, **TheFlow, SlidyBat, Flatz, cow, nhk, bollarz, Sleirsgoevy, EchoStretch and EarthOnion** are named.
This attribution applies to their upstream work, not to any claimed direct OurArk collaboration.

## Indirect libraries and data

| Component | Contribution / origin | Limit of review |
|---|---|---|
| [cpp-httplib — Yuji Hirose](https://github.com/yhirose/cpp-httplib) | HTTP library, MIT; [vendored header](https://github.com/ggml-org/llama.cpp/blob/552f18f912a32ea86edf82e2b76431cb7131538d/vendor/cpp-httplib/httplib.h) | Not bundled in this documentation start |
| [JSON for Modern C++ — Niels Lohmann](https://github.com/nlohmann/json) | JSON processing, MIT; [vendored header](https://github.com/ggml-org/llama.cpp/blob/552f18f912a32ea86edf82e2b76431cb7131538d/vendor/nlohmann/json.hpp) | Preserve specific file notices when adopted |
| [Mbed TLS](https://github.com/Mbed-TLS/mbedtls) | TLS; [3.6.7 licence](https://github.com/Mbed-TLS/mbedtls/blob/mbedtls-3.6.7/LICENSE): Apache-2.0 OR GPL-2.0-or-later | Document licence choice and build contents before own distribution |
| Mozilla/NSS and [curl / mk-ca-bundle](https://curl.se/docs/caextract.html) | CA data and conversion | Check data licence and notices separately; no blanket PS5LM licence assignment |
| [PS5Dev/PS5SDK](https://github.com/PS5Dev/PS5SDK), FreeBSD contributors | Indirect provenance documented in the SDK | Determine the files actually adopted and their exceptions |
| LLVM/Clang/LLD, CMake, Ninja, GNU Make | Optional tools for building it yourself | No SDK/toolchain rebuild as a prerequisite for every user |

## Hosts, network, platforms and tools

**[Node.js](https://github.com/nodejs/node)** as the intended host runtime,
**[OpenSSH/OpenBSD](https://github.com/openssh/openssh-portable)** for the reverse tunnel and
**[cloudflared](https://github.com/cloudflare/cloudflared)** for the optional tunnel profile.
The [cloudflared licence](https://github.com/cloudflare/cloudflared/blob/master/LICENSE) is to be distinguished from the
terms of use of the Cloudflare service.

Depending on the profile actually chosen, Python/Python Software Foundation, curl/libcurl,
Git, Bash, socat, systemd as well as Apple launchd/macOS services are added. A mention is not evidence of their
installation. Operating systems and their packages keep their own terms.

**Hetzner** is the hosting provider of the reference design, **Cloudflare** an optional service,
**Hugging Face** the model host and **GitHub** the planned place of collaboration.
**Claude Code / Anthropic** and **ChatGPT / OpenAI** are assisting development/documentation tools,
not required runtime components. No third-party copyrights or partnerships are invented from this.

## Research, backends not in use

PS5LM acknowledges [PS5SX2](https://github.com/Swordpdf/PS5SX2),
[ProsperoAI](https://github.com/blackbearreloaded/ProsperoAI) and
[PS5_Vulkan](https://github.com/mihawk-99/PS5_Vulkan) for memory/GPU insights.
Further earlier research sources are [PS5CEMU-HAR](https://github.com/premohq/PS5CEMU-HAR) and
[PS5 RetroArch](https://github.com/mihawk-99/PS5_RetroArch).
None of these projects is presented here as an already demonstrated OurArk GPU or simulation backend.

[ftpsrv](https://github.com/ps5-payload-dev/ftpsrv), [shsrv](https://github.com/ps5-payload-dev/shsrv) and
[klogsrv](https://github.com/ps5-payload-dev/klogsrv) are optional diagnostic candidates, not mandatory installations.
Payload Manager, WebKit Autoloader, vLLM, Ollama and orchestration frameworks are only listed
as dependencies in use once selection, revision, integration and tests are in place.

Please report missing acknowledgement or incorrect attribution as a source correction.
See [THIRD_PARTY_NOTICES.md](THIRD_PARTY_NOTICES.md): this register is not a complete build SBOM.
