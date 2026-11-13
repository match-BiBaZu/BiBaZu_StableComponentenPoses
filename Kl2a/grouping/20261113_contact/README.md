# Kl2a: rounded support families

A rounded support family ignores circumferential roll while retaining the extrusion-axis direction and broad cut-feature supports. The pinned meshes use source Z as their extrusion axis. Axis alignment uses 10°, and broad-support normals use 5°. A side hull facet is broad when its area is at least twice the median side-strip area. Kk2i retains broad wall/belt support distinctions. Kl2a also merges end-on-belt azimuths. Kk4a retains the signed axis direction; tilted observations stay separate for review. This simple geometric classification does not claim a 0.5 mm energy barrier or add rotational recognition symmetry.

![Counts and seated heights](energy_basins.png)

| Group | Displayed poses | Drops | Incidence | Review | Saved orientation |
| --- | --- | ---: | ---: | --- | --- |
| 0 | 3, 5, 6, 8, 9, 10, 11, 12, 13, 14, 15, 17, 19 | 4729 | 47.29% | False | ![Kl2a_0009](../../images/Kl2a_0009.png) |
| 1 | 0, 2 | 2647 | 26.47% | False | ![Kl2a_0007](../../images/Kl2a_0007.png) |
| 2 | 1, 4 | 1802 | 18.02% | False | ![Kl2a_0008](../../images/Kl2a_0008.png) |
| 3 | 7, 22, 24 | 438 | 4.38% | False | ![Kl2a_0019](../../images/Kl2a_0019.png) |
| 4 | 16, 18, 21, 25 | 263 | 2.63% | False | ![Kl2a_0001](../../images/Kl2a_0001.png) |
| 5 | 20, 26 | 30 | 0.30% | False | ![Kl2a_0005](../../images/Kl2a_0005.png) |
| 6 | 23 | 3 | 0.03% | True | ![Kl2a_0025](../../images/Kl2a_0025.png) |

Illustrations use an existing frequent orientation, without claiming a stability representative.

[Per-pose axes, supporting normals and family signatures](grouping_evidence.json.gz) · [Provenance](provenance.json) · [Reproducible simulator patch](simulator.patch)

To reproduce, check out the simulator base revision in provenance, apply simulator.patch, and run the tests.
