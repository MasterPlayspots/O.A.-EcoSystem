# Licence and distribution boundaries

This start contains our own documentation, contribution templates and publicly linked sources.
No third-party source packages, model weights, ELF payloads, SDKs, firmware or font files are shipped.
[MIT](LICENSE) applies to the project's own files of this start, not to linked third-party projects.
[CREDITS.md](CREDITS.md) is an acknowledgement register, not a relicensing and not a final legal review.

Before any later adoption of a file, source, full commit, author/copyright information,
licence, modifications and scope of distribution must be documented. Required licence and notice texts
are then kept together with the respective file. GPL files do not receive a new MIT header.
For any own binary distribution, the appropriate Corresponding Source path in particular must be clarified.

References: [PS5LM GPLv3](https://github.com/cobanov/PS5LM/blob/a7debaf060f8e1632ade04a841f4d89e2d2b51f9/LICENSE),
[llama.cpp MIT](https://github.com/ggml-org/llama.cpp/blob/552f18f912a32ea86edf82e2b76431cb7131538d/LICENSE),
[SDK exceptions](https://github.com/ps5-payload-dev/sdk/blob/v0.43/README.md),
[Mbed TLS dual licence](https://github.com/Mbed-TLS/mbedtls/blob/mbedtls-3.6.7/LICENSE).

Models require their own artefact manifest: model author, quantiser, exact file,
source revision, hash, size, model card and specific licence. Models are not shipped.

Still open: the complete transitive build set, the exact loader/bootstrap revision,
CA data notices and the assignment of implementation files exported in the future.
Completeness is checked against the actual software release, not derived from this list of links.
