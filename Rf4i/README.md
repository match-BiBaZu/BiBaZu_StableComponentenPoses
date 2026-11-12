# Rf4i

[Workpiece index](../README.md#workpieces)

## Historical pose catalogue

Group numbers rank the saved pose basins by their combined incidence within each observation phase. Pose 0 is the most frequent individual pose in its observation phase. The membership CSV links the displayed numbers to the saved pose IDs. Groups below 1% remain visible.

[Group membership CSV](group_memberships.csv) · [Grouping method](../README.md#catalogue-grouping)

### Transport poses

9,885 settled outcomes across 10,000 historical drops on a 500 mm chute. Incidence uses all completed drops as the denominator.

Outcome counts: settled: 9,885, unsettled: 115.

| Pose | Group | Image | Count | Incidence | 95% interval | Share of settled outcomes |
| --- | --- | --- | ---: | ---: | ---: | ---: |
| Pose 0 | Group 0 | ![Rf4i_0008](images/Rf4i_0008.png) | 1061 | 10.61 % | 10.02–11.23 % | 10.73 % |
| Pose 1 | Group 1 | ![Rf4i_0005](images/Rf4i_0005.png) | 1052 | 10.52 % | 9.93–11.14 % | 10.64 % |
| Pose 2 | Group 2 | ![Rf4i_0015](images/Rf4i_0015.png) | 816 | 8.16 % | 7.64–8.71 % | 8.25 % |
| Pose 3 | Group 3 | ![Rf4i_0003](images/Rf4i_0003.png) | 776 | 7.76 % | 7.25–8.30 % | 7.85 % |
| Pose 4 | Group 4 | ![Rf4i_0006](images/Rf4i_0006.png) | 616 | 6.16 % | 5.71–6.65 % | 6.23 % |
| Pose 5 | Group 5 | ![Rf4i_0010](images/Rf4i_0010.png) | 571 | 5.71 % | 5.27–6.18 % | 5.78 % |
| Pose 6 | Group 6 | ![Rf4i_0016](images/Rf4i_0016.png) | 557 | 5.57 % | 5.14–6.04 % | 5.63 % |
| Pose 7 | Group 7 | ![Rf4i_0011](images/Rf4i_0011.png) | 550 | 5.50 % | 5.07–5.96 % | 5.56 % |
| Pose 8 | Group 8 | ![Rf4i_0002](images/Rf4i_0002.png) | 544 | 5.44 % | 5.01–5.90 % | 5.50 % |
| Pose 9 | Group 9 | ![Rf4i_0013](images/Rf4i_0013.png) | 544 | 5.44 % | 5.01–5.90 % | 5.50 % |
| Pose 10 | Group 10 | ![Rf4i_0009](images/Rf4i_0009.png) | 499 | 4.99 % | 4.58–5.43 % | 5.05 % |
| Pose 11 | Group 11 | ![Rf4i_0004](images/Rf4i_0004.png) | 496 | 4.96 % | 4.55–5.40 % | 5.02 % |
| Pose 12 | Group 12 | ![Rf4i_0020](images/Rf4i_0020.png) | 469 | 4.69 % | 4.29–5.12 % | 4.74 % |
| Pose 13 | Group 13 | ![Rf4i_0012](images/Rf4i_0012.png) | 466 | 4.66 % | 4.26–5.09 % | 4.71 % |
| Pose 14 | Group 14 | ![Rf4i_0014](images/Rf4i_0014.png) | 443 | 4.43 % | 4.04–4.85 % | 4.48 % |
| Pose 15 | Group 15 | ![Rf4i_0001](images/Rf4i_0001.png) | 396 | 3.96 % | 3.60–4.36 % | 4.01 % |
| Pose 16 | Group 16 | ![Rf4i_0017](images/Rf4i_0017.png) | 5 | 0.05 % | 0.02–0.12 % | 0.05 % |
| Pose 17 | Group 17 | ![Rf4i_0019](images/Rf4i_0019.png) | 4 | 0.04 % | 0.02–0.10 % | 0.04 % |
| Pose 18 | Group 14 | ![Rf4i_0022](images/Rf4i_0022.png) | 4 | 0.04 % | 0.02–0.10 % | 0.04 % |
| Pose 19 | Group 18 | ![Rf4i_0007](images/Rf4i_0007.png) | 3 | 0.03 % | 0.01–0.09 % | 0.03 % |
| Pose 20 | Group 7 | ![Rf4i_0023](images/Rf4i_0023.png) | 3 | 0.03 % | 0.01–0.09 % | 0.03 % |
| Pose 21 | Group 19 | ![Rf4i_0026](images/Rf4i_0026.png) | 3 | 0.03 % | 0.01–0.09 % | 0.03 % |
| Pose 22 | Group 16 | ![Rf4i_0018](images/Rf4i_0018.png) | 2 | 0.02 % | 0.01–0.07 % | 0.02 % |
| Pose 23 | Group 10 | ![Rf4i_0025](images/Rf4i_0025.png) | 2 | 0.02 % | 0.01–0.07 % | 0.02 % |
| Pose 24 | Group 20 | ![Rf4i_0021](images/Rf4i_0021.png) | 1 | 0.01 % | 0.00–0.06 % | 0.01 % |
| Pose 25 | Group 21 | ![Rf4i_0024](images/Rf4i_0024.png) | 1 | 0.01 % | 0.00–0.06 % | 0.01 % |
| Pose 26 | Group 22 | ![Rf4i_0027](images/Rf4i_0027.png) | 1 | 0.01 % | 0.00–0.06 % | 0.01 % |

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
