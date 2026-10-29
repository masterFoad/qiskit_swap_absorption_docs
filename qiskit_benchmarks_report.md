# Quality report — confirm-profile

Gate: **improved** — quality improved with every quality check passing

Quality checks: **PASS**. This is a quality-stage snapshot; run `decide` for the final benchmark verdict, including Benchpress.

Per-case quality cap: 2.00× (seed-aggregated; rule: plain).

Quality guard tolerances: family/level 5.0%, individual guards 15.0% (statistical margins beyond 3 SE); ordinary deterministic cases 25.0% on each seed. Overall N2 and basis-panel guards retain zero margin; zero-baseline and canary checks remain strict.

Overall scores cover the primary scored panel using frozen weights. Family and other marginal scores normalize those weights within their scored subset. Ratios below 1 improve on baseline; paired standard errors are in log space. The trade score is descriptive and does not determine the gate.

## Check results

| Result | Count |
| --- | ---: |
| passed | 213 |

## Checks needing attention

None.

## Quality stage improvement

Primary D2 ratio: 0.960719 (paired SE 0.000439; upper 2 SE log effect -0.039196).

Review trade score sqrt(D2 ratio × N2 ratio): 0.966104.

Primary scored-panel improvement is 100 × (1 − ratio), using the benchmark's weighted geometric ratios. Positive percentages mean improvement (lower is better); negative percentages mean regression. These are point estimates: the record named on each line judges its ratio against the paired standard error.

- Primary D2 improvement: +3.93%. Improvement rule `CA2/improvement`: passed.
- Primary N2 improvement: +2.85%. Guard `CA3/primary/N2`: passed.

## Quality tests

One row per quality test, including guards. D2 (two-qubit depth) and N2 (two-qubit gate count) are arithmetic means over the test's frozen B0 seeds. Each improvement is 100 × (baseline mean − evolved mean) / baseline mean. These descriptive means do not change the verdict or its weighted geometric estimates, and can differ slightly from the geometric ratios under Per-case changes.

Missing or invalid seed pairs make that metric unavailable. Percentages with a zero baseline are N/A (undefined). Seeds is the expected count per revision.

| Test | Seeds | Baseline D2 | Evolved D2 | D2 improvement | Baseline N2 | Evolved N2 | N2 improvement |
| --- | ---: | ---: | ---: | ---: | ---: | ---: | ---: |
| confirm/qft_n100/heavy_hex_d9_cz/L2 | 100 | 1823.86 | 1713.45 | +6.05% | 9563.88 | 8997.68 | +5.92% |
| confirm/qft_n100/heavy_hex_d9_cz/L3 | 100 | 1774.65 | 1649.40 | +7.06% | 9310.16 | 8745.56 | +6.06% |
| confirm/qft_cp_n14/melbourne_14_u/L2 | 100 | 120.27 | 102.30 | +14.94% | 281.29 | 249.33 | +11.36% |
| confirm/qft_cp_n14/melbourne_14_u/L3 | 100 | 118.76 | 100.37 | +15.49% | 281.33 | 249.15 | +11.44% |
| confirm/qft_full_n32/rochester_53/L2 | 100 | 380.89 | 342.30 | +10.13% | 1576.01 | 1493.23 | +5.25% |
| confirm/qft_full_n32/rochester_53/L3 | 100 | 355.54 | 318.16 | +10.51% | 1517.74 | 1441.86 | +5.00% |
| confirm/qft_cp_n8/melbourne_14_u/L2 | 100 | 51.62 | 48.57 | +5.91% | 81.28 | 74.96 | +7.78% |
| confirm/qft_cp_n8/melbourne_14_u/L3 | 100 | 47.31 | 44.80 | +5.31% | 78.21 | 73.05 | +6.60% |
| confirm/qft_full_n64/heavy_hex_d9_cz/L2 | 100 | 885.99 | 804.15 | +9.24% | 4534.05 | 4255.63 | +6.14% |
| confirm/qft_full_n64/heavy_hex_d9_cz/L3 | 100 | 862.98 | 772.23 | +10.52% | 4414.19 | 4140.39 | +6.20% |
| confirm/qft16_cancel/mumbai_27/L2 | 10 | 0.00 | 0.00 | N/A | 0.00 | 0.00 | N/A |
| confirm/qft16_cancel/mumbai_27/L3 | 10 | 0.00 | 0.00 | N/A | 0.00 | 0.00 | N/A |
| confirm/square_heisenberg_n100/heavy_hex_d9_cz/L2 | 100 | 401.94 | 401.94 | +0.00% | 1823.88 | 1823.88 | +0.00% |
| confirm/square_heisenberg_n100/heavy_hex_d9_cz/L3 | 100 | 355.71 | 355.71 | +0.00% | 1608.93 | 1608.93 | +0.00% |
| confirm/trotter_chain_n32/rochester_53/L2 | 10 | 178.00 | 178.00 | +0.00% | 1860.00 | 1860.00 | +0.00% |
| confirm/trotter_chain_n32/rochester_53/L3 | 10 | 178.00 | 178.00 | +0.00% | 1860.00 | 1860.00 | +0.00% |
| confirm/trotter_chain_n16/mumbai_27/L2 | 10 | 146.00 | 146.00 | +0.00% | 900.00 | 900.00 | +0.00% |
| confirm/trotter_chain_n16/mumbai_27/L3 | 10 | 146.00 | 146.00 | +0.00% | 900.00 | 900.00 | +0.00% |
| confirm/dtc_n100/heavy_hex_d9_cz/L2 | 10 | 400.00 | 400.00 | +0.00% | 19800.00 | 19800.00 | +0.00% |
| confirm/dtc_n100/heavy_hex_d9_cz/L3 | 10 | 400.00 | 400.00 | +0.00% | 19800.00 | 19800.00 | +0.00% |
| confirm/qaoa_ba_n100_3reps/heavy_hex_d9_cz/L2 | 100 | 1531.56 | 1502.86 | +1.87% | 8610.32 | 8527.66 | +0.96% |
| confirm/qaoa_ba_n100_3reps/heavy_hex_d9_cz/L3 | 100 | 1517.19 | 1489.27 | +1.84% | 8522.37 | 8438.47 | +0.98% |
| confirm/qaoa_complete_n8/mumbai_27/L2 | 100 | 497.24 | 415.37 | +16.46% | 787.62 | 681.88 | +13.43% |
| confirm/qaoa_complete_n8/mumbai_27/L3 | 100 | 498.85 | 416.13 | +16.58% | 788.26 | 682.08 | +13.47% |
| confirm/qaoa_complete_n16/mumbai_27/L2 | 100 | 1106.06 | 915.85 | +17.20% | 3750.94 | 3394.48 | +9.50% |
| confirm/qaoa_complete_n16/mumbai_27/L3 | 100 | 1115.30 | 927.65 | +16.83% | 3769.04 | 3409.60 | +9.54% |
| confirm/qaoa_complete_n32/rochester_53/L2 | 100 | 2176.55 | 1873.09 | +13.94% | 15163.06 | 14519.02 | +4.25% |
| confirm/qaoa_complete_n32/rochester_53/L3 | 100 | 2218.45 | 1910.05 | +13.90% | 15195.46 | 14538.58 | +4.32% |
| confirm/qv_n50_d50/heavy_hex_d9_cz/L2 | 100 | 2560.56 | 2560.56 | +0.00% | 16200.54 | 16200.54 | +0.00% |
| confirm/qv_n50_d50/heavy_hex_d9_cz/L3 | 100 | 2556.63 | 2556.63 | +0.00% | 16195.44 | 16195.44 | +0.00% |
| confirm/qv_n14_d14/melbourne_14/L2 | 100 | 187.74 | 187.74 | +0.00% | 532.05 | 532.05 | +0.00% |
| confirm/qv_n14_d14/melbourne_14/L3 | 100 | 191.49 | 191.49 | +0.00% | 533.52 | 533.52 | +0.00% |
| confirm/qv_n27_d27/mumbai_27_loose/L2 | 100 | 722.76 | 722.76 | +0.00% | 3083.61 | 3083.61 | +0.00% |
| confirm/qv_n27_d27/mumbai_27_loose/L3 | 100 | 722.10 | 722.10 | +0.00% | 3093.36 | 3093.36 | +0.00% |
| confirm/qv_n50_d20/rochester_53_u/L2 | 100 | 996.69 | 996.69 | +0.00% | 6392.25 | 6392.25 | +0.00% |
| confirm/qv_n50_d20/rochester_53_u/L3 | 100 | 988.65 | 988.65 | +0.00% | 6388.38 | 6388.38 | +0.00% |
| confirm/qv_n14_d14_s10/mumbai_27_loose/L2 | 100 | 180.99 | 180.99 | +0.00% | 575.55 | 575.55 | +0.00% |
| confirm/qv_n14_d14_s10/mumbai_27_loose/L3 | 100 | 178.47 | 178.47 | +0.00% | 572.97 | 572.97 | +0.00% |
| confirm/ripple_adder_10/grid_5x5_u/L2 | 100 | 206.02 | 205.98 | +0.02% | 349.95 | 349.91 | +0.01% |
| confirm/ripple_adder_10/grid_5x5_u/L3 | 100 | 201.73 | 201.73 | +0.00% | 347.77 | 347.77 | +0.00% |
| confirm/mcx_kg24_n6/mumbai_27/L2 | 100 | 23.85 | 23.85 | +0.00% | 27.04 | 27.04 | +0.00% |
| confirm/mcx_kg24_n6/mumbai_27/L3 | 100 | 23.85 | 23.85 | +0.00% | 27.04 | 27.04 | +0.00% |
| confirm/mcx_kg24_n5/mumbai_27/L2 | 10 | 14.00 | 14.00 | +0.00% | 15.00 | 15.00 | +0.00% |
| confirm/mcx_kg24_n5/mumbai_27/L3 | 10 | 14.00 | 14.00 | +0.00% | 15.00 | 15.00 | +0.00% |
| confirm/multiplier_h18_n32/rochester_53/L2 | 100 | 6048.58 | 6035.75 | +0.21% | 8394.16 | 8376.34 | +0.21% |
| confirm/multiplier_h18_n32/rochester_53/L3 | 100 | 6044.97 | 6032.45 | +0.21% | 8383.71 | 8366.35 | +0.21% |
| confirm/mcx_kg24_n16/mumbai_27/L2 | 100 | 117.85 | 117.85 | +0.00% | 166.39 | 166.39 | +0.00% |
| confirm/mcx_kg24_n16/mumbai_27/L3 | 100 | 117.81 | 117.81 | +0.00% | 166.08 | 166.08 | +0.00% |
| confirm/ripple_adder_20/grid_7x7_u/L2 | 100 | 460.54 | 460.49 | +0.01% | 797.93 | 797.87 | +0.01% |
| confirm/ripple_adder_20/grid_7x7_u/L3 | 100 | 450.97 | 450.97 | +0.00% | 786.23 | 786.23 | +0.00% |
| confirm/adder_modular_v17_n8/mumbai_27/L2 | 100 | 70.86 | 69.49 | +1.93% | 89.92 | 88.40 | +1.69% |
| confirm/adder_modular_v17_n8/mumbai_27/L3 | 100 | 70.70 | 69.28 | +2.01% | 89.90 | 88.38 | +1.69% |
| confirm/adder_modular_v17_n16/mumbai_27/L2 | 100 | 249.74 | 244.20 | +2.22% | 295.64 | 290.00 | +1.91% |
| confirm/adder_modular_v17_n16/mumbai_27/L3 | 100 | 246.96 | 241.87 | +2.06% | 289.36 | 284.28 | +1.76% |
| confirm/adder_modular_v17_n32/rochester_53/L2 | 100 | 602.65 | 588.64 | +2.32% | 723.80 | 709.66 | +1.95% |
| confirm/adder_modular_v17_n32/rochester_53/L3 | 100 | 587.11 | 573.02 | +2.40% | 702.23 | 688.09 | +2.01% |
| confirm/multiplier_h18_n16/mumbai_27/L2 | 100 | 1387.24 | 1382.16 | +0.37% | 1804.00 | 1798.14 | +0.32% |
| confirm/multiplier_h18_n16/mumbai_27/L3 | 100 | 1387.54 | 1382.85 | +0.34% | 1801.02 | 1795.42 | +0.31% |
| confirm/adder_modular_v17_n6/mumbai_27/L2 | 100 | 40.92 | 40.48 | +1.08% | 45.66 | 45.32 | +0.74% |
| confirm/adder_modular_v17_n6/mumbai_27/L3 | 100 | 40.93 | 40.50 | +1.05% | 45.66 | 45.32 | +0.74% |
| confirm/multiplier_h18_n20/heavy_hex_d9_cz/L2 | 100 | 2296.48 | 2290.94 | +0.24% | 3092.73 | 3087.58 | +0.17% |
| confirm/bv_all_ones_n100/heavy_hex_d9_cz/L2 | 100 | 649.53 | 626.83 | +3.49% | 802.43 | 779.29 | +2.88% |
| confirm/bv_all_ones_n100/heavy_hex_d9_cz/L3 | 100 | 563.25 | 538.36 | +4.42% | 660.38 | 635.14 | +3.82% |
| confirm/bv_all_ones_n16/mumbai_27/L2 | 100 | 49.34 | 42.38 | +14.11% | 53.50 | 46.88 | +12.37% |
| confirm/bv_all_ones_n16/mumbai_27/L3 | 100 | 49.53 | 42.95 | +13.28% | 53.34 | 47.16 | +11.59% |
| confirm/bv_all_ones_n50/rochester_53/L2 | 100 | 192.02 | 176.50 | +8.08% | 196.86 | 181.14 | +7.99% |
| confirm/bv_all_ones_n50/rochester_53/L3 | 100 | 193.78 | 177.35 | +8.48% | 199.74 | 182.86 | +8.45% |
| confirm/bvlike_n100/heavy_hex_d9_cz/L2 | 10 | 0.00 | 0.00 | N/A | 0.00 | 0.00 | N/A |
| confirm/bvlike_n100/heavy_hex_d9_cz/L3 | 10 | 0.00 | 0.00 | N/A | 0.00 | 0.00 | N/A |
| confirm/su2_circular_n89/heavy_hex_d9_cz/L2 | 100 | 1400.54 | 1400.54 | +0.00% | 1640.53 | 1640.53 | +0.00% |
| confirm/su2_circular_n89/heavy_hex_d9_cz/L3 | 10 | 1239.60 | 1239.60 | +0.00% | 1419.30 | 1419.30 | +0.00% |
| confirm/ring_random_n8/melbourne_14_u/L2 | 10 | 16.00 | 16.00 | +0.00% | 64.00 | 64.00 | +0.00% |
| confirm/ring_random_n8/melbourne_14_u/L3 | 10 | 16.00 | 16.00 | +0.00% | 64.00 | 64.00 | +0.00% |
| confirm/ring_random_n14/melbourne_14_u/L2 | 10 | 84.00 | 84.00 | +0.00% | 280.00 | 280.00 | +0.00% |
| confirm/ring_random_n14/melbourne_14_u/L3 | 10 | 84.00 | 84.00 | +0.00% | 280.00 | 280.00 | +0.00% |
| confirm/su2_circular_n100/heavy_hex_d9_cz/L2 | 10 | 300.00 | 300.00 | +0.00% | 300.00 | 300.00 | +0.00% |
| confirm/su2_circular_n100/heavy_hex_d9_cz/L3 | 10 | 300.00 | 300.00 | +0.00% | 300.00 | 300.00 | +0.00% |
| confirm/queko_bss_53+sabre/rochester_53/L2 | 100 | 230.24 | 229.12 | +0.49% | 1104.81 | 1100.47 | +0.39% |
| confirm/queko_bss_53+sabre/rochester_53/L3 | 100 | 197.72 | 196.53 | +0.60% | 947.11 | 940.97 | +0.65% |
| confirm/queko_bigd_20+sabre/tokyo_20/L2 | 100 | 20.39 | 20.20 | +0.93% | 21.72 | 21.48 | +1.10% |
| confirm/queko_bigd_20+sabre/tokyo_20/L3 | 100 | 19.77 | 19.54 | +1.16% | 21.25 | 20.93 | +1.51% |
| confirm/queko_bntf_54+sabre/sycamore_54/L2 | 100 | 96.73 | 95.82 | +0.94% | 486.45 | 480.57 | +1.21% |
| confirm/queko_bntf_54+sabre/sycamore_54/L3 | 100 | 84.06 | 83.22 | +1.00% | 441.75 | 435.95 | +1.31% |
| confirm/queko_bss_53/rochester_53/L2 | 10 | 46.00 | 46.00 | +0.00% | 363.00 | 363.00 | +0.00% |
| confirm/queko_bss_53/rochester_53/L3 | 10 | 46.00 | 46.00 | +0.00% | 355.00 | 355.00 | +0.00% |
| confirm/queko_bigd_20/tokyo_20/L2 | 10 | 17.00 | 17.00 | +0.00% | 17.00 | 17.00 | +0.00% |
| confirm/queko_bigd_20/tokyo_20/L3 | 10 | 17.00 | 17.00 | +0.00% | 17.00 | 17.00 | +0.00% |
| confirm/queko_bntf_54/sycamore_54/L2 | 10 | 18.00 | 18.00 | +0.00% | 172.00 | 172.00 | +0.00% |
| confirm/queko_bntf_54/sycamore_54/L3 | 10 | 18.00 | 18.00 | +0.00% | 172.00 | 172.00 | +0.00% |
| confirm/long_2q_sequence/rochester_53_u/L2 | 10 | 3.00 | 3.00 | +0.00% | 3.00 | 3.00 | +0.00% |
| confirm/long_2q_sequence/rochester_53_u/L3 | 10 | 3.00 | 3.00 | +0.00% | 3.00 | 3.00 | +0.00% |
| confirm/a2a_qft_n16/a2a_clifford_rz_16/L2 | 10 | 58.00 | 58.00 | +0.00% | 238.00 | 238.00 | +0.00% |
| confirm/a2a_qft_n16/a2a_clifford_rz_16/L3 | 10 | 58.00 | 58.00 | +0.00% | 238.00 | 238.00 | +0.00% |
| confirm/a2a_trotter_n16/a2a_clifford_rz_16/L2 | 10 | 146.00 | 146.00 | +0.00% | 900.00 | 900.00 | +0.00% |
| confirm/a2a_trotter_n16/a2a_clifford_rz_16/L3 | 10 | 146.00 | 146.00 | +0.00% | 900.00 | 900.00 | +0.00% |
| confirm/a2a_qaoa_n16/a2a_clifford_rz_16/L2 | 10 | 324.00 | 324.00 | +0.00% | 2100.00 | 2100.00 | +0.00% |
| confirm/a2a_qaoa_n16/a2a_clifford_rz_16/L3 | 10 | 324.00 | 324.00 | +0.00% | 2100.00 | 2100.00 | +0.00% |
| confirm/a2a_multiplier_n16/a2a_clifford_rz_16/L2 | 10 | 696.00 | 696.00 | +0.00% | 794.00 | 794.00 | +0.00% |
| confirm/a2a_multiplier_n16/a2a_clifford_rz_16/L3 | 10 | 696.00 | 696.00 | +0.00% | 794.00 | 794.00 | +0.00% |
| confirm/a2a_adder_modular_n16/a2a_clifford_rz_16/L2 | 10 | 107.00 | 107.00 | +0.00% | 113.00 | 113.00 | +0.00% |
| confirm/a2a_adder_modular_n16/a2a_clifford_rz_16/L3 | 10 | 107.00 | 107.00 | +0.00% | 113.00 | 113.00 | +0.00% |
| confirm/a2a_mcx_n16/a2a_clifford_rz_16/L2 | 10 | 68.00 | 68.00 | +0.00% | 78.00 | 78.00 | +0.00% |
| confirm/a2a_mcx_n16/a2a_clifford_rz_16/L3 | 10 | 68.00 | 68.00 | +0.00% | 78.00 | 78.00 | +0.00% |
| confirm/qft_n100/heavy_hex_d9_cx/L2 | 100 | 1807.94 | 1702.67 | +5.82% | 9497.08 | 8957.60 | +5.68% |
| confirm/qft_n100/heavy_hex_d9_ecr/L2 | 100 | 1823.86 | 1713.45 | +6.05% | 9563.88 | 8997.68 | +5.92% |
| confirm/square_heisenberg_n100/heavy_hex_d9_cx/L2 | 100 | 401.94 | 401.94 | +0.00% | 1823.88 | 1823.88 | +0.00% |
| confirm/square_heisenberg_n100/heavy_hex_d9_ecr/L2 | 100 | 401.94 | 401.94 | +0.00% | 1823.88 | 1823.88 | +0.00% |
| confirm/qaoa_ba_n100_3reps/heavy_hex_d9_cx/L2 | 100 | 1526.66 | 1502.58 | +1.58% | 8591.44 | 8525.92 | +0.76% |
| confirm/qaoa_ba_n100_3reps/heavy_hex_d9_ecr/L2 | 100 | 1531.56 | 1502.86 | +1.87% | 8610.32 | 8527.66 | +0.96% |

## Quality runtime

Fresh sequential timing runs cover the same quality cases and B0 seeds on both builds. Each worker warms up once before timing uninstrumented transpile calls; imports, fixture loading, export and checks are excluded. Machine load is neither checked nor corrected. Stored baseline quality results do not supply runtime samples.

Runtime differences are evolved − baseline; negative differences mean faster. Improvement is 100 × (baseline − evolved) / baseline. Runtime regressions are reported without an acceptance threshold.

Full-panel measured runtime (7390 seeds per revision): baseline **3304.823311 s**, evolved **3357.968575 s**; difference **+53.145264 s** (-1.61% improvement).

Equal-case geometric mean runtime ratio: 1.013023×.

Paired seeds: 7390 / 7390; missing samples: 0; failed samples: 0.

Per-case times are arithmetic means over the complete frozen seed block.

| Test | Seeds | Baseline (s) | Evolved (s) | Difference (s) | Runtime improvement |
| --- | ---: | ---: | ---: | ---: | ---: |
| confirm/qft_n100/heavy_hex_d9_cz/L2 | 100 | 0.955589 | 0.970893 | +0.015303 | -1.60% |
| confirm/qft_n100/heavy_hex_d9_cz/L3 | 100 | 1.303819 | 1.383770 | +0.079951 | -6.13% |
| confirm/qft_cp_n14/melbourne_14_u/L2 | 100 | 0.021441 | 0.024378 | +0.002937 | -13.70% |
| confirm/qft_cp_n14/melbourne_14_u/L3 | 100 | 0.026645 | 0.026875 | +0.000230 | -0.86% |
| confirm/qft_full_n32/rochester_53/L2 | 100 | 0.157660 | 0.159701 | +0.002040 | -1.29% |
| confirm/qft_full_n32/rochester_53/L3 | 100 | 0.204715 | 0.198249 | -0.006466 | +3.16% |
| confirm/qft_cp_n8/melbourne_14_u/L2 | 100 | 0.007935 | 0.008161 | +0.000226 | -2.85% |
| confirm/qft_cp_n8/melbourne_14_u/L3 | 100 | 0.008917 | 0.008764 | -0.000153 | +1.72% |
| confirm/qft_full_n64/heavy_hex_d9_cz/L2 | 100 | 0.483742 | 0.480710 | -0.003032 | +0.63% |
| confirm/qft_full_n64/heavy_hex_d9_cz/L3 | 100 | 0.783389 | 0.790074 | +0.006685 | -0.85% |
| confirm/qft16_cancel/mumbai_27/L2 | 10 | 0.005139 | 0.004750 | -0.000389 | +7.57% |
| confirm/qft16_cancel/mumbai_27/L3 | 10 | 0.004980 | 0.004860 | -0.000120 | +2.41% |
| confirm/square_heisenberg_n100/heavy_hex_d9_cz/L2 | 100 | 0.176920 | 0.179957 | +0.003037 | -1.72% |
| confirm/square_heisenberg_n100/heavy_hex_d9_cz/L3 | 100 | 0.270471 | 0.271464 | +0.000993 | -0.37% |
| confirm/trotter_chain_n32/rochester_53/L2 | 10 | 0.033710 | 0.033332 | -0.000377 | +1.12% |
| confirm/trotter_chain_n32/rochester_53/L3 | 10 | 0.060049 | 0.059400 | -0.000648 | +1.08% |
| confirm/trotter_chain_n16/mumbai_27/L2 | 10 | 0.018472 | 0.017876 | -0.000596 | +3.23% |
| confirm/trotter_chain_n16/mumbai_27/L3 | 10 | 0.036699 | 0.036876 | +0.000177 | -0.48% |
| confirm/dtc_n100/heavy_hex_d9_cz/L2 | 10 | 0.546620 | 0.545784 | -0.000836 | +0.15% |
| confirm/dtc_n100/heavy_hex_d9_cz/L3 | 10 | 1.496854 | 1.518727 | +0.021872 | -1.46% |
| confirm/qaoa_ba_n100_3reps/heavy_hex_d9_cz/L2 | 100 | 0.776214 | 0.786535 | +0.010321 | -1.33% |
| confirm/qaoa_ba_n100_3reps/heavy_hex_d9_cz/L3 | 100 | 1.088510 | 1.093688 | +0.005178 | -0.48% |
| confirm/qaoa_complete_n8/mumbai_27/L2 | 100 | 0.032564 | 0.033369 | +0.000805 | -2.47% |
| confirm/qaoa_complete_n8/mumbai_27/L3 | 100 | 0.052404 | 0.052608 | +0.000204 | -0.39% |
| confirm/qaoa_complete_n16/mumbai_27/L2 | 100 | 0.265186 | 0.272246 | +0.007060 | -2.66% |
| confirm/qaoa_complete_n16/mumbai_27/L3 | 100 | 0.393726 | 0.376001 | -0.017725 | +4.50% |
| confirm/qaoa_complete_n32/rochester_53/L2 | 100 | 1.431904 | 1.459486 | +0.027582 | -1.93% |
| confirm/qaoa_complete_n32/rochester_53/L3 | 100 | 1.735604 | 1.740358 | +0.004754 | -0.27% |
| confirm/qv_n50_d50/heavy_hex_d9_cz/L2 | 100 | 1.944265 | 1.976740 | +0.032474 | -1.67% |
| confirm/qv_n50_d50/heavy_hex_d9_cz/L3 | 100 | 2.608864 | 2.611257 | +0.002393 | -0.09% |
| confirm/qv_n14_d14/melbourne_14/L2 | 100 | 0.040962 | 0.040699 | -0.000263 | +0.64% |
| confirm/qv_n14_d14/melbourne_14/L3 | 100 | 0.056140 | 0.055847 | -0.000293 | +0.52% |
| confirm/qv_n27_d27/mumbai_27_loose/L2 | 100 | 0.263338 | 0.265645 | +0.002307 | -0.88% |
| confirm/qv_n27_d27/mumbai_27_loose/L3 | 100 | 0.311663 | 0.312957 | +0.001294 | -0.42% |
| confirm/qv_n50_d20/rochester_53_u/L2 | 100 | 0.690500 | 0.700665 | +0.010165 | -1.47% |
| confirm/qv_n50_d20/rochester_53_u/L3 | 100 | 0.823548 | 0.825520 | +0.001972 | -0.24% |
| confirm/qv_n14_d14_s10/mumbai_27_loose/L2 | 100 | 0.042810 | 0.043317 | +0.000507 | -1.18% |
| confirm/qv_n14_d14_s10/mumbai_27_loose/L3 | 100 | 0.053222 | 0.052790 | -0.000432 | +0.81% |
| confirm/ripple_adder_10/grid_5x5_u/L2 | 100 | 0.020851 | 0.021616 | +0.000765 | -3.67% |
| confirm/ripple_adder_10/grid_5x5_u/L3 | 100 | 0.023988 | 0.025039 | +0.001052 | -4.38% |
| confirm/mcx_kg24_n6/mumbai_27/L2 | 100 | 0.004719 | 0.004667 | -0.000052 | +1.10% |
| confirm/mcx_kg24_n6/mumbai_27/L3 | 100 | 0.004995 | 0.005146 | +0.000151 | -3.03% |
| confirm/mcx_kg24_n5/mumbai_27/L2 | 10 | 0.004180 | 0.004218 | +0.000037 | -0.90% |
| confirm/mcx_kg24_n5/mumbai_27/L3 | 10 | 0.004352 | 0.005127 | +0.000775 | -17.80% |
| confirm/multiplier_h18_n32/rochester_53/L2 | 100 | 0.367558 | 0.391287 | +0.023729 | -6.46% |
| confirm/multiplier_h18_n32/rochester_53/L3 | 100 | 0.503897 | 0.501123 | -0.002774 | +0.55% |
| confirm/mcx_kg24_n16/mumbai_27/L2 | 100 | 0.011181 | 0.012009 | +0.000827 | -7.40% |
| confirm/mcx_kg24_n16/mumbai_27/L3 | 100 | 0.014594 | 0.015050 | +0.000456 | -3.13% |
| confirm/ripple_adder_20/grid_7x7_u/L2 | 100 | 0.045751 | 0.048926 | +0.003175 | -6.94% |
| confirm/ripple_adder_20/grid_7x7_u/L3 | 100 | 0.055438 | 0.057927 | +0.002489 | -4.49% |
| confirm/adder_modular_v17_n8/mumbai_27/L2 | 100 | 0.006779 | 0.007086 | +0.000308 | -4.54% |
| confirm/adder_modular_v17_n8/mumbai_27/L3 | 100 | 0.009838 | 0.009908 | +0.000069 | -0.70% |
| confirm/adder_modular_v17_n16/mumbai_27/L2 | 100 | 0.013274 | 0.013548 | +0.000274 | -2.06% |
| confirm/adder_modular_v17_n16/mumbai_27/L3 | 100 | 0.020717 | 0.020719 | +0.000001 | -0.01% |
| confirm/adder_modular_v17_n32/rochester_53/L2 | 100 | 0.026493 | 0.027716 | +0.001223 | -4.62% |
| confirm/adder_modular_v17_n32/rochester_53/L3 | 100 | 0.039122 | 0.032416 | -0.006706 | +17.14% |
| confirm/multiplier_h18_n16/mumbai_27/L2 | 100 | 0.087378 | 0.092125 | +0.004747 | -5.43% |
| confirm/multiplier_h18_n16/mumbai_27/L3 | 100 | 0.127788 | 0.129486 | +0.001698 | -1.33% |
| confirm/adder_modular_v17_n6/mumbai_27/L2 | 100 | 0.005061 | 0.005331 | +0.000270 | -5.34% |
| confirm/adder_modular_v17_n6/mumbai_27/L3 | 100 | 0.005557 | 0.005700 | +0.000143 | -2.58% |
| confirm/multiplier_h18_n20/heavy_hex_d9_cz/L2 | 100 | 0.168734 | 0.180200 | +0.011466 | -6.80% |
| confirm/bv_all_ones_n100/heavy_hex_d9_cz/L2 | 100 | 0.071935 | 0.073873 | +0.001938 | -2.69% |
| confirm/bv_all_ones_n100/heavy_hex_d9_cz/L3 | 100 | 1.225538 | 1.291406 | +0.065867 | -5.37% |
| confirm/bv_all_ones_n16/mumbai_27/L2 | 100 | 0.005838 | 0.005931 | +0.000093 | -1.59% |
| confirm/bv_all_ones_n16/mumbai_27/L3 | 100 | 0.006550 | 0.006677 | +0.000127 | -1.94% |
| confirm/bv_all_ones_n50/rochester_53/L2 | 100 | 0.015046 | 0.015586 | +0.000541 | -3.59% |
| confirm/bv_all_ones_n50/rochester_53/L3 | 100 | 0.017059 | 0.017564 | +0.000506 | -2.96% |
| confirm/bvlike_n100/heavy_hex_d9_cz/L2 | 10 | 0.008367 | 0.008375 | +0.000008 | -0.10% |
| confirm/bvlike_n100/heavy_hex_d9_cz/L3 | 10 | 0.008823 | 0.008990 | +0.000167 | -1.90% |
| confirm/su2_circular_n89/heavy_hex_d9_cz/L2 | 100 | 5.357715 | 5.487209 | +0.129494 | -2.42% |
| confirm/su2_circular_n89/heavy_hex_d9_cz/L3 | 10 | 33.673165 | 33.681681 | +0.008516 | -0.03% |
| confirm/ring_random_n8/melbourne_14_u/L2 | 10 | 0.004711 | 0.004785 | +0.000074 | -1.56% |
| confirm/ring_random_n8/melbourne_14_u/L3 | 10 | 0.005056 | 0.005470 | +0.000414 | -8.19% |
| confirm/ring_random_n14/melbourne_14_u/L2 | 10 | 0.015278 | 0.016048 | +0.000770 | -5.04% |
| confirm/ring_random_n14/melbourne_14_u/L3 | 10 | 0.017578 | 0.018071 | +0.000493 | -2.80% |
| confirm/su2_circular_n100/heavy_hex_d9_cz/L2 | 10 | 0.024137 | 0.024028 | -0.000109 | +0.45% |
| confirm/su2_circular_n100/heavy_hex_d9_cz/L3 | 10 | 0.512467 | 0.502123 | -0.010344 | +2.02% |
| confirm/queko_bss_53+sabre/rochester_53/L2 | 100 | 0.129885 | 0.132437 | +0.002552 | -1.96% |
| confirm/queko_bss_53+sabre/rochester_53/L3 | 100 | 0.148711 | 0.153096 | +0.004385 | -2.95% |
| confirm/queko_bigd_20+sabre/tokyo_20/L2 | 100 | 0.005057 | 0.005146 | +0.000089 | -1.76% |
| confirm/queko_bigd_20+sabre/tokyo_20/L3 | 100 | 0.005524 | 0.005407 | -0.000117 | +2.11% |
| confirm/queko_bntf_54+sabre/sycamore_54/L2 | 100 | 0.079413 | 0.080686 | +0.001273 | -1.60% |
| confirm/queko_bntf_54+sabre/sycamore_54/L3 | 100 | 0.087910 | 0.087821 | -0.000090 | +0.10% |
| confirm/queko_bss_53/rochester_53/L2 | 10 | 0.012925 | 0.013128 | +0.000203 | -1.57% |
| confirm/queko_bss_53/rochester_53/L3 | 10 | 0.016359 | 0.016311 | -0.000048 | +0.29% |
| confirm/queko_bigd_20/tokyo_20/L2 | 10 | 0.004268 | 0.004412 | +0.000144 | -3.38% |
| confirm/queko_bigd_20/tokyo_20/L3 | 10 | 0.004558 | 0.004546 | -0.000012 | +0.27% |
| confirm/queko_bntf_54/sycamore_54/L2 | 10 | 0.009510 | 0.009304 | -0.000207 | +2.17% |
| confirm/queko_bntf_54/sycamore_54/L3 | 10 | 0.010167 | 0.010625 | +0.000458 | -4.51% |
| confirm/long_2q_sequence/rochester_53_u/L2 | 10 | 0.006049 | 0.006627 | +0.000578 | -9.56% |
| confirm/long_2q_sequence/rochester_53_u/L3 | 10 | 0.006797 | 0.006660 | -0.000137 | +2.02% |
| confirm/a2a_qft_n16/a2a_clifford_rz_16/L2 | 10 | 0.008015 | 0.008077 | +0.000062 | -0.78% |
| confirm/a2a_qft_n16/a2a_clifford_rz_16/L3 | 10 | 0.011445 | 0.010900 | -0.000545 | +4.76% |
| confirm/a2a_trotter_n16/a2a_clifford_rz_16/L2 | 10 | 0.024654 | 0.024377 | -0.000276 | +1.12% |
| confirm/a2a_trotter_n16/a2a_clifford_rz_16/L3 | 10 | 0.035023 | 0.034210 | -0.000812 | +2.32% |
| confirm/a2a_qaoa_n16/a2a_clifford_rz_16/L2 | 10 | 0.038761 | 0.038037 | -0.000724 | +1.87% |
| confirm/a2a_qaoa_n16/a2a_clifford_rz_16/L3 | 10 | 0.063565 | 0.062168 | -0.001396 | +2.20% |
| confirm/a2a_multiplier_n16/a2a_clifford_rz_16/L2 | 10 | 0.040185 | 0.039517 | -0.000667 | +1.66% |
| confirm/a2a_multiplier_n16/a2a_clifford_rz_16/L3 | 10 | 0.072467 | 0.068013 | -0.004454 | +6.15% |
| confirm/a2a_adder_modular_n16/a2a_clifford_rz_16/L2 | 10 | 0.005072 | 0.005441 | +0.000369 | -7.27% |
| confirm/a2a_adder_modular_n16/a2a_clifford_rz_16/L3 | 10 | 0.007531 | 0.007549 | +0.000018 | -0.24% |
| confirm/a2a_mcx_n16/a2a_clifford_rz_16/L2 | 10 | 0.004653 | 0.004954 | +0.000301 | -6.47% |
| confirm/a2a_mcx_n16/a2a_clifford_rz_16/L3 | 10 | 0.007393 | 0.006790 | -0.000602 | +8.15% |
| confirm/qft_n100/heavy_hex_d9_cx/L2 | 100 | 0.891461 | 0.921565 | +0.030104 | -3.38% |
| confirm/qft_n100/heavy_hex_d9_ecr/L2 | 100 | 0.908930 | 0.945880 | +0.036950 | -4.07% |
| confirm/square_heisenberg_n100/heavy_hex_d9_cx/L2 | 100 | 0.174477 | 0.181198 | +0.006722 | -3.85% |
| confirm/square_heisenberg_n100/heavy_hex_d9_ecr/L2 | 100 | 0.176182 | 0.177758 | +0.001576 | -0.89% |
| confirm/qaoa_ba_n100_3reps/heavy_hex_d9_cx/L2 | 100 | 0.735826 | 0.738975 | +0.003149 | -0.43% |
| confirm/qaoa_ba_n100_3reps/heavy_hex_d9_ecr/L2 | 100 | 0.741794 | 0.753505 | +0.011711 | -1.58% |

## Quality estimates

| Panel | Ratio | Paired SE (log) | Upper 2 SE | Seeds |
| --- | ---: | ---: | ---: | ---: |
| CA2/improvement | 0.960719 | 0.000439 | -0.039196 | 100 |
| CA3/primary/N2 | 0.971520 | 0.000363 | -0.028167 | 100 |
| CA3/cx/D2 | 0.975192 | 0.000921 | -0.023278 | 100 |
| CA3/cx/N2 | 0.978253 | 0.000436 | -0.021115 | 100 |
| CA3/ecr/D2 | 0.973408 | 0.000944 | -0.025065 | 100 |
| CA3/ecr/N2 | 0.976780 | 0.000448 | -0.022598 | 100 |

## Marginal quality estimates

| Dimension | Value | Metric | Ratio | Paired SE | Cases | Seeds |
| --- | --- | --- | ---: | ---: | ---: | ---: |
| family | G1 | D2 | 0.910936 | 0.001394 | 10 | 100 |
| family | G1 | N2 | 0.930538 | 0.000994 | 10 | 100 |
| family | G2 | D2 | 1.000000 | 0.000000 | 2 | 100 |
| family | G2 | N2 | 1.000000 | 0.000000 | 2 | 100 |
| family | G3 | D2 | 0.888986 | 0.001489 | 8 | 100 |
| family | G3 | N2 | 0.943367 | 0.000648 | 8 | 100 |
| family | G4 | D2 | 1.000000 | 0.000000 | 10 | 100 |
| family | G4 | N2 | 1.000000 | 0.000000 | 10 | 100 |
| family | G5 | D2 | 0.992236 | 0.000272 | 18 | 100 |
| family | G5 | N2 | 0.993339 | 0.000211 | 18 | 100 |
| family | G6 | D2 | 0.911712 | 0.002379 | 6 | 100 |
| family | G6 | N2 | 0.919846 | 0.001887 | 6 | 100 |
| family | G7 | D2 | 1.000000 | 0.000000 | 1 | 100 |
| family | G7 | N2 | 1.000000 | 0.000000 | 1 | 100 |
| family | G8 | D2 | 0.990637 | 0.001586 | 6 | 100 |
| family | G8 | N2 | 0.989435 | 0.001553 | 6 | 100 |
| native_basis | cx | D2 | 0.944521 | 0.000724 | 48 | 100 |
| native_basis | cx | N2 | 0.960369 | 0.000625 | 48 | 100 |
| native_basis | cz | D2 | 0.982884 | 0.000258 | 13 | 100 |
| native_basis | cz | N2 | 0.986683 | 0.000144 | 13 | 100 |
| optimization_level | 2 | D2 | 0.965467 | 0.000445 | 31 | 100 |
| optimization_level | 2 | N2 | 0.974805 | 0.000348 | 31 | 100 |
| optimization_level | 3 | D2 | 0.954648 | 0.000660 | 30 | 100 |
| optimization_level | 3 | N2 | 0.967314 | 0.000485 | 30 | 100 |
| size_band | large | D2 | 0.986025 | 0.000232 | 9 | 100 |
| size_band | large | N2 | 0.988313 | 0.000155 | 9 | 100 |
| size_band | medium | D2 | 0.952796 | 0.000659 | 26 | 100 |
| size_band | medium | N2 | 0.972486 | 0.000284 | 26 | 100 |
| size_band | small | D2 | 0.938950 | 0.001173 | 26 | 100 |
| size_band | small | N2 | 0.950800 | 0.001079 | 26 | 100 |
| topology | grid | D2 | 0.972357 | 0.001083 | 14 | 100 |
| topology | grid | N2 | 0.974086 | 0.001137 | 14 | 100 |
| topology | heavy_hex | D2 | 0.957868 | 0.000478 | 47 | 100 |
| topology | heavy_hex | N2 | 0.970888 | 0.000327 | 47 | 100 |

Score without the iterations profile's scored groups (report-only):
- D2 ratio 0.954945 (paired SE 0.000533; cases: 55; seeds: 100).
- N2 ratio 0.967791 (paired SE 0.000448; cases: 55; seeds: 100).

Instance bootstrap (report-only): Fewer than three groups per family
Input groups by family: G1: 5, G2: 1, G3: 4, G4: 5, G5: 9, G6: 3, G7: 1, G8: 3.


## Per-case changes

| Case / metric | Ratio | Worst seed |
| --- | ---: | ---: |
| confirm/qft_n100/heavy_hex_d9_cz/L2/D2 | 0.939996 | 88 |
| confirm/qft_n100/heavy_hex_d9_cz/L2/N2 | 0.940982 | 64 |
| confirm/qft_n100/heavy_hex_d9_cz/L3/D2 | 0.930334 | 64 |
| confirm/qft_n100/heavy_hex_d9_cz/L3/N2 | 0.939499 | 53 |
| confirm/qft_cp_n14/melbourne_14_u/L2/D2 | 0.849700 | 12 |
| confirm/qft_cp_n14/melbourne_14_u/L2/N2 | 0.886946 | 49 |
| confirm/qft_cp_n14/melbourne_14_u/L3/D2 | 0.844614 | 80 |
| confirm/qft_cp_n14/melbourne_14_u/L3/N2 | 0.885994 | 95 |
| confirm/qft_full_n32/rochester_53/L2/D2 | 0.900492 | 34 |
| confirm/qft_full_n32/rochester_53/L2/N2 | 0.947995 | 34 |
| confirm/qft_full_n32/rochester_53/L3/D2 | 0.896628 | 37 |
| confirm/qft_full_n32/rochester_53/L3/N2 | 0.950575 | 59 |
| confirm/qft_cp_n8/melbourne_14_u/L2/D2 | 0.944750 | 11 |
| confirm/qft_cp_n8/melbourne_14_u/L2/N2 | 0.923559 | 1 |
| confirm/qft_cp_n8/melbourne_14_u/L3/D2 | 0.953593 | 48 |
| confirm/qft_cp_n8/melbourne_14_u/L3/N2 | 0.935829 | 12 |
| confirm/qft_full_n64/heavy_hex_d9_cz/L2/D2 | 0.910239 | 23 |
| confirm/qft_full_n64/heavy_hex_d9_cz/L2/N2 | 0.939026 | 90 |
| confirm/qft_full_n64/heavy_hex_d9_cz/L3/D2 | 0.898405 | 62 |
| confirm/qft_full_n64/heavy_hex_d9_cz/L3/N2 | 0.938421 | 4 |
| confirm/square_heisenberg_n100/heavy_hex_d9_cz/L2/D2 | 1.000000 | 0 |
| confirm/square_heisenberg_n100/heavy_hex_d9_cz/L2/N2 | 1.000000 | 0 |
| confirm/square_heisenberg_n100/heavy_hex_d9_cz/L3/D2 | 1.000000 | 0 |
| confirm/square_heisenberg_n100/heavy_hex_d9_cz/L3/N2 | 1.000000 | 0 |
| confirm/qaoa_ba_n100_3reps/heavy_hex_d9_cz/L2/D2 | 0.981202 | 42 |
| confirm/qaoa_ba_n100_3reps/heavy_hex_d9_cz/L2/N2 | 0.990397 | 65 |
| confirm/qaoa_ba_n100_3reps/heavy_hex_d9_cz/L3/D2 | 0.981578 | 6 |
| confirm/qaoa_ba_n100_3reps/heavy_hex_d9_cz/L3/N2 | 0.990151 | 6 |
| confirm/qaoa_complete_n8/mumbai_27/L2/D2 | 0.835064 | 37 |
| confirm/qaoa_complete_n8/mumbai_27/L2/N2 | 0.865890 | 37 |
| confirm/qaoa_complete_n8/mumbai_27/L3/D2 | 0.833902 | 37 |
| confirm/qaoa_complete_n8/mumbai_27/L3/N2 | 0.865443 | 37 |
| confirm/qaoa_complete_n16/mumbai_27/L2/D2 | 0.828449 | 32 |
| confirm/qaoa_complete_n16/mumbai_27/L2/N2 | 0.905768 | 66 |
| confirm/qaoa_complete_n16/mumbai_27/L3/D2 | 0.831941 | 81 |
| confirm/qaoa_complete_n16/mumbai_27/L3/N2 | 0.905719 | 96 |
| confirm/qaoa_complete_n32/rochester_53/L2/D2 | 0.860661 | 1 |
| confirm/qaoa_complete_n32/rochester_53/L2/N2 | 0.957824 | 76 |
| confirm/qaoa_complete_n32/rochester_53/L3/D2 | 0.859524 | 7 |
| confirm/qaoa_complete_n32/rochester_53/L3/N2 | 0.957048 | 51 |
| confirm/qv_n50_d50/heavy_hex_d9_cz/L2/D2 | 1.000000 | 0 |
| confirm/qv_n50_d50/heavy_hex_d9_cz/L2/N2 | 1.000000 | 0 |
| confirm/qv_n50_d50/heavy_hex_d9_cz/L3/D2 | 1.000000 | 0 |
| confirm/qv_n50_d50/heavy_hex_d9_cz/L3/N2 | 1.000000 | 0 |
| confirm/qv_n14_d14/melbourne_14/L2/D2 | 1.000000 | 0 |
| confirm/qv_n14_d14/melbourne_14/L2/N2 | 1.000000 | 0 |
| confirm/qv_n14_d14/melbourne_14/L3/D2 | 1.000000 | 0 |
| confirm/qv_n14_d14/melbourne_14/L3/N2 | 1.000000 | 0 |
| confirm/qv_n27_d27/mumbai_27_loose/L2/D2 | 1.000000 | 0 |
| confirm/qv_n27_d27/mumbai_27_loose/L2/N2 | 1.000000 | 0 |
| confirm/qv_n27_d27/mumbai_27_loose/L3/D2 | 1.000000 | 0 |
| confirm/qv_n27_d27/mumbai_27_loose/L3/N2 | 1.000000 | 0 |
| confirm/qv_n50_d20/rochester_53_u/L2/D2 | 1.000000 | 0 |
| confirm/qv_n50_d20/rochester_53_u/L2/N2 | 1.000000 | 0 |
| confirm/qv_n50_d20/rochester_53_u/L3/D2 | 1.000000 | 0 |
| confirm/qv_n50_d20/rochester_53_u/L3/N2 | 1.000000 | 0 |
| confirm/qv_n14_d14_s10/mumbai_27_loose/L2/D2 | 1.000000 | 0 |
| confirm/qv_n14_d14_s10/mumbai_27_loose/L2/N2 | 1.000000 | 0 |
| confirm/qv_n14_d14_s10/mumbai_27_loose/L3/D2 | 1.000000 | 0 |
| confirm/qv_n14_d14_s10/mumbai_27_loose/L3/N2 | 1.000000 | 0 |
| confirm/ripple_adder_10/grid_5x5_u/L2/D2 | 0.999798 | 0 |
| confirm/ripple_adder_10/grid_5x5_u/L2/N2 | 0.999883 | 0 |
| confirm/ripple_adder_10/grid_5x5_u/L3/D2 | 1.000000 | 0 |
| confirm/ripple_adder_10/grid_5x5_u/L3/N2 | 1.000000 | 0 |
| confirm/mcx_kg24_n6/mumbai_27/L2/D2 | 1.000000 | 0 |
| confirm/mcx_kg24_n6/mumbai_27/L2/N2 | 1.000000 | 0 |
| confirm/mcx_kg24_n6/mumbai_27/L3/D2 | 1.000000 | 0 |
| confirm/mcx_kg24_n6/mumbai_27/L3/N2 | 1.000000 | 0 |
| confirm/multiplier_h18_n32/rochester_53/L2/D2 | 0.997876 | 9 |
| confirm/multiplier_h18_n32/rochester_53/L2/N2 | 0.997877 | 85 |
| confirm/multiplier_h18_n32/rochester_53/L3/D2 | 0.997929 | 14 |
| confirm/multiplier_h18_n32/rochester_53/L3/N2 | 0.997931 | 79 |
| confirm/mcx_kg24_n16/mumbai_27/L2/D2 | 1.000000 | 0 |
| confirm/mcx_kg24_n16/mumbai_27/L2/N2 | 1.000000 | 0 |
| confirm/mcx_kg24_n16/mumbai_27/L3/D2 | 1.000000 | 0 |
| confirm/mcx_kg24_n16/mumbai_27/L3/N2 | 1.000000 | 0 |
| confirm/ripple_adder_20/grid_7x7_u/L2/D2 | 0.999890 | 0 |
| confirm/ripple_adder_20/grid_7x7_u/L2/N2 | 0.999925 | 0 |
| confirm/ripple_adder_20/grid_7x7_u/L3/D2 | 1.000000 | 0 |
| confirm/ripple_adder_20/grid_7x7_u/L3/N2 | 1.000000 | 0 |
| confirm/adder_modular_v17_n8/mumbai_27/L2/D2 | 0.980828 | 1 |
| confirm/adder_modular_v17_n8/mumbai_27/L2/N2 | 0.983124 | 1 |
| confirm/adder_modular_v17_n8/mumbai_27/L3/D2 | 0.980061 | 1 |
| confirm/adder_modular_v17_n8/mumbai_27/L3/N2 | 0.983120 | 1 |
| confirm/adder_modular_v17_n16/mumbai_27/L2/D2 | 0.977747 | 10 |
| confirm/adder_modular_v17_n16/mumbai_27/L2/N2 | 0.980818 | 10 |
| confirm/adder_modular_v17_n16/mumbai_27/L3/D2 | 0.979323 | 0 |
| confirm/adder_modular_v17_n16/mumbai_27/L3/N2 | 0.982136 | 0 |
| confirm/adder_modular_v17_n32/rochester_53/L2/D2 | 0.976598 | 27 |
| confirm/adder_modular_v17_n32/rochester_53/L2/N2 | 0.980391 | 27 |
| confirm/adder_modular_v17_n32/rochester_53/L3/D2 | 0.975757 | 86 |
| confirm/adder_modular_v17_n32/rochester_53/L3/N2 | 0.979709 | 45 |
| confirm/multiplier_h18_n16/mumbai_27/L2/D2 | 0.996329 | 26 |
| confirm/multiplier_h18_n16/mumbai_27/L2/N2 | 0.996761 | 76 |
| confirm/multiplier_h18_n16/mumbai_27/L3/D2 | 0.996620 | 57 |
| confirm/multiplier_h18_n16/mumbai_27/L3/N2 | 0.996891 | 80 |
| confirm/adder_modular_v17_n6/mumbai_27/L2/D2 | 0.990039 | 1 |
| confirm/adder_modular_v17_n6/mumbai_27/L2/N2 | 0.992791 | 1 |
| confirm/adder_modular_v17_n6/mumbai_27/L3/D2 | 0.990282 | 1 |
| confirm/adder_modular_v17_n6/mumbai_27/L3/N2 | 0.992791 | 1 |
| confirm/multiplier_h18_n20/heavy_hex_d9_cz/L2/D2 | 0.997587 | 19 |
| confirm/multiplier_h18_n20/heavy_hex_d9_cz/L2/N2 | 0.998338 | 4 |
| confirm/bv_all_ones_n100/heavy_hex_d9_cz/L2/D2 | 0.964490 | 32 |
| confirm/bv_all_ones_n100/heavy_hex_d9_cz/L2/N2 | 0.970932 | 32 |
| confirm/bv_all_ones_n100/heavy_hex_d9_cz/L3/D2 | 0.955515 | 51 |
| confirm/bv_all_ones_n100/heavy_hex_d9_cz/L3/N2 | 0.961448 | 51 |
| confirm/bv_all_ones_n16/mumbai_27/L2/D2 | 0.857139 | 13 |
| confirm/bv_all_ones_n16/mumbai_27/L2/N2 | 0.874425 | 9 |
| confirm/bv_all_ones_n16/mumbai_27/L3/D2 | 0.864469 | 13 |
| confirm/bv_all_ones_n16/mumbai_27/L3/N2 | 0.881900 | 30 |
| confirm/bv_all_ones_n50/rochester_53/L2/D2 | 0.918904 | 60 |
| confirm/bv_all_ones_n50/rochester_53/L2/N2 | 0.919368 | 12 |
| confirm/bv_all_ones_n50/rochester_53/L3/D2 | 0.915250 | 8 |
| confirm/bv_all_ones_n50/rochester_53/L3/N2 | 0.915259 | 46 |
| confirm/su2_circular_n89/heavy_hex_d9_cz/L2/D2 | 1.000000 | 0 |
| confirm/su2_circular_n89/heavy_hex_d9_cz/L2/N2 | 1.000000 | 0 |
| confirm/su2_circular_n89/heavy_hex_d9_cz/L3/D2 | 1.000000 | 0 |
| confirm/su2_circular_n89/heavy_hex_d9_cz/L3/N2 | 1.000000 | 0 |
| confirm/queko_bss_53+sabre/rochester_53/L2/D2 | 0.995232 | 93 |
| confirm/queko_bss_53+sabre/rochester_53/L2/N2 | 0.996099 | 10 |
| confirm/queko_bss_53+sabre/rochester_53/L3/D2 | 0.993724 | 52 |
| confirm/queko_bss_53+sabre/rochester_53/L3/N2 | 0.993533 | 1 |
| confirm/queko_bigd_20+sabre/tokyo_20/L2/D2 | 0.989984 | 0 |
| confirm/queko_bigd_20+sabre/tokyo_20/L2/N2 | 0.989398 | 0 |
| confirm/queko_bigd_20+sabre/tokyo_20/L3/D2 | 0.988126 | 0 |
| confirm/queko_bigd_20+sabre/tokyo_20/L3/N2 | 0.986167 | 0 |
| confirm/queko_bntf_54+sabre/sycamore_54/L2/D2 | 0.990157 | 97 |
| confirm/queko_bntf_54+sabre/sycamore_54/L2/N2 | 0.987847 | 13 |
| confirm/queko_bntf_54+sabre/sycamore_54/L3/D2 | 0.989782 | 1 |
| confirm/queko_bntf_54+sabre/sycamore_54/L3/N2 | 0.986919 | 8 |
| confirm/qft_n100/heavy_hex_d9_cx/L2/D2 | 0.942310 | 88 |
| confirm/qft_n100/heavy_hex_d9_cx/L2/N2 | 0.943364 | 64 |
| confirm/qft_n100/heavy_hex_d9_ecr/L2/D2 | 0.939996 | 88 |
| confirm/qft_n100/heavy_hex_d9_ecr/L2/N2 | 0.940982 | 64 |
| confirm/square_heisenberg_n100/heavy_hex_d9_cx/L2/D2 | 1.000000 | 0 |
| confirm/square_heisenberg_n100/heavy_hex_d9_cx/L2/N2 | 1.000000 | 0 |
| confirm/square_heisenberg_n100/heavy_hex_d9_ecr/L2/D2 | 1.000000 | 0 |
| confirm/square_heisenberg_n100/heavy_hex_d9_ecr/L2/N2 | 1.000000 | 0 |
| confirm/qaoa_ba_n100_3reps/heavy_hex_d9_cx/L2/D2 | 0.984184 | 27 |
| confirm/qaoa_ba_n100_3reps/heavy_hex_d9_cx/L2/N2 | 0.992371 | 69 |
| confirm/qaoa_ba_n100_3reps/heavy_hex_d9_ecr/L2/D2 | 0.981202 | 42 |
| confirm/qaoa_ba_n100_3reps/heavy_hex_d9_ecr/L2/N2 | 0.990397 | 65 |

## Zero-baseline changes

| Case | Metric | Worst delta | Seed | Baseline | Evolved |
| --- | --- | ---: | ---: | ---: | ---: |
| confirm/qft16_cancel/mumbai_27/L2 | D2 | 0 | 0 | 0 | 0 |
| confirm/qft16_cancel/mumbai_27/L2 | N2 | 0 | 0 | 0 | 0 |
| confirm/qft16_cancel/mumbai_27/L3 | D2 | 0 | 0 | 0 | 0 |
| confirm/qft16_cancel/mumbai_27/L3 | N2 | 0 | 0 | 0 | 0 |
| confirm/bvlike_n100/heavy_hex_d9_cz/L2 | D2 | 0 | 0 | 0 | 0 |
| confirm/bvlike_n100/heavy_hex_d9_cz/L2 | N2 | 0 | 0 | 0 | 0 |
| confirm/bvlike_n100/heavy_hex_d9_cz/L3 | D2 | 0 | 0 | 0 | 0 |
| confirm/bvlike_n100/heavy_hex_d9_cz/L3 | N2 | 0 | 0 | 0 | 0 |
