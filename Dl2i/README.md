# Dl2i

[Workpiece index](../README.md#workpieces)

## Historical pose catalogue

Group numbers rank the saved pose basins by their combined incidence within each observation phase. Pose 0 is the most frequent individual pose in its observation phase. The membership CSV links the displayed numbers to the saved pose IDs. Groups below 1% remain visible.

[Group membership CSV](group_memberships.csv) · [Grouping method](../README.md#catalogue-grouping)

### Transport poses

9,965 settled outcomes across 10,000 historical drops on a 500 mm chute. Incidence uses all completed drops as the denominator.

Outcome counts: settled: 9,965, unsettled: 35.

| Pose | Group | Image | Count | Incidence | 95% interval | Share of settled outcomes |
| --- | --- | --- | ---: | ---: | ---: | ---: |
| Pose 0 | Group 0 | ![Dl2i_0003](images/Dl2i_0003.png) | 1926 | 19.26 % | 18.50–20.04 % | 19.33 % |
| Pose 1 | Group 1 | ![Dl2i_0008](images/Dl2i_0008.png) | 1837 | 18.37 % | 17.62–19.14 % | 18.43 % |
| Pose 2 | Group 0 | ![Dl2i_0006](images/Dl2i_0006.png) | 1703 | 17.03 % | 16.31–17.78 % | 17.09 % |
| Pose 3 | Group 2 | ![Dl2i_0013](images/Dl2i_0013.png) | 1623 | 16.23 % | 15.52–16.97 % | 16.29 % |
| Pose 4 | Group 2 | ![Dl2i_0012](images/Dl2i_0012.png) | 1188 | 11.88 % | 11.26–12.53 % | 11.92 % |
| Pose 5 | Group 1 | ![Dl2i_0009](images/Dl2i_0009.png) | 1025 | 10.25 % | 9.67–10.86 % | 10.29 % |
| Pose 6 | Group 3 | ![Dl2i_0007](images/Dl2i_0007.png) | 173 | 1.73 % | 1.49–2.00 % | 1.74 % |
| Pose 7 | Group 4 | ![Dl2i_0005](images/Dl2i_0005.png) | 145 | 1.45 % | 1.23–1.70 % | 1.46 % |
| Pose 8 | Group 5 | ![Dl2i_0010](images/Dl2i_0010.png) | 143 | 1.43 % | 1.22–1.68 % | 1.44 % |
| Pose 9 | Group 6 | ![Dl2i_0001](images/Dl2i_0001.png) | 95 | 0.95 % | 0.78–1.16 % | 0.95 % |
| Pose 10 | Group 7 | ![Dl2i_0002](images/Dl2i_0002.png) | 46 | 0.46 % | 0.35–0.61 % | 0.46 % |
| Pose 11 | Group 8 | ![Dl2i_0011](images/Dl2i_0011.png) | 46 | 0.46 % | 0.35–0.61 % | 0.46 % |
| Pose 12 | Group 3 | ![Dl2i_0015](images/Dl2i_0015.png) | 3 | 0.03 % | 0.01–0.09 % | 0.03 % |
| Pose 13 | Group 3 | ![Dl2i_0016](images/Dl2i_0016.png) | 3 | 0.03 % | 0.01–0.09 % | 0.03 % |
| Pose 14 | Group 9 | ![Dl2i_0019](images/Dl2i_0019.png) | 3 | 0.03 % | 0.01–0.09 % | 0.03 % |
| Pose 15 | Group 4 | ![Dl2i_0018](images/Dl2i_0018.png) | 2 | 0.02 % | 0.01–0.07 % | 0.02 % |
| Pose 16 | Group 10 | ![Dl2i_0020](images/Dl2i_0020.png) | 2 | 0.02 % | 0.01–0.07 % | 0.02 % |
| Pose 17 | Group 3 | ![Dl2i_0014](images/Dl2i_0014.png) | 1 | 0.01 % | 0.00–0.06 % | 0.01 % |
| Pose 18 | Group 4 | ![Dl2i_0017](images/Dl2i_0017.png) | 1 | 0.01 % | 0.00–0.06 % | 0.01 % |

[Pose catalogue JSON](poses.json) · [Pose catalogue YAML](poses.yaml) · [Frequencies](frequencies.csv) · [Trial records](trials.csv)

Pose orientations use `xyzw` quaternions from the workpiece frame to the chute frame. Recognition uses the recorded symmetry, a 5° tolerance, and a 1° ambiguity margin. The pose registry reserves previously observed IDs for later recognition.

### Historical run files

- [Configuration](config.json)
- [Manifest](manifest.json)

<!-- remaining-workpieces-20261110_10000:start -->
## Additional 10,000-drop runs

10,000 stationary and 10,000 moving-belt drops with the archived reference settings.

[Results and validation](simulations/20261110_10000/README.md).
<!-- remaining-workpieces-20261110_10000:end -->
