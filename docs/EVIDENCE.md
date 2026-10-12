# Evidence, measurement reports and the first RAM investigation

## Types of evidence

Own measurement (with the person who ran it/report back), repository check, manufacturer statement,
third-party project measurement, hypothesis and unknown are kept separate.
Reading an old report today does not renew its measurement date. A CI test with a fixture does not measure a PS5.
HTTP 200 proves neither visible text nor the hardware or the backend. New capabilities are only marked after acceptance.

## Minimal redacted report

Source; measurement time in UTC and time zone; device family/CFI and firmware; host/runtime/model revision;
hash and hash provenance; profile/route without a private host; parameters including thinking, context and limit;
cache state; actual token count; finish reason; first visible text; header time; total time;
server times separately; unit and measurement point; errors and final state.

Do not ask for secrets, serial numbers, host IDs, private prompts or response content.
Missing values are null with a reason, not 0 performance or 0 bytes.
Durations per measurement point with a monotonic clock, not a difference of unsynchronised host timestamps.
Keep raw data limited and redacted with a checksum. Do not market small samples as sustained load/p95.

## RAM-01: observe first, do not allocate until it crashes

The goal is initially a stable working profile of a defined inference run, not a claimed absolute upper limit.
First check existing logs and supported counters of the actual inference process.
A new diagnostic payload is an intervention and needs a separate approval; its name does not prove passivity.
Do not assume Linux/BSD counters on the PS5 without confirmed platform semantics.

Separate quantities: model file bytes, mapping, current residency/RSS, peak, requested/successful locked bytes,
KV/recurrent state buffers, working buffers, runtime overhead, fault/I/O deltas and system pressure.
Do not double-count overlapping memory shares. An mlock request is not success.
Minor faults do not prove disk access; major faults/file page-ins are not automatically swap.

Only after an instrumentation review and operational approval: a small 0.8B profile, one model,
short sequential requests, limited telemetry and idle/resume observation.
Define the measurement budget, sampling rate, return path and stop rules beforehand; do not raise priority/threads/file limits.
In case of warnings, API loss, UI blocking or budget overrun, no further jobs.
2B and context variations follow separately. No full-hash/full-page-touch action immediately before
residency attempts as a supposedly state-neutral measurement.

Third-party measurements from [PS5LM CONSOLE.md](https://github.com/cobanov/PS5LM/blob/4173291e0554ff60945f3ed3b0a2d9dcc5190168/docs/CONSOLE.md)
belong to its test device, not to every console. The limits described there are not our own safety budgets.
No new device check was carried out by writing this document.


## Placement in the new umbrella project

The PS5-specific RAM investigation is a single profile. Other devices need
their own corresponding counters and tests; do not transfer API, operating-system or resource semantics.
The general evidence rules apply independently of any particular device.
