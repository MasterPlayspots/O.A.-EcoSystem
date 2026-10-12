# Lizenz- und Distributionsgrenzen

Dieser Start enthält eigene Dokumentation, Beitragsvorlagen und öffentlich verlinkte Quellen.
Es werden keine fremden Quellcodepakete, Modellgewichte, ELF-Payloads, SDKs, Firmware oder Fontdateien ausgeliefert.
[MIT](LICENSE) gilt für die eigenen Dateien dieses Starts, nicht für verlinkte Drittprojekte.
[CREDITS.md](CREDITS.md) ist ein Anerkennungsregister, keine Umlizenzierung und keine abschließende Rechtsprüfung.

Vor der späteren Übernahme einer Datei müssen Quelle, vollständiger Commit, Autor-/Copyrightangaben,
Lizenz, Modifikationen und Verteilungsumfang dokumentiert werden. Erforderliche Lizenz- und Notice-Texte
werden dann zusammen mit der jeweiligen Datei erhalten. GPL-Dateien erhalten keinen neuen MIT-Kopf.
Bei eigener Binärverteilung ist insbesondere der passende Corresponding-Source-Weg zu klären.

Referenzen: [PS5LM GPLv3](https://github.com/cobanov/PS5LM/blob/a7debaf060f8e1632ade04a841f4d89e2d2b51f9/LICENSE),
[llama.cpp MIT](https://github.com/ggml-org/llama.cpp/blob/552f18f912a32ea86edf82e2b76431cb7131538d/LICENSE),
[SDK-Ausnahmen](https://github.com/ps5-payload-dev/sdk/blob/v0.43/README.md),
[Mbed-TLS-Duallizenz](https://github.com/Mbed-TLS/mbedtls/blob/mbedtls-3.6.7/LICENSE).

Modelle benötigen ein eigenes Artefaktmanifest: Modellurheber, Quantisierer, exakte Datei,
Herkunftsrevision, Hash, Größe, Modellkarte und konkrete Lizenz. Modelle werden nicht mitgeliefert.

Offen bleiben die vollständige transitive Buildmenge, die genaue Loader-/Bootstrap-Revision,
CA-Daten-Notices und die Zuordnung künftig exportierter Implementierungsdateien.
Die Vollständigkeit wird am tatsächlichen Software-Release geprüft, nicht aus dieser Linkliste abgeleitet.
