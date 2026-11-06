# Simulation timing log

Published results: **2/12 parts**, **4,000/24,000 trials**. Each part has 1,000 static trials and 1,000 trials at 100 ±3 mm/s, with grouping off.

Measured wall time uses `time.perf_counter()` around the simulation call. It includes geometry and symmetry preparation, process startup, physics, and writing raw results. Validation, archive compression, commits, and pushes take additional time. Each run uses 24 worker processes on a machine with 24 logical CPUs. Cached geometry can affect preparation time.

| Part | Static: 1,000 trials (s) | 100 ±3 mm/s: 1,000 trials (s) | Simulation total (s) |
| --- | ---: | ---: | ---: |
| Df1a | 177.640 | 132.430 | 310.070 |
| Dk1i | 250.266 | 189.489 | 439.755 |

Sum of measured simulation durations: **749.825 s (12.50 min)**.

The CSV and JSON include individual start times, measured durations, throughput, result-save times, push times, settings signatures, and result commits. UTC times are explicitly labelled. Replaced exact-speed and interrupted attempts remain in the event log; their durations are excluded from this table.

- [CSV timing log](run_timings.csv)
- [JSON timings and machine/software metadata](run_timings.json)
- [Timestamped run and publication events](event_log.jsonl)

README link: `[Simulation timing log](timing/run_timings.md)`.
