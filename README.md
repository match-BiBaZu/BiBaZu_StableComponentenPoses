# BiBaZu Stable Component Poses

The paper dataset contains **240,000 simulated drops**. Each of 12 workpieces has **10,000 trials with the belt stationary from release** and **10,000 trials on the moving belt**. The linked runs contain the saved orientations, trial outcomes, configuration, and validation records. The workpiece pages also present earlier pose catalogues for all 39 components.

The moving series records the outcome at the virtual exit while the belt runs. The post-exit braking and rest check produces a separate result. The reported moving incidence uses the exit outcomes, and moving-series wall times include the follow-up observation.

## Simulator settings

| Parameter | Recorded paper benchmark setting |
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
| Trial grouping and additional stability tests | Disabled in the saved benchmark runs |

The belt and wall coefficients describe effective contact in the simulation. The PE/plastic example in the Habasit guide supports 0.10 as a nominal starting value for the belt. The archived configurations identify the geometry and full parameter set for each run. [Habasit engineering guide, p. 94](https://rodavigo.net/catalogos/HABASIT/Bandas%20modulares%20HABASITLINK/HABASIT%2004%20Gu%C3%ADa%20Ingenier%C3%ADa%20HabasitLINK.pdf#page=94) · [Archived run plan](timing/20261107_10000/run_plan.json)

The runs used a Beckhoff C6043 with an Intel Core i9-13900E, 32 GB RAM, and Windows 11 IoT Enterprise LTSC 24H2. The timing log records 24 logical CPUs, Python 3.12.13, MuJoCo 3.14.0, CoACD 1.0.14, NumPy 2.5.3, SciPy 1.18.1, trimesh 5.1.0, and `bibazu-chute-pose` 0.1.0. [Simulator revision](https://github.com/match-BiBaZu/BiBaZu_PoseFindingDropSim/commit/72b1ba08aa9b317804cd60e1e2ae6e636910f3fd)

The 24 simulation calls took **12 h 46 min 42 s** in total. They include geometry and symmetry preparation, worker startup, physics, and raw result writing. The full workflow took **20 h 23 min 32 s**, including validation, compression, publishing, and interruption and recovery. [Timing records](timing/20261107_10000/run_timings.md) · [Batch validation](timing/20261107_10000/batch_validation.json)

## Workpieces

The paper columns report settled outcomes out of 10,000 trials per condition. A dash indicates a workpiece outside the paper series.

| Workpiece catalogue | Stationary settled | Moving settled | Paper run records |
| --- | --- | --- | --- |
| [Df1a](Df1a/README.md) | 9,975 | 9,999 | [Moving and stationary runs](Df1a/simulations/20261107_10000/README.md) |
| [Df2i](Df2i/README.md) | — | — | — |
| [Df4a](Df4a/README.md) | — | — | — |
| [Dk1i](Dk1i/README.md) | 10,000 | 9,950 | [Moving and stationary runs](Dk1i/simulations/20261107_10000/README.md) |
| [Dk2a](Dk2a/README.md) | — | — | — |
| [Dk4i](Dk4i/README.md) | — | — | — |
| [Dl1a](Dl1a/README.md) | 9,992 | 10,000 | [Moving and stationary runs](Dl1a/simulations/20261107_10000/README.md) |
| [Dl2i](Dl2i/README.md) | — | — | — |
| [Dl4a](Dl4a/README.md) | — | — | — |
| [Kf1i](Kf1i/README.md) | 10,000 | 9 | [Moving and stationary runs](Kf1i/simulations/20261107_10000/README.md) |
| [Kf2a](Kf2a/README.md) | — | — | — |
| [Kf4i](Kf4i/README.md) | — | — | — |
| [Kk1a](Kk1a/README.md) | 9,676 | 8,201 | [Moving and stationary runs](Kk1a/simulations/20261107_10000/README.md) |
| [Kk2i](Kk2i/README.md) | — | — | — |
| [Kk4a](Kk4a/README.md) | — | — | — |
| [Kl1i](Kl1i/README.md) | 9,997 | 9,999 | [Moving and stationary runs](Kl1i/simulations/20261107_10000/README.md) |
| [Kl2a](Kl2a/README.md) | — | — | — |
| [Kl4i](Kl4i/README.md) | — | — | — |
| [Qf1i](Qf1i/README.md) | 9,943 | 9,991 | [Moving and stationary runs](Qf1i/simulations/20261107_10000/README.md) |
| [Qf2a](Qf2a/README.md) | — | — | — |
| [Qf4i](Qf4i/README.md) | — | — | — |
| [Qk1a](Qk1a/README.md) | 9,899 | 9,953 | [Moving and stationary runs](Qk1a/simulations/20261107_10000/README.md) |
| [Qk2i](Qk2i/README.md) | — | — | — |
| [Qk4a](Qk4a/README.md) | — | — | — |
| [Ql1i](Ql1i/README.md) | 9,995 | 9,992 | [Moving and stationary runs](Ql1i/simulations/20261107_10000/README.md) |
| [Ql2a](Ql2a/README.md) | — | — | — |
| [Ql4i](Ql4i/README.md) | — | — | — |
| [Rf1a](Rf1a/README.md) | 9,988 | 10,000 | [Moving and stationary runs](Rf1a/simulations/20261107_10000/README.md) |
| [Rf2i](Rf2i/README.md) | — | — | — |
| [Rf3a](Rf3a/README.md) | — | — | — |
| [Rf4i](Rf4i/README.md) | — | — | — |
| [Rk1a](Rk1a/README.md) | 9,970 | 9,998 | [Moving and stationary runs](Rk1a/simulations/20261107_10000/README.md) |
| [Rk2i](Rk2i/README.md) | — | — | — |
| [Rk3a](Rk3a/README.md) | — | — | — |
| [Rk4i](Rk4i/README.md) | — | — | — |
| [Rl1a](Rl1a/README.md) | 9,994 | 9,996 | [Moving and stationary runs](Rl1a/simulations/20261107_10000/README.md) |
| [Rl2i](Rl2i/README.md) | — | — | — |
| [Rl3a](Rl3a/README.md) | — | — | — |
| [Rl4i](Rl4i/README.md) | — | — | — |

## Catalogue grouping

Each historical catalogue displays its saved individual poses and the basin assigned by the local plotter’s simulator grouping method. The algorithm uses the recorded orientations, workpiece symmetry, and chute angles. It applies directed absorption with a 0.5 mm equivalent lift barrier, a 60° whole-group diameter limit, and 0.1° angular path sampling. Group 0 has the highest combined incidence in its catalogue. Ties follow the sorted member pose IDs, and groups below 1% stay visible.

Transport and post-braking catalogues have separate group numbering. The membership CSV on each workpiece page records the observation phase, original pose ID, display group, basin ID, and counts. The table grouping was computed from saved catalogue poses. The paper archives retain their original ungrouped trial records. [Grouping engine](https://github.com/match-BiBaZu/BiBaZu_PoseFindingDropSim/blob/b872011538ae74d2c2a4570a32457cb79054a598/src/dashas_drop_sim/grouping.py) · [Historical grouped snapshot](https://github.com/match-BiBaZu/BiBaZu_Stable_ComponentPoses/tree/632b830bd890498e1b07b14d44d97b25f5bba7bb)
