# BiBaZu Stable Component Poses

The completed ungrouped 10,000-drop dataset contains **780,000 simulated drops across all 39 workpieces**. Each workpiece has **10,000 trials with the belt stationary from release** and **10,000 trials on the moving belt**. The original twelve-workpiece paper study contributes 240,000 drops; the same-settings extension adds 540,000 drops for the remaining 27 workpieces. All 78 runs are complete and validated.

The linked runs preserve individual orientations, trial outcomes, configurations, execution timings, and validation records. Earlier pose catalogues and 1,000-drop comparisons remain separate historical datasets.

The moving series records the outcome at the virtual exit while the belt runs. The post-exit braking and rest check produces a separate result. The reported moving incidence uses the exit outcomes, and moving-series wall times include the follow-up observation.

## Simulator settings

| Parameter | Shared 10,000-drop benchmark setting |
| --- | --- |
| Trials per workpiece and condition | 10,000 |
| Random seed | 42 |
| Worker processes per run | 24 |
| Chute geometry | 45° transverse tilt, 0° longitudinal inclination, 500 mm configured length |
| Initial orientation | Uniform random orientation in 3D |
| Release height | 100 mm with 0 mm spread |
| Lateral release offset | 0 mm with 0 mm spread |
| Workpiece density | 1.15 g/cm³, uniform |
| Moving belt | 100 ± 3 mm/s with 0.2 s between speed targets |
| Stationary belt | 0 mm/s from release, with no speed variation |
| Moving outcome | Virtual exit with the belt running. The final 0.5 s window checks contact support, orientation and transverse motion. |
| Stationary outcome | At 10 s. The final 0.5 s window checks contact support, orientation and motion in all three axes. |
| Separate post-exit observation | Moving series only. 0.2 s braking ramp, then 2 s with the belt stopped. |
| Friction cone | Elliptic |
| PE mesh belt sliding friction | 0.10 |
| PTFE wall sliding friction | 0.05 |
| Torsional and rolling friction parameters | 5 mm torsional, 0.1 mm rolling |
| Contact time constant | 5 ms |
| Contact damping ratio | 0.19 |
| Integration time step | 1 ms |
| Surface excitation | `weight_impulse` for the first 1 s |
| Impulse magnitude | 49.05 mm/s equivalent free-body velocity change |
| Mean impulse interval | 0.2 s |
| Trial grouping and additional stability tests | Disabled in all 78 saved benchmark runs |

The belt and wall coefficients describe effective contact in the simulation. The PE/plastic example in the Habasit guide supports 0.10 as a nominal starting value for the belt. The archived configurations identify the geometry and full parameter set for each run. [Habasit engineering guide, p. 94](https://rodavigo.net/catalogos/HABASIT/Bandas%20modulares%20HABASITLINK/HABASIT%2004%20Gu%C3%ADa%20Ingenier%C3%ADa%20HabasitLINK.pdf#page=94) · [Original run plan](timing/20261107_10000/run_plan.json) · [Extension run plan](timing/20261110_10000/run_plan.json)

The original benchmark used a Beckhoff C6043 with an Intel Core i9-13900E, 32 GB RAM, and Windows 11 IoT Enterprise LTSC 24H2. The timing log records 24 logical CPUs, Python 3.12.13, MuJoCo 3.14.0, CoACD 1.0.14, NumPy 2.5.3, SciPy 1.18.1, trimesh 5.1.0, and `bibazu-chute-pose` 0.1.0. [Simulator repository](https://github.com/match-BiBaZu/BiBaZu_PoseFindingDropSim) · [Simulator revision](https://github.com/match-BiBaZu/BiBaZu_PoseFindingDropSim/commit/72b1ba08aa9b317804cd60e1e2ae6e636910f3fd)

## Completed batches and timings

Both batches used the same archived simulator settings, revision, and dependency fingerprint. Times below are the sums of the measured simulation-call wall times, rounded to the nearest second. They include geometry and symmetry preparation, worker startup, physics, and raw result writing; validation, compression, and publishing are excluded.

| Batch | Workpieces | Runs | Drops | Simulation wall time | Records |
| --- | ---: | ---: | ---: | --- | --- |
| Original paper study (`20261107_10000`) | 12 | 24 | 240,000 | 12 h 46 min 42 s | [Plan](timing/20261107_10000/run_plan.json) · [Timings](timing/20261107_10000/run_timings.md) · [Validation](timing/20261107_10000/batch_validation.json) |
| Remaining-workpiece extension (`20261110_10000`) | 27 | 54 | 540,000 | 42 h 30 min 01 s | [Plan](timing/20261110_10000/run_plan.json) · [Timings](timing/20261110_10000/status.json) · [Validation](timing/20261110_10000/batch_validation.json) |
| **Total** | **39** | **78** | **780,000** | **55 h 16 min 43 s** | Both batches |

## Workpieces

Each count below is the number of settled outcomes out of **10,000 trials** in that condition. Moving counts use the virtual-exit outcome, separately from the post-braking observation. Catalogue pages describe the earlier saved pose catalogues; run links open the completed ungrouped 10,000-drop datasets.

| Workpiece catalogue | Stationary settled / 10,000 | Moving settled / 10,000 | Run records |
| --- | ---: | ---: | --- |
| [Df1a](Df1a/README.md) | 9,975 | 9,999 | [Moving and stationary runs](Df1a/simulations/20261107_10000/README.md) |
| [Df2i](Df2i/README.md) | 9,998 | 9,999 | [Moving and stationary runs](Df2i/simulations/20261110_10000/README.md) |
| [Df4a](Df4a/README.md) | 9,998 | 10,000 | [Moving and stationary runs](Df4a/simulations/20261110_10000/README.md) |
| [Dk1i](Dk1i/README.md) | 10,000 | 9,950 | [Moving and stationary runs](Dk1i/simulations/20261107_10000/README.md) |
| [Dk2a](Dk2a/README.md) | 9,962 | 9,998 | [Moving and stationary runs](Dk2a/simulations/20261110_10000/README.md) |
| [Dk4i](Dk4i/README.md) | 9,995 | 9,906 | [Moving and stationary runs](Dk4i/simulations/20261110_10000/README.md) |
| [Dl1a](Dl1a/README.md) | 9,992 | 10,000 | [Moving and stationary runs](Dl1a/simulations/20261107_10000/README.md) |
| [Dl2i](Dl2i/README.md) | 10,000 | 9,999 | [Moving and stationary runs](Dl2i/simulations/20261110_10000/README.md) |
| [Dl4a](Dl4a/README.md) | 9,999 | 9,999 | [Moving and stationary runs](Dl4a/simulations/20261110_10000/README.md) |
| [Kf1i](Kf1i/README.md) | 10,000 | 9 | [Moving and stationary runs](Kf1i/simulations/20261107_10000/README.md) |
| [Kf2a](Kf2a/README.md) | 9,936 | 8,763 | [Moving and stationary runs](Kf2a/simulations/20261110_10000/README.md) |
| [Kf4i](Kf4i/README.md) | 8,982 | 8,997 | [Moving and stationary runs](Kf4i/simulations/20261110_10000/README.md) |
| [Kk1a](Kk1a/README.md) | 9,676 | 8,201 | [Moving and stationary runs](Kk1a/simulations/20261107_10000/README.md) |
| [Kk2i](Kk2i/README.md) | 9,978 | 9,385 | [Moving and stationary runs](Kk2i/simulations/20261110_10000/README.md) |
| [Kk4a](Kk4a/README.md) | 9,995 | 9,988 | [Moving and stationary runs](Kk4a/simulations/20261110_10000/README.md) |
| [Kl1i](Kl1i/README.md) | 9,997 | 9,999 | [Moving and stationary runs](Kl1i/simulations/20261107_10000/README.md) |
| [Kl2a](Kl2a/README.md) | 9,989 | 9,994 | [Moving and stationary runs](Kl2a/simulations/20261110_10000/README.md) |
| [Kl4i](Kl4i/README.md) | 9,995 | 9,939 | [Moving and stationary runs](Kl4i/simulations/20261110_10000/README.md) |
| [Qf1i](Qf1i/README.md) | 9,943 | 9,991 | [Moving and stationary runs](Qf1i/simulations/20261107_10000/README.md) |
| [Qf2a](Qf2a/README.md) | 9,971 | 9,997 | [Moving and stationary runs](Qf2a/simulations/20261110_10000/README.md) |
| [Qf4i](Qf4i/README.md) | 9,994 | 9,997 | [Moving and stationary runs](Qf4i/simulations/20261110_10000/README.md) |
| [Qk1a](Qk1a/README.md) | 9,899 | 9,953 | [Moving and stationary runs](Qk1a/simulations/20261107_10000/README.md) |
| [Qk2i](Qk2i/README.md) | 9,977 | 9,998 | [Moving and stationary runs](Qk2i/simulations/20261110_10000/README.md) |
| [Qk4a](Qk4a/README.md) | 9,984 | 9,993 | [Moving and stationary runs](Qk4a/simulations/20261110_10000/README.md) |
| [Ql1i](Ql1i/README.md) | 9,995 | 9,992 | [Moving and stationary runs](Ql1i/simulations/20261107_10000/README.md) |
| [Ql2a](Ql2a/README.md) | 9,997 | 9,997 | [Moving and stationary runs](Ql2a/simulations/20261110_10000/README.md) |
| [Ql4i](Ql4i/README.md) | 9,997 | 10,000 | [Moving and stationary runs](Ql4i/simulations/20261110_10000/README.md) |
| [Rf1a](Rf1a/README.md) | 9,988 | 10,000 | [Moving and stationary runs](Rf1a/simulations/20261107_10000/README.md) |
| [Rf2i](Rf2i/README.md) | 9,989 | 9,999 | [Moving and stationary runs](Rf2i/simulations/20261110_10000/README.md) |
| [Rf3a](Rf3a/README.md) | 9,993 | 10,000 | [Moving and stationary runs](Rf3a/simulations/20261110_10000/README.md) |
| [Rf4i](Rf4i/README.md) | 9,995 | 10,000 | [Moving and stationary runs](Rf4i/simulations/20261110_10000/README.md) |
| [Rk1a](Rk1a/README.md) | 9,970 | 9,998 | [Moving and stationary runs](Rk1a/simulations/20261107_10000/README.md) |
| [Rk2i](Rk2i/README.md) | 9,985 | 9,997 | [Moving and stationary runs](Rk2i/simulations/20261110_10000/README.md) |
| [Rk3a](Rk3a/README.md) | 9,975 | 9,995 | [Moving and stationary runs](Rk3a/simulations/20261110_10000/README.md) |
| [Rk4i](Rk4i/README.md) | 9,965 | 9,996 | [Moving and stationary runs](Rk4i/simulations/20261110_10000/README.md) |
| [Rl1a](Rl1a/README.md) | 9,994 | 9,996 | [Moving and stationary runs](Rl1a/simulations/20261107_10000/README.md) |
| [Rl2i](Rl2i/README.md) | 9,995 | 9,985 | [Moving and stationary runs](Rl2i/simulations/20261110_10000/README.md) |
| [Rl3a](Rl3a/README.md) | 9,997 | 10,000 | [Moving and stationary runs](Rl3a/simulations/20261110_10000/README.md) |
| [Rl4i](Rl4i/README.md) | 9,999 | 10,000 | [Moving and stationary runs](Rl4i/simulations/20261110_10000/README.md) |

## Run files

Each condition folder contains a lossless `simulation_results.tar.xz` archive and the following records:

| File | Contents |
| --- | --- |
| `summary.json` | Compact outcome counts; the full per-trial frequency summary is inside the archive. |
| `config.json` | Run settings with a relative path to the workpiece STL. |
| `manifest.json` | Simulator revision, dependency versions, geometry hashes, and model details. |
| `execution.json` | Original configuration, settings signature, simulation wall time, and reference comparison. |
| `validation.json` | Checks of trial counts and IDs, deterministic seeds, outcomes, and finite normalized orientations. |
| `archive_contents.sha256.json` | SHA-256 checksums of every original file inside the archive. |
| `files.sha256.json` | SHA-256 checksums of the published files, including the archive and README. |

The archive preserves the CSV/JSONL trial records, individual settled orientations, roughness events, original configuration, full summary, and post-braking observations where recorded. With grouping disabled, each settled trial keeps its own orientation and trial ID; frequency rows represent individual trials rather than grouped pose classes. Incidence uses all completed trials as the denominator, including unsettled outcomes.

Extract an archive with:

```powershell
python -m tarfile -e simulation_results.tar.xz extracted
```

## Catalogue grouping

Except for the six scoped rolling-surface catalogues described below, each historical catalogue displays its saved individual poses and the basin assigned by the local plotter’s simulator grouping method. The algorithm uses the recorded orientations, workpiece symmetry, and chute angles. It applies directed absorption with a 0.5 mm equivalent lift barrier, a 60° whole-group diameter limit, and 0.1° angular path sampling. Group 0 has the highest combined incidence in its catalogue. Ties follow the sorted member pose IDs, and groups below 1% stay visible.

Transport and post-braking catalogues have separate group and pose numbering. Pose 0 is the most frequent individual pose in its catalogue. Ties follow the saved pose IDs. The membership CSV links each displayed pose number and group to the original pose ID, basin ID, and counts. The table grouping was computed from saved catalogue poses. All 10,000-drop archives retain their original ungrouped trial records; the historical catalogue grouping does not change those results. [Grouping engine](https://github.com/match-BiBaZu/BiBaZu_PoseFindingDropSim/blob/b872011538ae74d2c2a4570a32457cb79054a598/src/dashas_drop_sim/grouping.py) · [Historical grouped snapshot](https://github.com/match-BiBaZu/BiBaZu_Stable_ComponentPoses/tree/632b830bd890498e1b07b14d44d97b25f5bba7bb)

## Scoped rolling-surface validation (13 November 2026)

Kk2i, Kk4a, Kl4i, Kl2a, Kf2a and Kf4i use persistent seated-energy minima and minimax-height assignments. The 60° limit is local to each path; sampling remains 0.1° and the escape-barrier threshold remains 0.5 mm. A pose reaching multiple minima stays separate for review. Individual poses, counts, feature directions and recognition tolerances are preserved. The saved Kl4i catalogue yields four groups. Original simulation archives remain unchanged.

Each of these six workpieces adds 100 stationary and 100 moving-belt drops (1,200 published drops), using the archived physical settings. No disturbance sweeps were added. The other 33 workpieces also passed paired 100-drop checks and exact legacy-grouping comparisons; their validation data remains local and their catalogue directories are byte-for-byte unchanged.

| Workpiece | Grouping evidence | Paired validation |
| --- | --- | --- |
| Kk2i | [Groups](Kk2i/grouping/20261113/README.md) | [200 drops](Kk2i/simulations/20261113_rolling_100/README.md) |
| Kk4a | [Groups](Kk4a/grouping/20261113/README.md) | [200 drops](Kk4a/simulations/20261113_rolling_100/README.md) |
| Kl4i | [Groups](Kl4i/grouping/20261113/README.md) | [200 drops](Kl4i/simulations/20261113_rolling_100/README.md) |
| Kl2a | [Groups](Kl2a/grouping/20261113/README.md) | [200 drops](Kl2a/simulations/20261113_rolling_100/README.md) |
| Kf2a | [Groups](Kf2a/grouping/20261113/README.md) | [200 drops](Kf2a/simulations/20261113_rolling_100/README.md) |
| Kf4i | [Groups](Kf4i/grouping/20261113/README.md) | [200 drops](Kf4i/simulations/20261113_rolling_100/README.md) |
