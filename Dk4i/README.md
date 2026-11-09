# Dk4i

[Workpiece index](../README.md#workpieces)

## Historical pose catalogue

Group numbers rank the saved pose basins by their combined incidence within each observation phase. The percentages in the table describe each individual pose. Groups below 1% remain visible.

[Group membership CSV](group_memberships.csv) · [Grouping method](../README.md#catalogue-grouping)

### Transport poses

9,999 settled outcomes across 10,000 historical drops on a 500 mm chute. Incidence uses all completed drops as the denominator.

Outcome counts: settled: 9,999, unsettled: 1.

| Pose | Group | Image | Count | Incidence | 95% interval | Share of settled outcomes |
| --- | --- | --- | ---: | ---: | ---: | ---: |
| Dk4i_0003 | Group 1 | ![Dk4i_0003](images/Dk4i_0003.png) | 633 | 6.33 % | 5.87–6.82 % | 6.33 % |
| Dk4i_0009 | Group 0 | ![Dk4i_0009](images/Dk4i_0009.png) | 609 | 6.09 % | 5.64–6.58 % | 6.09 % |
| Dk4i_0006 | Group 2 | ![Dk4i_0006](images/Dk4i_0006.png) | 584 | 5.84 % | 5.40–6.32 % | 5.84 % |
| Dk4i_0015 | Group 6 | ![Dk4i_0015](images/Dk4i_0015.png) | 552 | 5.52 % | 5.09–5.98 % | 5.52 % |
| Dk4i_0023 | Group 4 | ![Dk4i_0023](images/Dk4i_0023.png) | 541 | 5.41 % | 4.98–5.87 % | 5.41 % |
| Dk4i_0010 | Group 5 | ![Dk4i_0010](images/Dk4i_0010.png) | 502 | 5.02 % | 4.61–5.47 % | 5.02 % |
| Dk4i_0022 | Group 3 | ![Dk4i_0022](images/Dk4i_0022.png) | 495 | 4.95 % | 4.54–5.39 % | 4.95 % |
| Dk4i_0017 | Group 7 | ![Dk4i_0017](images/Dk4i_0017.png) | 456 | 4.56 % | 4.17–4.99 % | 4.56 % |
| Dk4i_0016 | Group 8 | ![Dk4i_0016](images/Dk4i_0016.png) | 445 | 4.45 % | 4.06–4.87 % | 4.45 % |
| Dk4i_0008 | Group 9 | ![Dk4i_0008](images/Dk4i_0008.png) | 440 | 4.40 % | 4.02–4.82 % | 4.40 % |
| Dk4i_0020 | Group 3 | ![Dk4i_0020](images/Dk4i_0020.png) | 425 | 4.25 % | 3.87–4.66 % | 4.25 % |
| Dk4i_0007 | Group 10 | ![Dk4i_0007](images/Dk4i_0007.png) | 405 | 4.05 % | 3.68–4.45 % | 4.05 % |
| Dk4i_0014 | Group 11 | ![Dk4i_0014](images/Dk4i_0014.png) | 405 | 4.05 % | 3.68–4.45 % | 4.05 % |
| Dk4i_0012 | Group 5 | ![Dk4i_0012](images/Dk4i_0012.png) | 403 | 4.03 % | 3.66–4.43 % | 4.03 % |
| Dk4i_0021 | Group 4 | ![Dk4i_0021](images/Dk4i_0021.png) | 370 | 3.70 % | 3.35–4.09 % | 3.70 % |
| Dk4i_0011 | Group 0 | ![Dk4i_0011](images/Dk4i_0011.png) | 366 | 3.66 % | 3.31–4.05 % | 3.66 % |
| Dk4i_0004 | Group 2 | ![Dk4i_0004](images/Dk4i_0004.png) | 360 | 3.60 % | 3.25–3.98 % | 3.60 % |
| Dk4i_0001 | Group 12 | ![Dk4i_0001](images/Dk4i_0001.png) | 325 | 3.25 % | 2.92–3.62 % | 3.25 % |
| Dk4i_0005 | Group 1 | ![Dk4i_0005](images/Dk4i_0005.png) | 315 | 3.15 % | 2.83–3.51 % | 3.15 % |
| Dk4i_0002 | Group 13 | ![Dk4i_0002](images/Dk4i_0002.png) | 281 | 2.81 % | 2.50–3.15 % | 2.81 % |
| Dk4i_0024 | Group 14 | ![Dk4i_0024](images/Dk4i_0024.png) | 280 | 2.80 % | 2.49–3.14 % | 2.80 % |
| Dk4i_0013 | Group 15 | ![Dk4i_0013](images/Dk4i_0013.png) | 275 | 2.75 % | 2.45–3.09 % | 2.75 % |
| Dk4i_0019 | Group 16 | ![Dk4i_0019](images/Dk4i_0019.png) | 268 | 2.68 % | 2.38–3.02 % | 2.68 % |
| Dk4i_0018 | Group 17 | ![Dk4i_0018](images/Dk4i_0018.png) | 264 | 2.64 % | 2.34–2.97 % | 2.64 % |

[Pose catalogue JSON](poses.json) · [Pose catalogue YAML](poses.yaml) · [Frequencies](frequencies.csv) · [Trial records](trials.csv)

Pose orientations use `xyzw` quaternions from the workpiece frame to the chute frame. Recognition uses the recorded symmetry, a 5° tolerance, and a 1° ambiguity margin. The pose registry reserves previously observed IDs for later recognition.

### Historical run files

- [Configuration](config.json)
- [Manifest](manifest.json)
