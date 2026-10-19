# Dk1i: grouped observed poses

1,000 completed drops; 998 settled. 8 assessed source poses; 6 groups meet the 1% cutoff.

Grouping uses 0.5 mm equivalent lift and a 60° maximum diameter. All members receive the same disturbance protocol.

| Representative | Image | Members | Combined count | Frequency | Retention AUC |
| --- | --- | --- | ---: | ---: | ---: |
| Dk1i_0002 | ![pose](images/Dk1i_0002.png) | Dk1i_0002, Dk1i_0004 | 368 | 36.80% | 1.0000 |
| Dk1i_0003 | ![pose](images/Dk1i_0003.png) | Dk1i_0003, Dk1i_0005 | 310 | 31.00% | 1.0000 |
| Dk1i_0007 | ![pose](images/Dk1i_0007.png) | Dk1i_0007 | 113 | 11.30% | 0.9792 |
| Dk1i_0006 | ![pose](images/Dk1i_0006.png) | Dk1i_0006 | 80 | 8.00% | 1.0000 |
| Dk1i_0001 | ![pose](images/Dk1i_0001.png) | Dk1i_0001 | 76 | 7.60% | 1.0000 |
| Dk1i_0008 | ![pose](images/Dk1i_0008.png) | Dk1i_0008 | 51 | 5.10% | 0.9792 |

[All original observations and member images](original_observations.json), [memberships](membership.csv), [barrier evidence](grouping_geometry.json), [member stability curves](group_stability.csv), [individual disturbance curves](stability.csv), [validation](validation.json).

Frequencies retain the original completed-drop denominator. Stability scores describe the configured virtual chute.

## Latest main-parameter rerun, 2026-10-19

Fresh **1,000 drops** using simulator main `2a0c74f5e3eb921cf6e6b5a54102203d01c34ae7` and its `configs/dk1i-1000.json` profile. Recognition anchors and source orientations come from stable poses main `fb055c61c79e789570712f13151aede036c14c51`; earlier counts are not reused.

Observation length 500 mm; chute 45°/0°; belt 100 ± 3 mm/s; contact damping ratio 0.19; 100 mm release height; seed 42; 16 independent workers. Weight impulses (Δv 49.05 mm/s) act during the first second. The belt stops over 0.2 s, followed by 2 s of rest observation. Grouping adds complete member disturbance assessments, including the 0.5 mm barrier level.

Stopped-belt observations: `{"enabled": true, "observed_trials": 1000, "settled_transport_then_unsettled": 1, "status_counts": {"settled": 999, "unsettled": 1}, "unsettled_transport_then_settled": 2}`. Transport frequencies and later rest observations remain separate. Roadmap pose numbers are assigned from current individual frequencies, so pose 0 can change between runs.

[All 1,000 raw trials](run_data/trials.jsonl.gz), [all member disturbance trials](run_data/group_disturbances.jsonl.gz), [run summary](run_data/summary.json), [stopped-belt table](run_data/stop_observations.csv), [exact provenance](simulation_provenance.json), [original main profile](main_profile.json).
