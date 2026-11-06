# Simulation timing log

Published results: **12/12 parts**, **24,000/24,000 trials**. Each part has 1,000 static trials and 1,000 trials at 100 ±3 mm/s, with grouping off.

Measured wall time uses `time.perf_counter()` around the simulation call. It includes geometry and symmetry preparation, process startup, physics, and writing raw results. Validation, archive compression, commits, and pushes take additional time. Each run uses 24 worker processes on a machine with 24 logical CPUs. Cached geometry can affect preparation time.

| Part | Static: 1,000 trials (s) | 100 ±3 mm/s: 1,000 trials (s) | Simulation total (s) |
| --- | ---: | ---: | ---: |
| Df1a | 177.640 | 132.430 | 310.070 |
| Dk1i | 250.266 | 189.489 | 439.755 |
| Dl1a | 156.680 | 110.346 | 267.026 |
| Kf1i | 861.055 | 323.513 | 1184.568 |
| Kk1a | 135.395 | 117.715 | 253.110 |
| Kl1i | 152.676 | 117.047 | 269.723 |
| Qf1i | 275.210 | 196.544 | 471.754 |
| Qk1a | 142.557 | 116.233 | 258.790 |
| Ql1i | 360.110 | 217.505 | 577.615 |
| Rf1a | 145.935 | 109.333 | 255.268 |
| Rk1a | 162.171 | 126.741 | 288.912 |
| Rl1a | 141.499 | 108.874 | 250.373 |

Sum of measured simulation durations: **4826.964 s (80.45 min)**.

The CSV and JSON include individual start times, measured durations, throughput, result-save times, push times, settings signatures, and result commits. UTC times are explicitly labelled. Replaced exact-speed and interrupted attempts remain in the event log; their durations are excluded from this table.

- [CSV timing log](run_timings.csv)
- [JSON timings and machine/software metadata](run_timings.json)
- [Timestamped run and publication events](event_log.jsonl)

README link: `[Simulation timing log](timing/run_timings.md)`.

## Separate geometry preparation

The following meshes and symmetry data were prepared before their simulation calls. Up to four preparation processes ran concurrently, with one native thread each. These durations are outside the simulation-call timings above and can overlap other work; they must not be added to derive end-to-end elapsed time. Concurrent preparation may also affect simulation throughput.

| Part | Preparation wall time (s) | Collision components |
| --- | ---: | ---: |
| Kk1a | 13.154 | 3 |
| Kl1i | 46.599 | 12 |
| Qf1i | 126.460 | 38 |
| Qk1a | 60.545 | 9 |
| Ql1i | 412.587 | 107 |
| Rf1a | 12.443 | 3 |
| Rk1a | 27.537 | 5 |
| Rl1a | 11.180 | 4 |

[Preparation start/end times and mesh checksums](geometry_preparation.json).

End-to-end batch elapsed time: **5216.984 s (86.95 min)**. This includes preparation, validation, compression, publishing, the settings change, and superseded/interrupted attempts.
