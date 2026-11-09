# Qk2i

[Workpiece index](../README.md#workpieces)

## Historical pose catalogue

Group numbers rank the saved pose basins by their combined incidence within each observation phase. Pose 0 is the most frequent individual pose in its observation phase. The membership CSV links the displayed numbers to the saved pose IDs. Groups below 1% remain visible.

[Group membership CSV](group_memberships.csv) · [Grouping method](../README.md#catalogue-grouping)

### Transport poses

10,000 settled outcomes across 10,000 historical drops on a 500 mm chute. Incidence uses all completed drops as the denominator.

Outcome counts: settled: 10,000.

| Pose | Group | Image | Count | Incidence | 95% interval | Share of settled outcomes |
| --- | --- | --- | ---: | ---: | ---: | ---: |
| Pose 0 | Group 0 | ![Qk2i_0004](images/Qk2i_0004.png) | 1188 | 11.88 % | 11.26–12.53 % | 11.88 % |
| Pose 1 | Group 1 | ![Qk2i_0012](images/Qk2i_0012.png) | 1147 | 11.47 % | 10.86–12.11 % | 11.47 % |
| Pose 2 | Group 2 | ![Qk2i_0011](images/Qk2i_0011.png) | 1145 | 11.45 % | 10.84–12.09 % | 11.45 % |
| Pose 3 | Group 3 | ![Qk2i_0006](images/Qk2i_0006.png) | 1113 | 11.13 % | 10.53–11.76 % | 11.13 % |
| Pose 4 | Group 4 | ![Qk2i_0003](images/Qk2i_0003.png) | 712 | 7.12 % | 6.63–7.64 % | 7.12 % |
| Pose 5 | Group 5 | ![Qk2i_0015](images/Qk2i_0015.png) | 705 | 7.05 % | 6.56–7.57 % | 7.05 % |
| Pose 6 | Group 6 | ![Qk2i_0005](images/Qk2i_0005.png) | 672 | 6.72 % | 6.25–7.23 % | 6.72 % |
| Pose 7 | Group 7 | ![Qk2i_0009](images/Qk2i_0009.png) | 667 | 6.67 % | 6.20–7.18 % | 6.67 % |
| Pose 8 | Group 8 | ![Qk2i_0002](images/Qk2i_0002.png) | 644 | 6.44 % | 5.98–6.94 % | 6.44 % |
| Pose 9 | Group 9 | ![Qk2i_0001](images/Qk2i_0001.png) | 643 | 6.43 % | 5.97–6.93 % | 6.43 % |
| Pose 10 | Group 10 | ![Qk2i_0010](images/Qk2i_0010.png) | 622 | 6.22 % | 5.76–6.71 % | 6.22 % |
| Pose 11 | Group 11 | ![Qk2i_0014](images/Qk2i_0014.png) | 575 | 5.75 % | 5.31–6.22 % | 5.75 % |
| Pose 12 | Group 12 | ![Qk2i_0013](images/Qk2i_0013.png) | 125 | 1.25 % | 1.05–1.49 % | 1.25 % |
| Pose 13 | Group 13 | ![Qk2i_0007](images/Qk2i_0007.png) | 27 | 0.27 % | 0.19–0.39 % | 0.27 % |
| Pose 14 | Group 14 | ![Qk2i_0008](images/Qk2i_0008.png) | 15 | 0.15 % | 0.09–0.25 % | 0.15 % |

[Pose catalogue JSON](poses.json) · [Pose catalogue YAML](poses.yaml) · [Frequencies](frequencies.csv) · [Trial records](trials.csv)

Pose orientations use `xyzw` quaternions from the workpiece frame to the chute frame. Recognition uses the recorded symmetry, a 5° tolerance, and a 1° ambiguity margin. The pose registry reserves previously observed IDs for later recognition.

### Historical run files

- [Configuration](config.json)
- [Manifest](manifest.json)
