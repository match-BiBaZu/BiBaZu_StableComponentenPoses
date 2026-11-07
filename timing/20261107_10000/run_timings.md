# Simulation timing log

Published results: **2/12 parts**, **40,000/240,000 trials**. Each part has 10,000 static trials and 10,000 trials at 100 ±3 mm/s, with grouping off.

Measured wall time uses `time.perf_counter()` around the simulation call. It includes geometry and symmetry preparation, process startup, physics, and writing raw results. Validation, archive compression, commits, and pushes take additional time. Each run uses 24 worker processes on a machine with 24 logical CPUs. Cached geometry can affect preparation time.

| Part | Static: 10,000 trials (s) | 100 ±3 mm/s: 10,000 trials (s) | Simulation total (s) |
| --- | ---: | ---: | ---: |
| Df1a | 1757.604 | 1313.984 | 3071.588 |
| Dk1i | 2480.068 | 1846.479 | 4326.547 |

Sum of measured simulation durations: **7398.135 s (123.30 min)**.

The CSV and JSON include individual start times, measured durations, throughput, result-save times, push times, settings signatures, and result commits. UTC times are explicitly labelled.

- [CSV timing log](run_timings.csv)
- [JSON timings and machine/software metadata](run_timings.json)
- [Timestamped run and publication events](event_log.jsonl)

README link: `[Simulation timing log](timing/20261107_10000/run_timings.md)`.
