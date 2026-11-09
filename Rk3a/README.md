# Rk3a

[Workpiece index](../README.md#workpieces)

## Historical pose catalogue

Group numbers rank the saved pose basins by their combined incidence within each observation phase. Pose 0 is the most frequent individual pose in its observation phase. The membership CSV links the displayed numbers to the saved pose IDs. Groups below 1% remain visible.

[Group membership CSV](group_memberships.csv) · [Grouping method](../README.md#catalogue-grouping)

### Transport poses

9,995 settled outcomes across 10,000 historical drops on a 500 mm chute. Incidence uses all completed drops as the denominator.

Outcome counts: settled: 9,995, unsettled: 5.

| Pose | Group | Image | Count | Incidence | 95% interval | Share of settled outcomes |
| --- | --- | --- | ---: | ---: | ---: | ---: |
| Pose 0 | Group 0 | ![Rk3a_0014](images/Rk3a_0014.png) | 1349 | 13.49 % | 12.83–14.17 % | 13.50 % |
| Pose 1 | Group 2 | ![Rk3a_0012](images/Rk3a_0012.png) | 1267 | 12.67 % | 12.03–13.34 % | 12.68 % |
| Pose 2 | Group 1 | ![Rk3a_0010](images/Rk3a_0010.png) | 1109 | 11.09 % | 10.49–11.72 % | 11.10 % |
| Pose 3 | Group 3 | ![Rk3a_0004](images/Rk3a_0004.png) | 1053 | 10.53 % | 9.94–11.15 % | 10.54 % |
| Pose 4 | Group 4 | ![Rk3a_0003](images/Rk3a_0003.png) | 1035 | 10.35 % | 9.77–10.96 % | 10.36 % |
| Pose 5 | Group 5 | ![Rk3a_0009](images/Rk3a_0009.png) | 1027 | 10.27 % | 9.69–10.88 % | 10.28 % |
| Pose 6 | Group 6 | ![Rk3a_0002](images/Rk3a_0002.png) | 899 | 8.99 % | 8.45–9.57 % | 8.99 % |
| Pose 7 | Group 7 | ![Rk3a_0008](images/Rk3a_0008.png) | 849 | 8.49 % | 7.96–9.05 % | 8.49 % |
| Pose 8 | Group 8 | ![Rk3a_0011](images/Rk3a_0011.png) | 426 | 4.26 % | 3.88–4.67 % | 4.26 % |
| Pose 9 | Group 9 | ![Rk3a_0013](images/Rk3a_0013.png) | 409 | 4.09 % | 3.72–4.50 % | 4.09 % |
| Pose 10 | Group 1 | ![Rk3a_0007](images/Rk3a_0007.png) | 201 | 2.01 % | 1.75–2.30 % | 2.01 % |
| Pose 11 | Group 3 | ![Rk3a_0006](images/Rk3a_0006.png) | 162 | 1.62 % | 1.39–1.89 % | 1.62 % |
| Pose 12 | Group 10 | ![Rk3a_0001](images/Rk3a_0001.png) | 133 | 1.33 % | 1.12–1.57 % | 1.33 % |
| Pose 13 | Group 11 | ![Rk3a_0005](images/Rk3a_0005.png) | 61 | 0.61 % | 0.48–0.78 % | 0.61 % |
| Pose 14 | Group 12 | ![Rk3a_0016](images/Rk3a_0016.png) | 12 | 0.12 % | 0.07–0.21 % | 0.12 % |
| Pose 15 | Group 12 | ![Rk3a_0017](images/Rk3a_0017.png) | 2 | 0.02 % | 0.01–0.07 % | 0.02 % |
| Pose 16 | Group 13 | ![Rk3a_0015](images/Rk3a_0015.png) | 1 | 0.01 % | 0.00–0.06 % | 0.01 % |

[Pose catalogue JSON](poses.json) · [Pose catalogue YAML](poses.yaml) · [Frequencies](frequencies.csv) · [Trial records](trials.csv)

Pose orientations use `xyzw` quaternions from the workpiece frame to the chute frame. Recognition uses the recorded symmetry, a 5° tolerance, and a 1° ambiguity margin. The pose registry reserves previously observed IDs for later recognition.

### Historical run files

- [Configuration](config.json)
- [Manifest](manifest.json)
