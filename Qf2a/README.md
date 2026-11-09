# Qf2a

[Workpiece index](../README.md#workpieces)

## Historical pose catalogue

Group numbers rank the saved pose basins by their combined incidence within each observation phase. Pose 0 is the most frequent individual pose in its observation phase. The membership CSV links the displayed numbers to the saved pose IDs. Groups below 1% remain visible.

[Group membership CSV](group_memberships.csv) · [Grouping method](../README.md#catalogue-grouping)

### Transport poses

9,829 settled outcomes across 10,000 historical drops on a 500 mm chute. Incidence uses all completed drops as the denominator.

Outcome counts: settled: 9,829, unsettled: 171.

| Pose | Group | Image | Count | Incidence | 95% interval | Share of settled outcomes |
| --- | --- | --- | ---: | ---: | ---: | ---: |
| Pose 0 | Group 0 | ![Qf2a_0006](images/Qf2a_0006.png) | 1483 | 14.83 % | 14.15–15.54 % | 15.09 % |
| Pose 1 | Group 1 | ![Qf2a_0013](images/Qf2a_0013.png) | 1370 | 13.70 % | 13.04–14.39 % | 13.94 % |
| Pose 2 | Group 2 | ![Qf2a_0012](images/Qf2a_0012.png) | 1292 | 12.92 % | 12.28–13.59 % | 13.14 % |
| Pose 3 | Group 3 | ![Qf2a_0009](images/Qf2a_0009.png) | 1247 | 12.47 % | 11.84–13.13 % | 12.69 % |
| Pose 4 | Group 4 | ![Qf2a_0001](images/Qf2a_0001.png) | 1191 | 11.91 % | 11.29–12.56 % | 12.12 % |
| Pose 5 | Group 5 | ![Qf2a_0005](images/Qf2a_0005.png) | 1114 | 11.14 % | 10.54–11.77 % | 11.33 % |
| Pose 6 | Group 6 | ![Qf2a_0007](images/Qf2a_0007.png) | 745 | 7.45 % | 6.95–7.98 % | 7.58 % |
| Pose 7 | Group 7 | ![Qf2a_0008](images/Qf2a_0008.png) | 530 | 5.30 % | 4.88–5.76 % | 5.39 % |
| Pose 8 | Group 8 | ![Qf2a_0011](images/Qf2a_0011.png) | 409 | 4.09 % | 3.72–4.50 % | 4.16 % |
| Pose 9 | Group 9 | ![Qf2a_0002](images/Qf2a_0002.png) | 362 | 3.62 % | 3.27–4.00 % | 3.68 % |
| Pose 10 | Group 10 | ![Qf2a_0018](images/Qf2a_0018.png) | 25 | 0.25 % | 0.17–0.37 % | 0.25 % |
| Pose 11 | Group 11 | ![Qf2a_0014](images/Qf2a_0014.png) | 18 | 0.18 % | 0.11–0.28 % | 0.18 % |
| Pose 12 | Group 10 | ![Qf2a_0017](images/Qf2a_0017.png) | 9 | 0.09 % | 0.05–0.17 % | 0.09 % |
| Pose 13 | Group 11 | ![Qf2a_0016](images/Qf2a_0016.png) | 7 | 0.07 % | 0.03–0.14 % | 0.07 % |
| Pose 14 | Group 7 | ![Qf2a_0010](images/Qf2a_0010.png) | 6 | 0.06 % | 0.03–0.13 % | 0.06 % |
| Pose 15 | Group 12 | ![Qf2a_0019](images/Qf2a_0019.png) | 4 | 0.04 % | 0.02–0.10 % | 0.04 % |
| Pose 16 | Group 5 | ![Qf2a_0003](images/Qf2a_0003.png) | 3 | 0.03 % | 0.01–0.09 % | 0.03 % |
| Pose 17 | Group 4 | ![Qf2a_0015](images/Qf2a_0015.png) | 3 | 0.03 % | 0.01–0.09 % | 0.03 % |
| Pose 18 | Group 13 | ![Qf2a_0020](images/Qf2a_0020.png) | 3 | 0.03 % | 0.01–0.09 % | 0.03 % |
| Pose 19 | Group 1 | ![Qf2a_0023](images/Qf2a_0023.png) | 3 | 0.03 % | 0.01–0.09 % | 0.03 % |
| Pose 20 | Group 14 | ![Qf2a_0021](images/Qf2a_0021.png) | 2 | 0.02 % | 0.01–0.07 % | 0.02 % |
| Pose 21 | Group 5 | ![Qf2a_0022](images/Qf2a_0022.png) | 1 | 0.01 % | 0.00–0.06 % | 0.01 % |
| Pose 22 | Group 1 | ![Qf2a_0024](images/Qf2a_0024.png) | 1 | 0.01 % | 0.00–0.06 % | 0.01 % |
| Pose 23 | Group 15 | ![Qf2a_0025](images/Qf2a_0025.png) | 1 | 0.01 % | 0.00–0.06 % | 0.01 % |

[Pose catalogue JSON](poses.json) · [Pose catalogue YAML](poses.yaml) · [Frequencies](frequencies.csv) · [Trial records](trials.csv)

Pose orientations use `xyzw` quaternions from the workpiece frame to the chute frame. Recognition uses the recorded symmetry, a 5° tolerance, and a 1° ambiguity margin. The pose registry reserves previously observed IDs for later recognition.

### Historical run files

- [Configuration](config.json)
- [Manifest](manifest.json)
