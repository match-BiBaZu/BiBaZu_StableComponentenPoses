# Simulation timing log

Published results: **9/12 parts**, **180,000/240,000 trials**. Each part has 10,000 static trials and 10,000 trials at 100 ±3 mm/s, with grouping off.

Measured wall time uses `time.perf_counter()` around the simulation call. It includes geometry and symmetry preparation, process startup, physics, and writing raw results. Validation, archive compression, commits, and pushes take additional time. Each run uses 24 worker processes on a machine with 24 logical CPUs. Cached geometry can affect preparation time.

| Part | Static: 10,000 trials (s) | 100 ±3 mm/s: 10,000 trials (s) | Simulation total (s) |
| --- | ---: | ---: | ---: |
| Df1a | 1757.604 | 1313.984 | 3071.588 |
| Dk1i | 2480.068 | 1846.479 | 4326.547 |
| Dl1a | 1390.716 | 1036.027 | 2426.743 |
| Kf1i | 5809.434 | 3827.321 | 9636.755 |
| Kk1a | 1285.232 | 1012.153 | 2297.385 |
| Kl1i | 1515.157 | 1154.316 | 2669.473 |
| Qf1i | 3098.354 | 2071.705 | 5170.059 |
| Qk1a | 1319.863 | 1038.933 | 2358.796 |
| Ql1i | 3674.549 | 2511.958 | 6186.507 |

Sum of measured simulation durations: **38143.853 s (635.73 min)**.

The CSV and JSON include individual start times, measured durations, throughput, result-save times, push times, settings signatures, and result commits. UTC times are explicitly labelled.

- [CSV timing log](run_timings.csv)
- [JSON timings and machine/software metadata](run_timings.json)
- [Timestamped run and publication events](event_log.jsonl)

README link: `[Simulation timing log](timing/20261107_10000/run_timings.md)`.
