# benchpress report — confirm-profile

Stage evidence snapshot; run decide for the final benchmark verdict.

## Benchpress

Stage: **complete**.

### Check results

| Result | Count |
| --- | --- |
| passed | 1 |

### Checks needing attention

None.

50 circuit/target entries; optimization levels 2 and 3; seeds [0, 1, 2]. Complete cases: 100/100.

### Benchpress improvement

Changes are evolved minus baseline; ratios are evolved / baseline. Lower is better. Improvement is 100 × (1 − ratio): positive means better, negative means worse. Quality and runtime differences are descriptive; no separate Benchpress regression threshold is imposed.

Each case uses the median of its paired seed ratios; geometric means give each complete case with a defined ratio equal weight. Zero-baseline ratios are unavailable and excluded from geometric means. A zero median change can coexist with a nonzero geometric improvement when most cases are unchanged. The quality stage uses a different panel, seed blocks and frozen weights, so its overall score is not directly comparable.

Overall rows pool the complete cases across levels 2 and 3 with equal case weights.

| Level | Metric | Complete cases | Median change | Geomean ratio | Geomean improvement | Better | Equal | Worse |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| 2 | N2 | 50 | 0.0 | 0.982862306765265 | +1.71% | 18 | 32 | 0 |
| 2 | D2 | 50 | 0.0 | 0.9721537469477612 | +2.78% | 18 | 32 | 0 |
| 3 | N2 | 50 | 0.0 | 0.9827244654128316 | +1.73% | 19 | 31 | 0 |
| 3 | D2 | 50 | 0.0 | 0.9752739511522205 | +2.47% | 19 | 31 | 0 |
| Overall | D2 | 100 | 0.0 | 0.9737125992371564 | +2.63% | 37 | 63 | 0 |
| Overall | N2 | 100 | 0.0 | 0.9827933836724367 | +1.72% | 37 | 63 | 0 |

### Quality tests

One row per Benchpress test and optimization level. D2 (two-qubit depth) and N2 (two-qubit gate count) are arithmetic means over the test's paired seeds. Improvement is 100 × (baseline mean − evolved mean) / baseline mean. These descriptive means can differ from the paired-median geometric estimates above.

Missing or invalid seed pairs make that metric unavailable. Percentages with a zero baseline are N/A (undefined). Seeds is the expected count per revision.

| Test | Target | Level | Seeds | Baseline D2 | Evolved D2 | D2 improvement | Baseline N2 | Evolved N2 | N2 improvement |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| test_hamiltonians[ham_bh_graph-1D-grid-pbc-qubitnodes_Lx-14_U-10_enc-stdbinary_d-4-all-to-all] | all-to-all | 2 | 3 | 978.00 | 978.00 | +0.00% | 1066.00 | 1066.00 | +0.00% |
| test_hamiltonians[ham_bh_graph-1D-grid-pbc-qubitnodes_Lx-14_U-10_enc-stdbinary_d-4-all-to-all] | all-to-all | 3 | 3 | 981.00 | 981.00 | +0.00% | 1068.00 | 1068.00 | +0.00% |
| test_hamiltonians[ham_bh_graph-1D-grid-pbc-qubitnodes_Lx-14_U-10_enc-stdbinary_d-4-heavy-hex] | heavy-hex | 2 | 3 | 946.33 | 946.33 | +0.00% | 1011.67 | 1011.67 | +0.00% |
| test_hamiltonians[ham_bh_graph-1D-grid-pbc-qubitnodes_Lx-14_U-10_enc-stdbinary_d-4-heavy-hex] | heavy-hex | 3 | 3 | 940.00 | 940.00 | +0.00% | 999.00 | 999.00 | +0.00% |
| test_hamiltonians[ham_bh_graph-1D-grid-pbc-qubitnodes_Lx-14_U-10_enc-stdbinary_d-4-linear] | linear | 2 | 3 | 1054.00 | 1054.00 | +0.00% | 1169.00 | 1169.00 | +0.00% |
| test_hamiltonians[ham_bh_graph-1D-grid-pbc-qubitnodes_Lx-14_U-10_enc-stdbinary_d-4-linear] | linear | 3 | 3 | 1082.00 | 1082.00 | +0.00% | 1199.00 | 1199.00 | +0.00% |
| test_hamiltonians[ham_bh_graph-1D-grid-pbc-qubitnodes_Lx-14_U-10_enc-stdbinary_d-4-square] | square | 2 | 3 | 946.00 | 945.00 | +0.11% | 1002.67 | 1002.00 | +0.07% |
| test_hamiltonians[ham_bh_graph-1D-grid-pbc-qubitnodes_Lx-14_U-10_enc-stdbinary_d-4-square] | square | 3 | 3 | 926.00 | 926.00 | +0.00% | 985.00 | 985.00 | +0.00% |
| test_hamiltonians[ham_ham_JW14-all-to-all] | all-to-all | 2 | 3 | 2334.00 | 2334.00 | +0.00% | 3332.00 | 3332.00 | +0.00% |
| test_hamiltonians[ham_ham_JW14-all-to-all] | all-to-all | 3 | 3 | 2330.00 | 2330.00 | +0.00% | 3328.00 | 3328.00 | +0.00% |
| test_hamiltonians[ham_ham_JW14-heavy-hex] | heavy-hex | 2 | 3 | 6435.00 | 6399.33 | +0.55% | 7443.33 | 7419.33 | +0.32% |
| test_hamiltonians[ham_ham_JW14-heavy-hex] | heavy-hex | 3 | 3 | 5060.00 | 5017.00 | +0.85% | 5991.00 | 5964.33 | +0.45% |
| test_hamiltonians[ham_ham_JW14-linear] | linear | 2 | 3 | 5949.00 | 5937.67 | +0.19% | 6865.67 | 6859.00 | +0.10% |
| test_hamiltonians[ham_ham_JW14-linear] | linear | 3 | 3 | 5099.00 | 5087.67 | +0.22% | 5942.67 | 5936.00 | +0.11% |
| test_hamiltonians[ham_ham_JW14-square] | square | 2 | 3 | 5554.33 | 5524.33 | +0.54% | 6380.33 | 6353.67 | +0.42% |
| test_hamiltonians[ham_ham_JW14-square] | square | 3 | 3 | 4830.33 | 4803.67 | +0.55% | 5619.33 | 5592.67 | +0.47% |
| test_QASMBench_large[qft_n29-all-to-all] | all-to-all | 2 | 3 | 110.00 | 110.00 | +0.00% | 602.00 | 602.00 | +0.00% |
| test_QASMBench_large[qft_n29-all-to-all] | all-to-all | 3 | 3 | 110.00 | 110.00 | +0.00% | 602.00 | 602.00 | +0.00% |
| test_QASMBench_large[qft_n29-heavy-hex] | heavy-hex | 2 | 3 | 332.33 | 294.00 | +11.53% | 1353.00 | 1273.00 | +5.91% |
| test_QASMBench_large[qft_n29-heavy-hex] | heavy-hex | 3 | 3 | 303.33 | 267.00 | +11.98% | 1285.33 | 1207.33 | +6.07% |
| test_QASMBench_large[qft_n29-linear] | linear | 2 | 3 | 276.67 | 228.00 | +17.59% | 1373.67 | 1302.33 | +5.19% |
| test_QASMBench_large[qft_n29-linear] | linear | 3 | 3 | 263.33 | 242.00 | +8.10% | 1363.67 | 1313.00 | +3.72% |
| test_QASMBench_large[qft_n29-square] | square | 2 | 3 | 391.67 | 348.00 | +11.15% | 1249.00 | 1127.00 | +9.77% |
| test_QASMBench_large[qft_n29-square] | square | 3 | 3 | 396.67 | 357.00 | +10.00% | 1212.67 | 1102.00 | +9.13% |
| test_QASMBench_large[swap_test_n41-all-to-all] | all-to-all | 2 | 3 | 102.00 | 102.00 | +0.00% | 140.00 | 140.00 | +0.00% |
| test_QASMBench_large[swap_test_n41-all-to-all] | all-to-all | 3 | 3 | 102.00 | 102.00 | +0.00% | 140.00 | 140.00 | +0.00% |
| test_QASMBench_large[swap_test_n41-heavy-hex] | heavy-hex | 2 | 3 | 298.33 | 298.33 | +0.00% | 367.67 | 367.67 | +0.00% |
| test_QASMBench_large[swap_test_n41-heavy-hex] | heavy-hex | 3 | 3 | 302.67 | 299.67 | +0.99% | 371.00 | 369.00 | +0.54% |
| test_QASMBench_large[swap_test_n41-linear] | linear | 2 | 3 | 181.33 | 181.33 | +0.00% | 232.67 | 232.67 | +0.00% |
| test_QASMBench_large[swap_test_n41-linear] | linear | 3 | 3 | 181.33 | 181.33 | +0.00% | 232.67 | 232.67 | +0.00% |
| test_QASMBench_large[swap_test_n41-square] | square | 2 | 3 | 207.33 | 206.33 | +0.48% | 286.33 | 285.67 | +0.23% |
| test_QASMBench_large[swap_test_n41-square] | square | 3 | 3 | 220.67 | 217.67 | +1.36% | 299.00 | 298.33 | +0.22% |
| test_QASMBench_medium[ising_n26-all-to-all] | all-to-all | 2 | 3 | 4.00 | 4.00 | +0.00% | 50.00 | 50.00 | +0.00% |
| test_QASMBench_medium[ising_n26-all-to-all] | all-to-all | 3 | 3 | 4.00 | 4.00 | +0.00% | 50.00 | 50.00 | +0.00% |
| test_QASMBench_medium[ising_n26-heavy-hex] | heavy-hex | 2 | 3 | 4.00 | 4.00 | +0.00% | 50.00 | 50.00 | +0.00% |
| test_QASMBench_medium[ising_n26-heavy-hex] | heavy-hex | 3 | 3 | 4.00 | 4.00 | +0.00% | 50.00 | 50.00 | +0.00% |
| test_QASMBench_medium[ising_n26-linear] | linear | 2 | 3 | 4.00 | 4.00 | +0.00% | 50.00 | 50.00 | +0.00% |
| test_QASMBench_medium[ising_n26-linear] | linear | 3 | 3 | 4.00 | 4.00 | +0.00% | 50.00 | 50.00 | +0.00% |
| test_QASMBench_medium[ising_n26-square] | square | 2 | 3 | 4.00 | 4.00 | +0.00% | 50.00 | 50.00 | +0.00% |
| test_QASMBench_medium[ising_n26-square] | square | 3 | 3 | 4.00 | 4.00 | +0.00% | 50.00 | 50.00 | +0.00% |
| test_QASMBench_medium[qft_n18-all-to-all] | all-to-all | 2 | 3 | 66.00 | 66.00 | +0.00% | 294.00 | 294.00 | +0.00% |
| test_QASMBench_medium[qft_n18-all-to-all] | all-to-all | 3 | 3 | 66.00 | 66.00 | +0.00% | 294.00 | 294.00 | +0.00% |
| test_QASMBench_medium[qft_n18-heavy-hex] | heavy-hex | 2 | 3 | 193.67 | 161.33 | +16.70% | 543.67 | 492.33 | +9.44% |
| test_QASMBench_medium[qft_n18-heavy-hex] | heavy-hex | 3 | 3 | 194.67 | 156.33 | +19.69% | 515.33 | 466.67 | +9.44% |
| test_QASMBench_medium[qft_n18-linear] | linear | 2 | 3 | 150.33 | 112.33 | +25.28% | 510.00 | 460.00 | +9.80% |
| test_QASMBench_medium[qft_n18-linear] | linear | 3 | 3 | 159.67 | 119.00 | +25.47% | 521.67 | 462.33 | +11.37% |
| test_QASMBench_medium[qft_n18-square] | square | 2 | 3 | 206.67 | 187.67 | +9.19% | 511.67 | 461.67 | +9.77% |
| test_QASMBench_medium[qft_n18-square] | square | 3 | 3 | 225.67 | 206.67 | +8.42% | 508.00 | 459.33 | +9.58% |
| test_QASMBench_small[adder_n10-all-to-all] | all-to-all | 2 | 3 | 55.00 | 55.00 | +0.00% | 65.00 | 65.00 | +0.00% |
| test_QASMBench_small[adder_n10-all-to-all] | all-to-all | 3 | 3 | 55.00 | 55.00 | +0.00% | 65.00 | 65.00 | +0.00% |
| test_QASMBench_small[adder_n10-heavy-hex] | heavy-hex | 2 | 3 | 89.67 | 89.67 | +0.00% | 99.00 | 99.00 | +0.00% |
| test_QASMBench_small[adder_n10-heavy-hex] | heavy-hex | 3 | 3 | 89.67 | 89.67 | +0.00% | 99.00 | 99.00 | +0.00% |
| test_QASMBench_small[adder_n10-linear] | linear | 2 | 3 | 84.00 | 84.00 | +0.00% | 94.00 | 94.00 | +0.00% |
| test_QASMBench_small[adder_n10-linear] | linear | 3 | 3 | 84.00 | 84.00 | +0.00% | 94.00 | 94.00 | +0.00% |
| test_QASMBench_small[adder_n10-square] | square | 2 | 3 | 79.33 | 78.33 | +1.26% | 94.00 | 93.00 | +1.06% |
| test_QASMBench_small[adder_n10-square] | square | 3 | 3 | 76.33 | 76.33 | +0.00% | 90.00 | 90.00 | +0.00% |
| test_QASMBench_small[qaoa_n6-all-to-all] | all-to-all | 2 | 3 | 22.00 | 22.00 | +0.00% | 36.00 | 36.00 | +0.00% |
| test_QASMBench_small[qaoa_n6-all-to-all] | all-to-all | 3 | 3 | 22.00 | 22.00 | +0.00% | 36.00 | 36.00 | +0.00% |
| test_QASMBench_small[qaoa_n6-heavy-hex] | heavy-hex | 2 | 3 | 48.00 | 48.00 | +0.00% | 63.00 | 63.00 | +0.00% |
| test_QASMBench_small[qaoa_n6-heavy-hex] | heavy-hex | 3 | 3 | 48.67 | 48.67 | +0.00% | 61.33 | 61.33 | +0.00% |
| test_QASMBench_small[qaoa_n6-linear] | linear | 2 | 3 | 47.67 | 47.67 | +0.00% | 70.33 | 70.33 | +0.00% |
| test_QASMBench_small[qaoa_n6-linear] | linear | 3 | 3 | 51.67 | 51.67 | +0.00% | 72.00 | 72.00 | +0.00% |
| test_QASMBench_small[qaoa_n6-square] | square | 2 | 3 | 42.00 | 42.00 | +0.00% | 52.67 | 52.67 | +0.00% |
| test_QASMBench_small[qaoa_n6-square] | square | 3 | 3 | 45.00 | 45.00 | +0.00% | 54.00 | 54.00 | +0.00% |
| test_feynman_transpile[adder_8.qasm] | fake_torino | 2 | 3 | 297.33 | 291.33 | +2.02% | 751.00 | 740.33 | +1.42% |
| test_feynman_transpile[adder_8.qasm] | fake_torino | 3 | 3 | 280.33 | 277.33 | +1.07% | 746.33 | 737.67 | +1.16% |
| test_feynman_transpile[barenco_tof_5.qasm] | fake_torino | 2 | 3 | 92.67 | 92.67 | +0.00% | 117.67 | 117.67 | +0.00% |
| test_feynman_transpile[barenco_tof_5.qasm] | fake_torino | 3 | 3 | 92.67 | 92.67 | +0.00% | 117.67 | 117.67 | +0.00% |
| test_feynman_transpile[gf2^8_mult.qasm] | fake_torino | 2 | 3 | 524.00 | 521.67 | +0.45% | 1148.33 | 1143.00 | +0.46% |
| test_feynman_transpile[gf2^8_mult.qasm] | fake_torino | 3 | 3 | 530.33 | 525.33 | +0.94% | 1150.00 | 1143.33 | +0.58% |
| test_feynman_transpile[qft_4.qasm] | fake_torino | 2 | 3 | 76.33 | 76.33 | +0.00% | 79.00 | 79.00 | +0.00% |
| test_feynman_transpile[qft_4.qasm] | fake_torino | 3 | 3 | 76.33 | 76.33 | +0.00% | 79.00 | 79.00 | +0.00% |
| test_feynman_transpile[rc_adder_6.qasm] | fake_torino | 2 | 3 | 95.67 | 94.33 | +1.39% | 153.00 | 142.33 | +6.97% |
| test_feynman_transpile[rc_adder_6.qasm] | fake_torino | 3 | 3 | 91.67 | 90.33 | +1.45% | 150.67 | 141.33 | +6.19% |
| test_hamlib_hamiltonians_transpile[ham_bh_graph-1D-grid-pbc-qubitnodes_Lx-14_U-10_enc-stdbinary_d-4] | fake_torino | 2 | 3 | 966.67 | 966.67 | +0.00% | 1044.67 | 1044.67 | +0.00% |
| test_hamlib_hamiltonians_transpile[ham_bh_graph-1D-grid-pbc-qubitnodes_Lx-14_U-10_enc-stdbinary_d-4] | fake_torino | 3 | 3 | 974.00 | 974.00 | +0.00% | 1038.00 | 1038.00 | +0.00% |
| test_hamlib_hamiltonians_transpile[ham_complbipart-n-10_a-5_b-5] | fake_torino | 2 | 3 | 226.00 | 207.00 | +8.41% | 278.33 | 261.67 | +5.99% |
| test_hamlib_hamiltonians_transpile[ham_complbipart-n-10_a-5_b-5] | fake_torino | 3 | 3 | 227.67 | 210.00 | +7.76% | 283.00 | 265.67 | +6.12% |
| test_hamlib_hamiltonians_transpile[ham_ham_JW14] | fake_torino | 2 | 3 | 5401.33 | 5378.00 | +0.43% | 6279.67 | 6263.67 | +0.25% |
| test_hamlib_hamiltonians_transpile[ham_ham_JW14] | fake_torino | 3 | 3 | 4976.33 | 4939.67 | +0.74% | 5839.67 | 5815.67 | +0.41% |
| test_hamlib_hamiltonians_transpile[ham_tsp_prob-ts225_Ncity-5_enc-unary] | fake_torino | 2 | 3 | 150.00 | 134.00 | +10.67% | 469.67 | 443.67 | +5.54% |
| test_hamlib_hamiltonians_transpile[ham_tsp_prob-ts225_Ncity-5_enc-unary] | fake_torino | 3 | 3 | 157.33 | 144.33 | +8.26% | 497.00 | 461.67 | +7.11% |
| test_BV_100_transpile | fake_torino | 2 | 3 | 197.33 | 197.33 | +0.00% | 197.33 | 197.33 | +0.00% |
| test_BV_100_transpile | fake_torino | 3 | 3 | 197.33 | 197.33 | +0.00% | 197.33 | 197.33 | +0.00% |
| test_BVlike_simplification_transpile | fake_torino | 2 | 3 | 0.00 | 0.00 | N/A | 0.00 | 0.00 | N/A |
| test_BVlike_simplification_transpile | fake_torino | 3 | 3 | 0.00 | 0.00 | N/A | 0.00 | 0.00 | N/A |
| test_QAOA_100_transpile | fake_torino | 2 | 3 | 1592.67 | 1566.67 | +1.63% | 8747.33 | 8675.33 | +0.82% |
| test_QAOA_100_transpile | fake_torino | 3 | 3 | 1490.67 | 1468.00 | +1.52% | 8549.33 | 8457.33 | +1.08% |
| test_QFT_100_transpile | fake_torino | 2 | 3 | 1827.67 | 1741.67 | +4.71% | 9705.33 | 9098.00 | +6.26% |
| test_QFT_100_transpile | fake_torino | 3 | 3 | 1709.67 | 1601.33 | +6.34% | 9248.67 | 8756.67 | +5.32% |
| test_QV_100_transpile | fake_torino | 2 | 3 | 10380.00 | 10380.00 | +0.00% | 95893.00 | 95893.00 | +0.00% |
| test_QV_100_transpile | fake_torino | 3 | 3 | 10423.00 | 10423.00 | +0.00% | 95845.00 | 95845.00 | +0.00% |
| test_circSU2_100_transpile | fake_torino | 2 | 3 | 300.00 | 300.00 | +0.00% | 300.00 | 300.00 | +0.00% |
| test_circSU2_100_transpile | fake_torino | 3 | 3 | 300.00 | 300.00 | +0.00% | 300.00 | 300.00 | +0.00% |
| test_circSU2_89_transpile | fake_torino | 2 | 3 | 318.00 | 318.00 | +0.00% | 327.00 | 327.00 | +0.00% |
| test_circSU2_89_transpile | fake_torino | 3 | 3 | 318.00 | 318.00 | +0.00% | 327.00 | 327.00 | +0.00% |
| test_clifford_100_transpile | fake_torino | 2 | 3 | 20454.00 | 20156.00 | +1.46% | 58190.33 | 57665.00 | +0.90% |
| test_clifford_100_transpile | fake_torino | 3 | 3 | 20262.67 | 19956.33 | +1.51% | 58201.33 | 57680.67 | +0.89% |
| test_square_heisenberg_100_transpile | fake_torino | 2 | 3 | 350.00 | 350.00 | +0.00% | 1533.00 | 1533.00 | +0.00% |
| test_square_heisenberg_100_transpile | fake_torino | 3 | 3 | 346.00 | 346.00 | +0.00% | 1551.00 | 1551.00 | +0.00% |

### Runtime

Runtime measures a single pm.run(circuit) call, excluding input loading, pass-manager construction and validation. No warmup, calibration or machine-load filtering.

Differences are evolved − baseline; negative differences mean faster. Improvement is 100 × (baseline − evolved) / baseline. Per-test times are arithmetic means over all expected paired seeds.

Full-panel measured runtime (300 seeds per revision): baseline **338.239854 s**, evolved **341.676018 s**; difference **+3.436165 s** (-1.02% improvement).

Equal-case geometric mean runtime ratio (ratios of seed means): 1.032846×.

Paired seeds: 300 / 300; missing samples: 0; failed samples: 0.

| Test | Target | Level | Seeds | Baseline (s) | Evolved (s) | Difference (s) | Runtime improvement |
| --- | --- | --- | --- | --- | --- | --- | --- |
| test_hamiltonians[ham_bh_graph-1D-grid-pbc-qubitnodes_Lx-14_U-10_enc-stdbinary_d-4-all-to-all] | all-to-all | 2 | 3 | 0.045651 | 0.046675 | +0.001024 | -2.24% |
| test_hamiltonians[ham_bh_graph-1D-grid-pbc-qubitnodes_Lx-14_U-10_enc-stdbinary_d-4-all-to-all] | all-to-all | 3 | 3 | 0.353003 | 0.351421 | -0.001582 | +0.45% |
| test_hamiltonians[ham_bh_graph-1D-grid-pbc-qubitnodes_Lx-14_U-10_enc-stdbinary_d-4-heavy-hex] | heavy-hex | 2 | 3 | 0.057424 | 0.060604 | +0.003180 | -5.54% |
| test_hamiltonians[ham_bh_graph-1D-grid-pbc-qubitnodes_Lx-14_U-10_enc-stdbinary_d-4-heavy-hex] | heavy-hex | 3 | 3 | 0.084256 | 0.090684 | +0.006428 | -7.63% |
| test_hamiltonians[ham_bh_graph-1D-grid-pbc-qubitnodes_Lx-14_U-10_enc-stdbinary_d-4-linear] | linear | 2 | 3 | 0.052661 | 0.056196 | +0.003535 | -6.71% |
| test_hamiltonians[ham_bh_graph-1D-grid-pbc-qubitnodes_Lx-14_U-10_enc-stdbinary_d-4-linear] | linear | 3 | 3 | 0.072759 | 0.071889 | -0.000870 | +1.20% |
| test_hamiltonians[ham_bh_graph-1D-grid-pbc-qubitnodes_Lx-14_U-10_enc-stdbinary_d-4-square] | square | 2 | 3 | 0.062630 | 0.064166 | +0.001536 | -2.45% |
| test_hamiltonians[ham_bh_graph-1D-grid-pbc-qubitnodes_Lx-14_U-10_enc-stdbinary_d-4-square] | square | 3 | 3 | 0.320203 | 0.318198 | -0.002005 | +0.63% |
| test_hamiltonians[ham_ham_JW14-all-to-all] | all-to-all | 2 | 3 | 0.122816 | 0.133217 | +0.010401 | -8.47% |
| test_hamiltonians[ham_ham_JW14-all-to-all] | all-to-all | 3 | 3 | 0.677126 | 0.639866 | -0.037260 | +5.50% |
| test_hamiltonians[ham_ham_JW14-heavy-hex] | heavy-hex | 2 | 3 | 0.432056 | 0.450973 | +0.018917 | -4.38% |
| test_hamiltonians[ham_ham_JW14-heavy-hex] | heavy-hex | 3 | 3 | 0.598767 | 0.639442 | +0.040676 | -6.79% |
| test_hamiltonians[ham_ham_JW14-linear] | linear | 2 | 3 | 0.356640 | 0.359915 | +0.003275 | -0.92% |
| test_hamiltonians[ham_ham_JW14-linear] | linear | 3 | 3 | 0.467389 | 0.477258 | +0.009869 | -2.11% |
| test_hamiltonians[ham_ham_JW14-square] | square | 2 | 3 | 0.414554 | 0.419219 | +0.004665 | -1.13% |
| test_hamiltonians[ham_ham_JW14-square] | square | 3 | 3 | 0.568585 | 0.578901 | +0.010315 | -1.81% |
| test_QASMBench_large[qft_n29-all-to-all] | all-to-all | 2 | 3 | 0.033140 | 0.034106 | +0.000966 | -2.91% |
| test_QASMBench_large[qft_n29-all-to-all] | all-to-all | 3 | 3 | 0.869422 | 0.877116 | +0.007694 | -0.88% |
| test_QASMBench_large[qft_n29-heavy-hex] | heavy-hex | 2 | 3 | 0.144893 | 0.158501 | +0.013608 | -9.39% |
| test_QASMBench_large[qft_n29-heavy-hex] | heavy-hex | 3 | 3 | 0.185615 | 0.194023 | +0.008408 | -4.53% |
| test_QASMBench_large[qft_n29-linear] | linear | 2 | 3 | 0.115238 | 0.123697 | +0.008459 | -7.34% |
| test_QASMBench_large[qft_n29-linear] | linear | 3 | 3 | 0.162544 | 0.162792 | +0.000247 | -0.15% |
| test_QASMBench_large[qft_n29-square] | square | 2 | 3 | 0.131170 | 0.156011 | +0.024841 | -18.94% |
| test_QASMBench_large[qft_n29-square] | square | 3 | 3 | 0.165394 | 0.190898 | +0.025504 | -15.42% |
| test_QASMBench_large[swap_test_n41-all-to-all] | all-to-all | 2 | 3 | 0.017020 | 0.017032 | +0.000012 | -0.07% |
| test_QASMBench_large[swap_test_n41-all-to-all] | all-to-all | 3 | 3 | 0.430553 | 0.428271 | -0.002281 | +0.53% |
| test_QASMBench_large[swap_test_n41-heavy-hex] | heavy-hex | 2 | 3 | 0.025694 | 0.026588 | +0.000894 | -3.48% |
| test_QASMBench_large[swap_test_n41-heavy-hex] | heavy-hex | 3 | 3 | 0.035744 | 0.037517 | +0.001773 | -4.96% |
| test_QASMBench_large[swap_test_n41-linear] | linear | 2 | 3 | 0.021496 | 0.023133 | +0.001637 | -7.61% |
| test_QASMBench_large[swap_test_n41-linear] | linear | 3 | 3 | 0.027877 | 0.029432 | +0.001555 | -5.58% |
| test_QASMBench_large[swap_test_n41-square] | square | 2 | 3 | 0.029281 | 0.029734 | +0.000452 | -1.54% |
| test_QASMBench_large[swap_test_n41-square] | square | 3 | 3 | 0.042313 | 0.042810 | +0.000497 | -1.17% |
| test_QASMBench_medium[ising_n26-all-to-all] | all-to-all | 2 | 3 | 0.008247 | 0.007878 | -0.000369 | +4.48% |
| test_QASMBench_medium[ising_n26-all-to-all] | all-to-all | 3 | 3 | 0.213112 | 0.212343 | -0.000769 | +0.36% |
| test_QASMBench_medium[ising_n26-heavy-hex] | heavy-hex | 2 | 3 | 0.007272 | 0.007605 | +0.000333 | -4.58% |
| test_QASMBench_medium[ising_n26-heavy-hex] | heavy-hex | 3 | 3 | 0.031963 | 0.033152 | +0.001189 | -3.72% |
| test_QASMBench_medium[ising_n26-linear] | linear | 2 | 3 | 0.003677 | 0.003857 | +0.000180 | -4.89% |
| test_QASMBench_medium[ising_n26-linear] | linear | 3 | 3 | 0.004465 | 0.005098 | +0.000633 | -14.18% |
| test_QASMBench_medium[ising_n26-square] | square | 2 | 3 | 0.007542 | 0.007241 | -0.000302 | +4.00% |
| test_QASMBench_medium[ising_n26-square] | square | 3 | 3 | 0.160061 | 0.170140 | +0.010079 | -6.30% |
| test_QASMBench_medium[qft_n18-all-to-all] | all-to-all | 2 | 3 | 0.015992 | 0.016170 | +0.000178 | -1.11% |
| test_QASMBench_medium[qft_n18-all-to-all] | all-to-all | 3 | 3 | 0.347944 | 0.348657 | +0.000713 | -0.20% |
| test_QASMBench_medium[qft_n18-heavy-hex] | heavy-hex | 2 | 3 | 0.047742 | 0.050351 | +0.002609 | -5.46% |
| test_QASMBench_medium[qft_n18-heavy-hex] | heavy-hex | 3 | 3 | 0.065603 | 0.067270 | +0.001667 | -2.54% |
| test_QASMBench_medium[qft_n18-linear] | linear | 2 | 3 | 0.037966 | 0.041364 | +0.003398 | -8.95% |
| test_QASMBench_medium[qft_n18-linear] | linear | 3 | 3 | 0.047877 | 0.051579 | +0.003702 | -7.73% |
| test_QASMBench_medium[qft_n18-square] | square | 2 | 3 | 0.043798 | 0.046444 | +0.002647 | -6.04% |
| test_QASMBench_medium[qft_n18-square] | square | 3 | 3 | 0.062410 | 0.061455 | -0.000955 | +1.53% |
| test_QASMBench_small[adder_n10-all-to-all] | all-to-all | 2 | 3 | 0.007085 | 0.006868 | -0.000217 | +3.06% |
| test_QASMBench_small[adder_n10-all-to-all] | all-to-all | 3 | 3 | 0.039380 | 0.039046 | -0.000334 | +0.85% |
| test_QASMBench_small[adder_n10-heavy-hex] | heavy-hex | 2 | 3 | 0.007170 | 0.007563 | +0.000393 | -5.49% |
| test_QASMBench_small[adder_n10-heavy-hex] | heavy-hex | 3 | 3 | 0.007871 | 0.008639 | +0.000768 | -9.76% |
| test_QASMBench_small[adder_n10-linear] | linear | 2 | 3 | 0.006738 | 0.007408 | +0.000671 | -9.95% |
| test_QASMBench_small[adder_n10-linear] | linear | 3 | 3 | 0.007318 | 0.008043 | +0.000725 | -9.91% |
| test_QASMBench_small[adder_n10-square] | square | 2 | 3 | 0.007212 | 0.008102 | +0.000890 | -12.34% |
| test_QASMBench_small[adder_n10-square] | square | 3 | 3 | 0.009208 | 0.009515 | +0.000307 | -3.33% |
| test_QASMBench_small[qaoa_n6-all-to-all] | all-to-all | 2 | 3 | 0.002899 | 0.003121 | +0.000222 | -7.65% |
| test_QASMBench_small[qaoa_n6-all-to-all] | all-to-all | 3 | 3 | 0.005171 | 0.005347 | +0.000175 | -3.39% |
| test_QASMBench_small[qaoa_n6-heavy-hex] | heavy-hex | 2 | 3 | 0.005524 | 0.005782 | +0.000258 | -4.67% |
| test_QASMBench_small[qaoa_n6-heavy-hex] | heavy-hex | 3 | 3 | 0.007020 | 0.006933 | -0.000087 | +1.24% |
| test_QASMBench_small[qaoa_n6-linear] | linear | 2 | 3 | 0.005103 | 0.005233 | +0.000130 | -2.55% |
| test_QASMBench_small[qaoa_n6-linear] | linear | 3 | 3 | 0.006539 | 0.007309 | +0.000770 | -11.77% |
| test_QASMBench_small[qaoa_n6-square] | square | 2 | 3 | 0.004820 | 0.005208 | +0.000388 | -8.05% |
| test_QASMBench_small[qaoa_n6-square] | square | 3 | 3 | 0.006213 | 0.006337 | +0.000124 | -2.00% |
| test_feynman_transpile[adder_8.qasm] | fake_torino | 2 | 3 | 0.059481 | 0.061607 | +0.002126 | -3.57% |
| test_feynman_transpile[adder_8.qasm] | fake_torino | 3 | 3 | 0.086118 | 0.090304 | +0.004186 | -4.86% |
| test_feynman_transpile[barenco_tof_5.qasm] | fake_torino | 2 | 3 | 0.010309 | 0.011504 | +0.001195 | -11.60% |
| test_feynman_transpile[barenco_tof_5.qasm] | fake_torino | 3 | 3 | 0.012829 | 0.014413 | +0.001584 | -12.35% |
| test_feynman_transpile[gf2^8_mult.qasm] | fake_torino | 2 | 3 | 0.085560 | 0.091523 | +0.005963 | -6.97% |
| test_feynman_transpile[gf2^8_mult.qasm] | fake_torino | 3 | 3 | 0.112734 | 0.117430 | +0.004696 | -4.17% |
| test_feynman_transpile[qft_4.qasm] | fake_torino | 2 | 3 | 0.008367 | 0.008940 | +0.000572 | -6.84% |
| test_feynman_transpile[qft_4.qasm] | fake_torino | 3 | 3 | 0.009790 | 0.010372 | +0.000581 | -5.94% |
| test_feynman_transpile[rc_adder_6.qasm] | fake_torino | 2 | 3 | 0.016025 | 0.016717 | +0.000691 | -4.32% |
| test_feynman_transpile[rc_adder_6.qasm] | fake_torino | 3 | 3 | 0.017904 | 0.019690 | +0.001786 | -9.97% |
| test_hamlib_hamiltonians_transpile[ham_bh_graph-1D-grid-pbc-qubitnodes_Lx-14_U-10_enc-stdbinary_d-4] | fake_torino | 2 | 3 | 0.061837 | 0.065759 | +0.003922 | -6.34% |
| test_hamlib_hamiltonians_transpile[ham_bh_graph-1D-grid-pbc-qubitnodes_Lx-14_U-10_enc-stdbinary_d-4] | fake_torino | 3 | 3 | 0.094094 | 0.088920 | -0.005174 | +5.50% |
| test_hamlib_hamiltonians_transpile[ham_complbipart-n-10_a-5_b-5] | fake_torino | 2 | 3 | 0.016842 | 0.016634 | -0.000209 | +1.24% |
| test_hamlib_hamiltonians_transpile[ham_complbipart-n-10_a-5_b-5] | fake_torino | 3 | 3 | 0.022451 | 0.021348 | -0.001103 | +4.91% |
| test_hamlib_hamiltonians_transpile[ham_ham_JW14] | fake_torino | 2 | 3 | 0.404160 | 0.455961 | +0.051801 | -12.82% |
| test_hamlib_hamiltonians_transpile[ham_ham_JW14] | fake_torino | 3 | 3 | 0.508733 | 0.560675 | +0.051943 | -10.21% |
| test_hamlib_hamiltonians_transpile[ham_tsp_prob-ts225_Ncity-5_enc-unary] | fake_torino | 2 | 3 | 0.053353 | 0.053437 | +0.000085 | -0.16% |
| test_hamlib_hamiltonians_transpile[ham_tsp_prob-ts225_Ncity-5_enc-unary] | fake_torino | 3 | 3 | 0.067361 | 0.069658 | +0.002297 | -3.41% |
| test_BV_100_transpile | fake_torino | 2 | 3 | 0.060057 | 0.058735 | -0.001322 | +2.20% |
| test_BV_100_transpile | fake_torino | 3 | 3 | 15.128292 | 15.140950 | +0.012658 | -0.08% |
| test_BVlike_simplification_transpile | fake_torino | 2 | 3 | 0.006968 | 0.005194 | -0.001774 | +25.46% |
| test_BVlike_simplification_transpile | fake_torino | 3 | 3 | 0.005645 | 0.005392 | -0.000254 | +4.49% |
| test_QAOA_100_transpile | fake_torino | 2 | 3 | 0.754655 | 0.770751 | +0.016097 | -2.13% |
| test_QAOA_100_transpile | fake_torino | 3 | 3 | 0.998698 | 1.020865 | +0.022167 | -2.22% |
| test_QFT_100_transpile | fake_torino | 2 | 3 | 0.893760 | 0.928186 | +0.034426 | -3.85% |
| test_QFT_100_transpile | fake_torino | 3 | 3 | 1.234399 | 1.217548 | -0.016851 | +1.37% |
| test_QV_100_transpile | fake_torino | 2 | 3 | 16.256553 | 16.500426 | +0.243873 | -1.50% |
| test_QV_100_transpile | fake_torino | 3 | 3 | 19.890029 | 20.116111 | +0.226081 | -1.14% |
| test_circSU2_100_transpile | fake_torino | 2 | 3 | 0.070315 | 0.069895 | -0.000420 | +0.60% |
| test_circSU2_100_transpile | fake_torino | 3 | 3 | 0.286716 | 0.285595 | -0.001121 | +0.39% |
| test_circSU2_89_transpile | fake_torino | 2 | 3 | 3.383666 | 3.155414 | -0.228252 | +6.75% |
| test_circSU2_89_transpile | fake_torino | 3 | 3 | 35.671735 | 35.953894 | +0.282159 | -0.79% |
| test_clifford_100_transpile | fake_torino | 2 | 3 | 3.190061 | 3.316106 | +0.126045 | -3.95% |
| test_clifford_100_transpile | fake_torino | 3 | 3 | 4.534202 | 4.626147 | +0.091945 | -2.03% |
| test_square_heisenberg_100_transpile | fake_torino | 2 | 3 | 0.165706 | 0.176578 | +0.010873 | -6.56% |
| test_square_heisenberg_100_transpile | fake_torino | 3 | 3 | 0.202356 | 0.207984 | +0.005628 | -2.78% |

### Topology breakdown

Quality improvement by topology (equal case weights within each topology). Ratio cases counts the cases with a defined ratio for each metric.

| Level | Topology | Complete cases | D2 ratio cases | D2 improvement | N2 ratio cases | N2 improvement |
| --- | --- | --- | --- | --- | --- | --- |
| 2 | all-to-all | 8/8 | 8 | +0.00% | 8 | +0.00% |
| 2 | fake_torino | 18/18 | 17 | +1.82% | 17 | +1.84% |
| 2 | heavy-hex | 8/8 | 8 | +3.97% | 8 | +2.11% |
| 2 | linear | 8/8 | 8 | +6.41% | 8 | +1.83% |
| 2 | square | 8/8 | 8 | +2.67% | 8 | +2.64% |
| 3 | all-to-all | 8/8 | 8 | +0.00% | 8 | +0.00% |
| 3 | fake_torino | 18/18 | 17 | +1.73% | 17 | +1.78% |
| 3 | heavy-hex | 8/8 | 8 | +4.05% | 8 | +2.20% |
| 3 | linear | 8/8 | 8 | +4.78% | 8 | +2.04% |
| 3 | square | 8/8 | 8 | +2.56% | 8 | +2.54% |

<details>
<summary>Paired-seed statistics and full test IDs</summary>

Baseline and evolved columns are independent seed medians. Paired changes and ratios are calculated per seed before taking their medians; they need not equal the subtraction or division of the displayed baseline and evolved medians. Paired improvement is calculated from the median paired ratio.

| Case | Level | Paired seeds | Metric | Baseline median | Evolved median | Median paired change | Median paired ratio | Paired improvement |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| benchpress/qiskit_gym/abstract_transpile/test_hamiltonians.py::TestWorkoutAbstractHamiltonians::test_hamiltonians[ham_bh_graph-1D-grid-pbc-qubitnodes_Lx-14_U-10_enc-stdbinary_d-4-all-to-all] | 2 | 3 | D2 | 978 | 978 | 0 | 1.0 | +0.00% |
| benchpress/qiskit_gym/abstract_transpile/test_hamiltonians.py::TestWorkoutAbstractHamiltonians::test_hamiltonians[ham_bh_graph-1D-grid-pbc-qubitnodes_Lx-14_U-10_enc-stdbinary_d-4-all-to-all] | 2 | 3 | N2 | 1066 | 1066 | 0 | 1.0 | +0.00% |
| benchpress/qiskit_gym/abstract_transpile/test_hamiltonians.py::TestWorkoutAbstractHamiltonians::test_hamiltonians[ham_bh_graph-1D-grid-pbc-qubitnodes_Lx-14_U-10_enc-stdbinary_d-4-all-to-all] | 2 | 3 | runtime_s | 0.04606320895254612 | 0.04631354194134474 | 0.0002503329887986183 | 1.0054345538335487 | -0.54% |
| benchpress/qiskit_gym/abstract_transpile/test_hamiltonians.py::TestWorkoutAbstractHamiltonians::test_hamiltonians[ham_bh_graph-1D-grid-pbc-qubitnodes_Lx-14_U-10_enc-stdbinary_d-4-all-to-all] | 3 | 3 | D2 | 981 | 981 | 0 | 1.0 | +0.00% |
| benchpress/qiskit_gym/abstract_transpile/test_hamiltonians.py::TestWorkoutAbstractHamiltonians::test_hamiltonians[ham_bh_graph-1D-grid-pbc-qubitnodes_Lx-14_U-10_enc-stdbinary_d-4-all-to-all] | 3 | 3 | N2 | 1068 | 1068 | 0 | 1.0 | +0.00% |
| benchpress/qiskit_gym/abstract_transpile/test_hamiltonians.py::TestWorkoutAbstractHamiltonians::test_hamiltonians[ham_bh_graph-1D-grid-pbc-qubitnodes_Lx-14_U-10_enc-stdbinary_d-4-all-to-all] | 3 | 3 | runtime_s | 0.3570335421245545 | 0.34019916714169085 | -0.0010722498409450054 | 0.9968580731125233 | +0.31% |
| benchpress/qiskit_gym/abstract_transpile/test_hamiltonians.py::TestWorkoutAbstractHamiltonians::test_hamiltonians[ham_bh_graph-1D-grid-pbc-qubitnodes_Lx-14_U-10_enc-stdbinary_d-4-heavy-hex] | 2 | 3 | D2 | 947 | 947 | 0 | 1.0 | +0.00% |
| benchpress/qiskit_gym/abstract_transpile/test_hamiltonians.py::TestWorkoutAbstractHamiltonians::test_hamiltonians[ham_bh_graph-1D-grid-pbc-qubitnodes_Lx-14_U-10_enc-stdbinary_d-4-heavy-hex] | 2 | 3 | N2 | 1010 | 1010 | 0 | 1.0 | +0.00% |
| benchpress/qiskit_gym/abstract_transpile/test_hamiltonians.py::TestWorkoutAbstractHamiltonians::test_hamiltonians[ham_bh_graph-1D-grid-pbc-qubitnodes_Lx-14_U-10_enc-stdbinary_d-4-heavy-hex] | 2 | 3 | runtime_s | 0.059285541996359825 | 0.06032479181885719 | 0.002326499903574586 | 1.03924228108967 | -3.92% |
| benchpress/qiskit_gym/abstract_transpile/test_hamiltonians.py::TestWorkoutAbstractHamiltonians::test_hamiltonians[ham_bh_graph-1D-grid-pbc-qubitnodes_Lx-14_U-10_enc-stdbinary_d-4-heavy-hex] | 3 | 3 | D2 | 937 | 937 | 0 | 1.0 | +0.00% |
| benchpress/qiskit_gym/abstract_transpile/test_hamiltonians.py::TestWorkoutAbstractHamiltonians::test_hamiltonians[ham_bh_graph-1D-grid-pbc-qubitnodes_Lx-14_U-10_enc-stdbinary_d-4-heavy-hex] | 3 | 3 | N2 | 1002 | 1002 | 0 | 1.0 | +0.00% |
| benchpress/qiskit_gym/abstract_transpile/test_hamiltonians.py::TestWorkoutAbstractHamiltonians::test_hamiltonians[ham_bh_graph-1D-grid-pbc-qubitnodes_Lx-14_U-10_enc-stdbinary_d-4-heavy-hex] | 3 | 3 | runtime_s | 0.08408658299595118 | 0.08906429191119969 | 0.004977708915248513 | 1.0591974217276519 | -5.92% |
| benchpress/qiskit_gym/abstract_transpile/test_hamiltonians.py::TestWorkoutAbstractHamiltonians::test_hamiltonians[ham_bh_graph-1D-grid-pbc-qubitnodes_Lx-14_U-10_enc-stdbinary_d-4-linear] | 2 | 3 | D2 | 1082 | 1082 | 0 | 1.0 | +0.00% |
| benchpress/qiskit_gym/abstract_transpile/test_hamiltonians.py::TestWorkoutAbstractHamiltonians::test_hamiltonians[ham_bh_graph-1D-grid-pbc-qubitnodes_Lx-14_U-10_enc-stdbinary_d-4-linear] | 2 | 3 | N2 | 1199 | 1199 | 0 | 1.0 | +0.00% |
| benchpress/qiskit_gym/abstract_transpile/test_hamiltonians.py::TestWorkoutAbstractHamiltonians::test_hamiltonians[ham_bh_graph-1D-grid-pbc-qubitnodes_Lx-14_U-10_enc-stdbinary_d-4-linear] | 2 | 3 | runtime_s | 0.05358591699041426 | 0.05457366677001119 | 0.004362832754850388 | 1.086890266621205 | -8.69% |
| benchpress/qiskit_gym/abstract_transpile/test_hamiltonians.py::TestWorkoutAbstractHamiltonians::test_hamiltonians[ham_bh_graph-1D-grid-pbc-qubitnodes_Lx-14_U-10_enc-stdbinary_d-4-linear] | 3 | 3 | D2 | 1082 | 1082 | 0 | 1.0 | +0.00% |
| benchpress/qiskit_gym/abstract_transpile/test_hamiltonians.py::TestWorkoutAbstractHamiltonians::test_hamiltonians[ham_bh_graph-1D-grid-pbc-qubitnodes_Lx-14_U-10_enc-stdbinary_d-4-linear] | 3 | 3 | N2 | 1199 | 1199 | 0 | 1.0 | +0.00% |
| benchpress/qiskit_gym/abstract_transpile/test_hamiltonians.py::TestWorkoutAbstractHamiltonians::test_hamiltonians[ham_bh_graph-1D-grid-pbc-qubitnodes_Lx-14_U-10_enc-stdbinary_d-4-linear] | 3 | 3 | runtime_s | 0.06820620782673359 | 0.07195508386939764 | 0.0035208752378821373 | 1.0516210378801052 | -5.16% |
| benchpress/qiskit_gym/abstract_transpile/test_hamiltonians.py::TestWorkoutAbstractHamiltonians::test_hamiltonians[ham_bh_graph-1D-grid-pbc-qubitnodes_Lx-14_U-10_enc-stdbinary_d-4-square] | 2 | 3 | D2 | 947 | 947 | 0 | 1.0 | +0.00% |
| benchpress/qiskit_gym/abstract_transpile/test_hamiltonians.py::TestWorkoutAbstractHamiltonians::test_hamiltonians[ham_bh_graph-1D-grid-pbc-qubitnodes_Lx-14_U-10_enc-stdbinary_d-4-square] | 2 | 3 | N2 | 1004 | 1004 | 0 | 1.0 | +0.00% |
| benchpress/qiskit_gym/abstract_transpile/test_hamiltonians.py::TestWorkoutAbstractHamiltonians::test_hamiltonians[ham_bh_graph-1D-grid-pbc-qubitnodes_Lx-14_U-10_enc-stdbinary_d-4-square] | 2 | 3 | runtime_s | 0.06750483298674226 | 0.06307229190133512 | 0.004968584049493074 | 1.0863771507053142 | -8.64% |
| benchpress/qiskit_gym/abstract_transpile/test_hamiltonians.py::TestWorkoutAbstractHamiltonians::test_hamiltonians[ham_bh_graph-1D-grid-pbc-qubitnodes_Lx-14_U-10_enc-stdbinary_d-4-square] | 3 | 3 | D2 | 925 | 925 | 0 | 1.0 | +0.00% |
| benchpress/qiskit_gym/abstract_transpile/test_hamiltonians.py::TestWorkoutAbstractHamiltonians::test_hamiltonians[ham_bh_graph-1D-grid-pbc-qubitnodes_Lx-14_U-10_enc-stdbinary_d-4-square] | 3 | 3 | N2 | 983 | 983 | 0 | 1.0 | +0.00% |
| benchpress/qiskit_gym/abstract_transpile/test_hamiltonians.py::TestWorkoutAbstractHamiltonians::test_hamiltonians[ham_bh_graph-1D-grid-pbc-qubitnodes_Lx-14_U-10_enc-stdbinary_d-4-square] | 3 | 3 | runtime_s | 0.2101798749063164 | 0.21380649995990098 | 0.0036266250535845757 | 1.0172548635077505 | -1.73% |
| benchpress/qiskit_gym/abstract_transpile/test_hamiltonians.py::TestWorkoutAbstractHamiltonians::test_hamiltonians[ham_ham_JW14-all-to-all] | 2 | 3 | D2 | 2334 | 2334 | 0 | 1.0 | +0.00% |
| benchpress/qiskit_gym/abstract_transpile/test_hamiltonians.py::TestWorkoutAbstractHamiltonians::test_hamiltonians[ham_ham_JW14-all-to-all] | 2 | 3 | N2 | 3332 | 3332 | 0 | 1.0 | +0.00% |
| benchpress/qiskit_gym/abstract_transpile/test_hamiltonians.py::TestWorkoutAbstractHamiltonians::test_hamiltonians[ham_ham_JW14-all-to-all] | 2 | 3 | runtime_s | 0.12271225010044873 | 0.12387095810845494 | 0.0004776250571012497 | 1.0038707525381656 | -0.39% |
| benchpress/qiskit_gym/abstract_transpile/test_hamiltonians.py::TestWorkoutAbstractHamiltonians::test_hamiltonians[ham_ham_JW14-all-to-all] | 3 | 3 | D2 | 2330 | 2330 | 0 | 1.0 | +0.00% |
| benchpress/qiskit_gym/abstract_transpile/test_hamiltonians.py::TestWorkoutAbstractHamiltonians::test_hamiltonians[ham_ham_JW14-all-to-all] | 3 | 3 | N2 | 3328 | 3328 | 0 | 1.0 | +0.00% |
| benchpress/qiskit_gym/abstract_transpile/test_hamiltonians.py::TestWorkoutAbstractHamiltonians::test_hamiltonians[ham_ham_JW14-all-to-all] | 3 | 3 | runtime_s | 0.6698080408386886 | 0.6407695829402655 | -0.029038457898423076 | 0.9566465970428437 | +4.34% |
| benchpress/qiskit_gym/abstract_transpile/test_hamiltonians.py::TestWorkoutAbstractHamiltonians::test_hamiltonians[ham_ham_JW14-heavy-hex] | 2 | 3 | D2 | 6274 | 6246 | -29 | 0.9955371373924131 | +0.45% |
| benchpress/qiskit_gym/abstract_transpile/test_hamiltonians.py::TestWorkoutAbstractHamiltonians::test_hamiltonians[ham_ham_JW14-heavy-hex] | 2 | 3 | N2 | 7286 | 7262 | -24 | 0.9967060115289597 | +0.33% |
| benchpress/qiskit_gym/abstract_transpile/test_hamiltonians.py::TestWorkoutAbstractHamiltonians::test_hamiltonians[ham_ham_JW14-heavy-hex] | 2 | 3 | runtime_s | 0.4311139159835875 | 0.4461604589596391 | 0.018814583076164126 | 1.0409653128991538 | -4.10% |
| benchpress/qiskit_gym/abstract_transpile/test_hamiltonians.py::TestWorkoutAbstractHamiltonians::test_hamiltonians[ham_ham_JW14-heavy-hex] | 3 | 3 | D2 | 5064 | 5035 | -36 | 0.9927884615384616 | +0.72% |
| benchpress/qiskit_gym/abstract_transpile/test_hamiltonians.py::TestWorkoutAbstractHamiltonians::test_hamiltonians[ham_ham_JW14-heavy-hex] | 3 | 3 | N2 | 6037 | 6003 | -24 | 0.9960532807104094 | +0.39% |
| benchpress/qiskit_gym/abstract_transpile/test_hamiltonians.py::TestWorkoutAbstractHamiltonians::test_hamiltonians[ham_ham_JW14-heavy-hex] | 3 | 3 | runtime_s | 0.6046146668959409 | 0.6657887080218643 | 0.04355895798653364 | 1.0662799772361924 | -6.63% |
| benchpress/qiskit_gym/abstract_transpile/test_hamiltonians.py::TestWorkoutAbstractHamiltonians::test_hamiltonians[ham_ham_JW14-linear] | 2 | 3 | D2 | 5949 | 5935 | -10 | 0.9983170649612925 | +0.17% |
| benchpress/qiskit_gym/abstract_transpile/test_hamiltonians.py::TestWorkoutAbstractHamiltonians::test_hamiltonians[ham_ham_JW14-linear] | 2 | 3 | N2 | 6865 | 6857 | -6 | 0.9991251093613298 | +0.09% |
| benchpress/qiskit_gym/abstract_transpile/test_hamiltonians.py::TestWorkoutAbstractHamiltonians::test_hamiltonians[ham_ham_JW14-linear] | 2 | 3 | runtime_s | 0.33635616721585393 | 0.3681194169912487 | -0.004965459229424596 | 0.9852374961026416 | +1.48% |
| benchpress/qiskit_gym/abstract_transpile/test_hamiltonians.py::TestWorkoutAbstractHamiltonians::test_hamiltonians[ham_ham_JW14-linear] | 3 | 3 | D2 | 5099 | 5085 | -10 | 0.9980361351139042 | +0.20% |
| benchpress/qiskit_gym/abstract_transpile/test_hamiltonians.py::TestWorkoutAbstractHamiltonians::test_hamiltonians[ham_ham_JW14-linear] | 3 | 3 | N2 | 5942 | 5934 | -6 | 0.998989048020219 | +0.10% |
| benchpress/qiskit_gym/abstract_transpile/test_hamiltonians.py::TestWorkoutAbstractHamiltonians::test_hamiltonians[ham_ham_JW14-linear] | 3 | 3 | runtime_s | 0.4673466661479324 | 0.475706874858588 | 0.009908792097121477 | 1.0210293626934037 | -2.10% |
| benchpress/qiskit_gym/abstract_transpile/test_hamiltonians.py::TestWorkoutAbstractHamiltonians::test_hamiltonians[ham_ham_JW14-square] | 2 | 3 | D2 | 5461 | 5439 | -30 | 0.9944403261675315 | +0.56% |
| benchpress/qiskit_gym/abstract_transpile/test_hamiltonians.py::TestWorkoutAbstractHamiltonians::test_hamiltonians[ham_ham_JW14-square] | 2 | 3 | N2 | 6326 | 6302 | -24 | 0.9962061334176415 | +0.38% |
| benchpress/qiskit_gym/abstract_transpile/test_hamiltonians.py::TestWorkoutAbstractHamiltonians::test_hamiltonians[ham_ham_JW14-square] | 2 | 3 | runtime_s | 0.41053154109977186 | 0.41737350006587803 | 0.006841958966106176 | 1.0166660981706235 | -1.67% |
| benchpress/qiskit_gym/abstract_transpile/test_hamiltonians.py::TestWorkoutAbstractHamiltonians::test_hamiltonians[ham_ham_JW14-square] | 3 | 3 | D2 | 4802 | 4782 | -25 | 0.994908350305499 | +0.51% |
| benchpress/qiskit_gym/abstract_transpile/test_hamiltonians.py::TestWorkoutAbstractHamiltonians::test_hamiltonians[ham_ham_JW14-square] | 3 | 3 | N2 | 5570 | 5546 | -24 | 0.9956912028725314 | +0.43% |
| benchpress/qiskit_gym/abstract_transpile/test_hamiltonians.py::TestWorkoutAbstractHamiltonians::test_hamiltonians[ham_ham_JW14-square] | 3 | 3 | runtime_s | 0.5742635419592261 | 0.5771515411324799 | 0.014859790913760662 | 1.0274770577519707 | -2.75% |
| benchpress/qiskit_gym/abstract_transpile/test_qasmbench.py::TestWorkoutAbstractQasmBenchLarge::test_QASMBench_large[qft_n29-all-to-all] | 2 | 3 | D2 | 110 | 110 | 0 | 1.0 | +0.00% |
| benchpress/qiskit_gym/abstract_transpile/test_qasmbench.py::TestWorkoutAbstractQasmBenchLarge::test_QASMBench_large[qft_n29-all-to-all] | 2 | 3 | N2 | 602 | 602 | 0 | 1.0 | +0.00% |
| benchpress/qiskit_gym/abstract_transpile/test_qasmbench.py::TestWorkoutAbstractQasmBenchLarge::test_QASMBench_large[qft_n29-all-to-all] | 2 | 3 | runtime_s | 0.033103999914601445 | 0.034365416038781404 | 0.0009368329774588346 | 1.0280249083767707 | -2.80% |
| benchpress/qiskit_gym/abstract_transpile/test_qasmbench.py::TestWorkoutAbstractQasmBenchLarge::test_QASMBench_large[qft_n29-all-to-all] | 3 | 3 | D2 | 110 | 110 | 0 | 1.0 | +0.00% |
| benchpress/qiskit_gym/abstract_transpile/test_qasmbench.py::TestWorkoutAbstractQasmBenchLarge::test_QASMBench_large[qft_n29-all-to-all] | 3 | 3 | N2 | 602 | 602 | 0 | 1.0 | +0.00% |
| benchpress/qiskit_gym/abstract_transpile/test_qasmbench.py::TestWorkoutAbstractQasmBenchLarge::test_QASMBench_large[qft_n29-all-to-all] | 3 | 3 | runtime_s | 0.8687987921293825 | 0.8744354580994695 | -0.00036291778087615967 | 0.9995798408785662 | +0.04% |
| benchpress/qiskit_gym/abstract_transpile/test_qasmbench.py::TestWorkoutAbstractQasmBenchLarge::test_QASMBench_large[qft_n29-heavy-hex] | 2 | 3 | D2 | 353 | 297 | -39 | 0.8940217391304348 | +10.60% |
| benchpress/qiskit_gym/abstract_transpile/test_qasmbench.py::TestWorkoutAbstractQasmBenchLarge::test_QASMBench_large[qft_n29-heavy-hex] | 2 | 3 | N2 | 1352 | 1270 | -82 | 0.9393491124260355 | +6.07% |
| benchpress/qiskit_gym/abstract_transpile/test_qasmbench.py::TestWorkoutAbstractQasmBenchLarge::test_QASMBench_large[qft_n29-heavy-hex] | 2 | 3 | runtime_s | 0.14500549994409084 | 0.15161633398383856 | 0.006460541859269142 | 1.044507640823074 | -4.45% |
| benchpress/qiskit_gym/abstract_transpile/test_qasmbench.py::TestWorkoutAbstractQasmBenchLarge::test_QASMBench_large[qft_n29-heavy-hex] | 3 | 3 | D2 | 326 | 279 | -40 | 0.8773006134969326 | +12.27% |
| benchpress/qiskit_gym/abstract_transpile/test_qasmbench.py::TestWorkoutAbstractQasmBenchLarge::test_QASMBench_large[qft_n29-heavy-hex] | 3 | 3 | N2 | 1284 | 1202 | -82 | 0.9361370716510904 | +6.39% |
| benchpress/qiskit_gym/abstract_transpile/test_qasmbench.py::TestWorkoutAbstractQasmBenchLarge::test_QASMBench_large[qft_n29-heavy-hex] | 3 | 3 | runtime_s | 0.1823852499946952 | 0.18848562496714294 | 0.006100374972447753 | 1.0334477430199271 | -3.34% |
| benchpress/qiskit_gym/abstract_transpile/test_qasmbench.py::TestWorkoutAbstractQasmBenchLarge::test_QASMBench_large[qft_n29-linear] | 2 | 3 | D2 | 277 | 231 | -58 | 0.7906137184115524 | +20.94% |
| benchpress/qiskit_gym/abstract_transpile/test_qasmbench.py::TestWorkoutAbstractQasmBenchLarge::test_QASMBench_large[qft_n29-linear] | 2 | 3 | N2 | 1347 | 1295 | -58 | 0.9566840926064227 | +4.33% |
| benchpress/qiskit_gym/abstract_transpile/test_qasmbench.py::TestWorkoutAbstractQasmBenchLarge::test_QASMBench_large[qft_n29-linear] | 2 | 3 | runtime_s | 0.11629804200492799 | 0.12433891696855426 | 0.008040874963626266 | 1.0691402436791286 | -6.91% |
| benchpress/qiskit_gym/abstract_transpile/test_qasmbench.py::TestWorkoutAbstractQasmBenchLarge::test_QASMBench_large[qft_n29-linear] | 3 | 3 | D2 | 274 | 246 | -25 | 0.9087591240875912 | +9.12% |
| benchpress/qiskit_gym/abstract_transpile/test_qasmbench.py::TestWorkoutAbstractQasmBenchLarge::test_QASMBench_large[qft_n29-linear] | 3 | 3 | N2 | 1373 | 1308 | -46 | 0.9664967225054625 | +3.35% |
| benchpress/qiskit_gym/abstract_transpile/test_qasmbench.py::TestWorkoutAbstractQasmBenchLarge::test_QASMBench_large[qft_n29-linear] | 3 | 3 | runtime_s | 0.15057454211637378 | 0.1491475000511855 | -0.0014270420651882887 | 0.9905226870018613 | +0.95% |
| benchpress/qiskit_gym/abstract_transpile/test_qasmbench.py::TestWorkoutAbstractQasmBenchLarge::test_QASMBench_large[qft_n29-square] | 2 | 3 | D2 | 383 | 342 | -52 | 0.8779342723004695 | +12.21% |
| benchpress/qiskit_gym/abstract_transpile/test_qasmbench.py::TestWorkoutAbstractQasmBenchLarge::test_QASMBench_large[qft_n29-square] | 2 | 3 | N2 | 1259 | 1123 | -122 | 0.9044635865309318 | +9.55% |
| benchpress/qiskit_gym/abstract_transpile/test_qasmbench.py::TestWorkoutAbstractQasmBenchLarge::test_QASMBench_large[qft_n29-square] | 2 | 3 | runtime_s | 0.12215354200452566 | 0.14221325004473329 | 0.0035097908694297075 | 1.0287326164418522 | -2.87% |
| benchpress/qiskit_gym/abstract_transpile/test_qasmbench.py::TestWorkoutAbstractQasmBenchLarge::test_QASMBench_large[qft_n29-square] | 3 | 3 | D2 | 386 | 342 | -44 | 0.8860103626943006 | +11.40% |
| benchpress/qiskit_gym/abstract_transpile/test_qasmbench.py::TestWorkoutAbstractQasmBenchLarge::test_QASMBench_large[qft_n29-square] | 3 | 3 | N2 | 1214 | 1095 | -120 | 0.9012345679012346 | +9.88% |
| benchpress/qiskit_gym/abstract_transpile/test_qasmbench.py::TestWorkoutAbstractQasmBenchLarge::test_QASMBench_large[qft_n29-square] | 3 | 3 | runtime_s | 0.16462279087863863 | 0.178841165965423 | 0.005049459170550108 | 1.0306729046664784 | -3.07% |
| benchpress/qiskit_gym/abstract_transpile/test_qasmbench.py::TestWorkoutAbstractQasmBenchLarge::test_QASMBench_large[swap_test_n41-all-to-all] | 2 | 3 | D2 | 102 | 102 | 0 | 1.0 | +0.00% |
| benchpress/qiskit_gym/abstract_transpile/test_qasmbench.py::TestWorkoutAbstractQasmBenchLarge::test_QASMBench_large[swap_test_n41-all-to-all] | 2 | 3 | N2 | 140 | 140 | 0 | 1.0 | +0.00% |
| benchpress/qiskit_gym/abstract_transpile/test_qasmbench.py::TestWorkoutAbstractQasmBenchLarge::test_QASMBench_large[swap_test_n41-all-to-all] | 2 | 3 | runtime_s | 0.016862332820892334 | 0.016877250047400594 | 1.4917226508259773e-05 | 1.000884647851914 | -0.09% |
| benchpress/qiskit_gym/abstract_transpile/test_qasmbench.py::TestWorkoutAbstractQasmBenchLarge::test_QASMBench_large[swap_test_n41-all-to-all] | 3 | 3 | D2 | 102 | 102 | 0 | 1.0 | +0.00% |
| benchpress/qiskit_gym/abstract_transpile/test_qasmbench.py::TestWorkoutAbstractQasmBenchLarge::test_QASMBench_large[swap_test_n41-all-to-all] | 3 | 3 | N2 | 140 | 140 | 0 | 1.0 | +0.00% |
| benchpress/qiskit_gym/abstract_transpile/test_qasmbench.py::TestWorkoutAbstractQasmBenchLarge::test_QASMBench_large[swap_test_n41-all-to-all] | 3 | 3 | runtime_s | 0.43043025000952184 | 0.41601329087279737 | -0.012502334080636501 | 0.9708069232978355 | +2.92% |
| benchpress/qiskit_gym/abstract_transpile/test_qasmbench.py::TestWorkoutAbstractQasmBenchLarge::test_QASMBench_large[swap_test_n41-heavy-hex] | 2 | 3 | D2 | 302 | 302 | 0 | 1.0 | +0.00% |
| benchpress/qiskit_gym/abstract_transpile/test_qasmbench.py::TestWorkoutAbstractQasmBenchLarge::test_QASMBench_large[swap_test_n41-heavy-hex] | 2 | 3 | N2 | 369 | 369 | 0 | 1.0 | +0.00% |
| benchpress/qiskit_gym/abstract_transpile/test_qasmbench.py::TestWorkoutAbstractQasmBenchLarge::test_QASMBench_large[swap_test_n41-heavy-hex] | 2 | 3 | runtime_s | 0.026097415946424007 | 0.026307124877348542 | 0.0012616247404366732 | 1.0472776847623404 | -4.73% |
| benchpress/qiskit_gym/abstract_transpile/test_qasmbench.py::TestWorkoutAbstractQasmBenchLarge::test_QASMBench_large[swap_test_n41-heavy-hex] | 3 | 3 | D2 | 298 | 298 | -3 | 0.9908256880733946 | +0.92% |
| benchpress/qiskit_gym/abstract_transpile/test_qasmbench.py::TestWorkoutAbstractQasmBenchLarge::test_QASMBench_large[swap_test_n41-heavy-hex] | 3 | 3 | N2 | 373 | 373 | -2 | 0.9947916666666666 | +0.52% |
| benchpress/qiskit_gym/abstract_transpile/test_qasmbench.py::TestWorkoutAbstractQasmBenchLarge::test_QASMBench_large[swap_test_n41-heavy-hex] | 3 | 3 | runtime_s | 0.03301575011573732 | 0.03247874998487532 | 0.0016826668288558722 | 1.054638988352224 | -5.46% |
| benchpress/qiskit_gym/abstract_transpile/test_qasmbench.py::TestWorkoutAbstractQasmBenchLarge::test_QASMBench_large[swap_test_n41-linear] | 2 | 3 | D2 | 184 | 184 | 0 | 1.0 | +0.00% |
| benchpress/qiskit_gym/abstract_transpile/test_qasmbench.py::TestWorkoutAbstractQasmBenchLarge::test_QASMBench_large[swap_test_n41-linear] | 2 | 3 | N2 | 235 | 235 | 0 | 1.0 | +0.00% |
| benchpress/qiskit_gym/abstract_transpile/test_qasmbench.py::TestWorkoutAbstractQasmBenchLarge::test_QASMBench_large[swap_test_n41-linear] | 2 | 3 | runtime_s | 0.02158704213798046 | 0.02309799985960126 | 0.0015109577216207981 | 1.0724688337254744 | -7.25% |
| benchpress/qiskit_gym/abstract_transpile/test_qasmbench.py::TestWorkoutAbstractQasmBenchLarge::test_QASMBench_large[swap_test_n41-linear] | 3 | 3 | D2 | 184 | 184 | 0 | 1.0 | +0.00% |
| benchpress/qiskit_gym/abstract_transpile/test_qasmbench.py::TestWorkoutAbstractQasmBenchLarge::test_QASMBench_large[swap_test_n41-linear] | 3 | 3 | N2 | 235 | 235 | 0 | 1.0 | +0.00% |
| benchpress/qiskit_gym/abstract_transpile/test_qasmbench.py::TestWorkoutAbstractQasmBenchLarge::test_QASMBench_large[swap_test_n41-linear] | 3 | 3 | runtime_s | 0.026612708112224936 | 0.02753191697411239 | 0.0016524577513337135 | 1.0642757701955368 | -6.43% |
| benchpress/qiskit_gym/abstract_transpile/test_qasmbench.py::TestWorkoutAbstractQasmBenchLarge::test_QASMBench_large[swap_test_n41-square] | 2 | 3 | D2 | 208 | 208 | 0 | 1.0 | +0.00% |
| benchpress/qiskit_gym/abstract_transpile/test_qasmbench.py::TestWorkoutAbstractQasmBenchLarge::test_QASMBench_large[swap_test_n41-square] | 2 | 3 | N2 | 291 | 290 | 0 | 1.0 | +0.00% |
| benchpress/qiskit_gym/abstract_transpile/test_qasmbench.py::TestWorkoutAbstractQasmBenchLarge::test_QASMBench_large[swap_test_n41-square] | 2 | 3 | runtime_s | 0.028988208854570985 | 0.029641666915267706 | 0.0006534580606967211 | 1.0225422020372148 | -2.25% |
| benchpress/qiskit_gym/abstract_transpile/test_qasmbench.py::TestWorkoutAbstractQasmBenchLarge::test_QASMBench_large[swap_test_n41-square] | 3 | 3 | D2 | 221 | 221 | 0 | 1.0 | +0.00% |
| benchpress/qiskit_gym/abstract_transpile/test_qasmbench.py::TestWorkoutAbstractQasmBenchLarge::test_QASMBench_large[swap_test_n41-square] | 3 | 3 | N2 | 298 | 296 | 0 | 1.0 | +0.00% |
| benchpress/qiskit_gym/abstract_transpile/test_qasmbench.py::TestWorkoutAbstractQasmBenchLarge::test_QASMBench_large[swap_test_n41-square] | 3 | 3 | runtime_s | 0.04296358278952539 | 0.04369379091076553 | 0.000730208121240139 | 1.016995978310686 | -1.70% |
| benchpress/qiskit_gym/abstract_transpile/test_qasmbench.py::TestWorkoutAbstractQasmBenchMedium::test_QASMBench_medium[ising_n26-all-to-all] | 2 | 3 | D2 | 4 | 4 | 0 | 1.0 | +0.00% |
| benchpress/qiskit_gym/abstract_transpile/test_qasmbench.py::TestWorkoutAbstractQasmBenchMedium::test_QASMBench_medium[ising_n26-all-to-all] | 2 | 3 | N2 | 50 | 50 | 0 | 1.0 | +0.00% |
| benchpress/qiskit_gym/abstract_transpile/test_qasmbench.py::TestWorkoutAbstractQasmBenchMedium::test_QASMBench_medium[ising_n26-all-to-all] | 2 | 3 | runtime_s | 0.008265624986961484 | 0.007809292059391737 | -0.0005264580249786377 | 0.9363075356299018 | +6.37% |
| benchpress/qiskit_gym/abstract_transpile/test_qasmbench.py::TestWorkoutAbstractQasmBenchMedium::test_QASMBench_medium[ising_n26-all-to-all] | 3 | 3 | D2 | 4 | 4 | 0 | 1.0 | +0.00% |
| benchpress/qiskit_gym/abstract_transpile/test_qasmbench.py::TestWorkoutAbstractQasmBenchMedium::test_QASMBench_medium[ising_n26-all-to-all] | 3 | 3 | N2 | 50 | 50 | 0 | 1.0 | +0.00% |
| benchpress/qiskit_gym/abstract_transpile/test_qasmbench.py::TestWorkoutAbstractQasmBenchMedium::test_QASMBench_medium[ising_n26-all-to-all] | 3 | 3 | runtime_s | 0.21291870810091496 | 0.2126912500243634 | -0.0002274580765515566 | 0.9989317139927237 | +0.11% |
| benchpress/qiskit_gym/abstract_transpile/test_qasmbench.py::TestWorkoutAbstractQasmBenchMedium::test_QASMBench_medium[ising_n26-heavy-hex] | 2 | 3 | D2 | 4 | 4 | 0 | 1.0 | +0.00% |
| benchpress/qiskit_gym/abstract_transpile/test_qasmbench.py::TestWorkoutAbstractQasmBenchMedium::test_QASMBench_medium[ising_n26-heavy-hex] | 2 | 3 | N2 | 50 | 50 | 0 | 1.0 | +0.00% |
| benchpress/qiskit_gym/abstract_transpile/test_qasmbench.py::TestWorkoutAbstractQasmBenchMedium::test_QASMBench_medium[ising_n26-heavy-hex] | 2 | 3 | runtime_s | 0.007162291090935469 | 0.007539624813944101 | 0.0003648758865892887 | 1.0509440180462746 | -5.09% |
| benchpress/qiskit_gym/abstract_transpile/test_qasmbench.py::TestWorkoutAbstractQasmBenchMedium::test_QASMBench_medium[ising_n26-heavy-hex] | 3 | 3 | D2 | 4 | 4 | 0 | 1.0 | +0.00% |
| benchpress/qiskit_gym/abstract_transpile/test_qasmbench.py::TestWorkoutAbstractQasmBenchMedium::test_QASMBench_medium[ising_n26-heavy-hex] | 3 | 3 | N2 | 50 | 50 | 0 | 1.0 | +0.00% |
| benchpress/qiskit_gym/abstract_transpile/test_qasmbench.py::TestWorkoutAbstractQasmBenchMedium::test_QASMBench_medium[ising_n26-heavy-hex] | 3 | 3 | runtime_s | 0.032191375037655234 | 0.033318083034828305 | 0.0014714580029249191 | 1.045497107959452 | -4.55% |
| benchpress/qiskit_gym/abstract_transpile/test_qasmbench.py::TestWorkoutAbstractQasmBenchMedium::test_QASMBench_medium[ising_n26-linear] | 2 | 3 | D2 | 4 | 4 | 0 | 1.0 | +0.00% |
| benchpress/qiskit_gym/abstract_transpile/test_qasmbench.py::TestWorkoutAbstractQasmBenchMedium::test_QASMBench_medium[ising_n26-linear] | 2 | 3 | N2 | 50 | 50 | 0 | 1.0 | +0.00% |
| benchpress/qiskit_gym/abstract_transpile/test_qasmbench.py::TestWorkoutAbstractQasmBenchMedium::test_QASMBench_medium[ising_n26-linear] | 2 | 3 | runtime_s | 0.003725250018760562 | 0.003925625002011657 | 0.00018412363715469837 | 1.052205262294136 | -5.22% |
| benchpress/qiskit_gym/abstract_transpile/test_qasmbench.py::TestWorkoutAbstractQasmBenchMedium::test_QASMBench_medium[ising_n26-linear] | 3 | 3 | D2 | 4 | 4 | 0 | 1.0 | +0.00% |
| benchpress/qiskit_gym/abstract_transpile/test_qasmbench.py::TestWorkoutAbstractQasmBenchMedium::test_QASMBench_medium[ising_n26-linear] | 3 | 3 | N2 | 50 | 50 | 0 | 1.0 | +0.00% |
| benchpress/qiskit_gym/abstract_transpile/test_qasmbench.py::TestWorkoutAbstractQasmBenchMedium::test_QASMBench_medium[ising_n26-linear] | 3 | 3 | runtime_s | 0.004310291958972812 | 0.004661625018343329 | 0.0003650409635156393 | 1.0849607406389443 | -8.50% |
| benchpress/qiskit_gym/abstract_transpile/test_qasmbench.py::TestWorkoutAbstractQasmBenchMedium::test_QASMBench_medium[ising_n26-square] | 2 | 3 | D2 | 4 | 4 | 0 | 1.0 | +0.00% |
| benchpress/qiskit_gym/abstract_transpile/test_qasmbench.py::TestWorkoutAbstractQasmBenchMedium::test_QASMBench_medium[ising_n26-square] | 2 | 3 | N2 | 50 | 50 | 0 | 1.0 | +0.00% |
| benchpress/qiskit_gym/abstract_transpile/test_qasmbench.py::TestWorkoutAbstractQasmBenchMedium::test_QASMBench_medium[ising_n26-square] | 2 | 3 | runtime_s | 0.007260166807100177 | 0.007135916966944933 | -0.00014358269982039928 | 0.9802232230146585 | +1.98% |
| benchpress/qiskit_gym/abstract_transpile/test_qasmbench.py::TestWorkoutAbstractQasmBenchMedium::test_QASMBench_medium[ising_n26-square] | 3 | 3 | D2 | 4 | 4 | 0 | 1.0 | +0.00% |
| benchpress/qiskit_gym/abstract_transpile/test_qasmbench.py::TestWorkoutAbstractQasmBenchMedium::test_QASMBench_medium[ising_n26-square] | 3 | 3 | N2 | 50 | 50 | 0 | 1.0 | +0.00% |
| benchpress/qiskit_gym/abstract_transpile/test_qasmbench.py::TestWorkoutAbstractQasmBenchMedium::test_QASMBench_medium[ising_n26-square] | 3 | 3 | runtime_s | 0.15945904213003814 | 0.16168870800174773 | 0.002352166222408414 | 1.01476225225012 | -1.48% |
| benchpress/qiskit_gym/abstract_transpile/test_qasmbench.py::TestWorkoutAbstractQasmBenchMedium::test_QASMBench_medium[qft_n18-all-to-all] | 2 | 3 | D2 | 66 | 66 | 0 | 1.0 | +0.00% |
| benchpress/qiskit_gym/abstract_transpile/test_qasmbench.py::TestWorkoutAbstractQasmBenchMedium::test_QASMBench_medium[qft_n18-all-to-all] | 2 | 3 | N2 | 294 | 294 | 0 | 1.0 | +0.00% |
| benchpress/qiskit_gym/abstract_transpile/test_qasmbench.py::TestWorkoutAbstractQasmBenchMedium::test_QASMBench_medium[qft_n18-all-to-all] | 2 | 3 | runtime_s | 0.015998875023797154 | 0.01611704216338694 | 2.512522041797638e-05 | 1.001561356580886 | -0.16% |
| benchpress/qiskit_gym/abstract_transpile/test_qasmbench.py::TestWorkoutAbstractQasmBenchMedium::test_QASMBench_medium[qft_n18-all-to-all] | 3 | 3 | D2 | 66 | 66 | 0 | 1.0 | +0.00% |
| benchpress/qiskit_gym/abstract_transpile/test_qasmbench.py::TestWorkoutAbstractQasmBenchMedium::test_QASMBench_medium[qft_n18-all-to-all] | 3 | 3 | N2 | 294 | 294 | 0 | 1.0 | +0.00% |
| benchpress/qiskit_gym/abstract_transpile/test_qasmbench.py::TestWorkoutAbstractQasmBenchMedium::test_QASMBench_medium[qft_n18-all-to-all] | 3 | 3 | runtime_s | 0.3476864171680063 | 0.34898062516003847 | 0.0010248341131955385 | 1.0029570466066546 | -0.30% |
| benchpress/qiskit_gym/abstract_transpile/test_qasmbench.py::TestWorkoutAbstractQasmBenchMedium::test_QASMBench_medium[qft_n18-heavy-hex] | 2 | 3 | D2 | 169 | 151 | -33 | 0.8122448979591836 | +18.78% |
| benchpress/qiskit_gym/abstract_transpile/test_qasmbench.py::TestWorkoutAbstractQasmBenchMedium::test_QASMBench_medium[qft_n18-heavy-hex] | 2 | 3 | N2 | 545 | 491 | -54 | 0.9009174311926605 | +9.91% |
| benchpress/qiskit_gym/abstract_transpile/test_qasmbench.py::TestWorkoutAbstractQasmBenchMedium::test_QASMBench_medium[qft_n18-heavy-hex] | 2 | 3 | runtime_s | 0.04755620798096061 | 0.0495132920332253 | 0.002551957033574581 | 1.0509713905261147 | -5.10% |
| benchpress/qiskit_gym/abstract_transpile/test_qasmbench.py::TestWorkoutAbstractQasmBenchMedium::test_QASMBench_medium[qft_n18-heavy-hex] | 3 | 3 | D2 | 213 | 159 | -35 | 0.832258064516129 | +16.77% |
| benchpress/qiskit_gym/abstract_transpile/test_qasmbench.py::TestWorkoutAbstractQasmBenchMedium::test_QASMBench_medium[qft_n18-heavy-hex] | 3 | 3 | N2 | 532 | 476 | -52 | 0.9022556390977443 | +9.77% |
| benchpress/qiskit_gym/abstract_transpile/test_qasmbench.py::TestWorkoutAbstractQasmBenchMedium::test_QASMBench_medium[qft_n18-heavy-hex] | 3 | 3 | runtime_s | 0.06868804199621081 | 0.06570054101757705 | 0.006470249034464359 | 1.0941976048002837 | -9.42% |
| benchpress/qiskit_gym/abstract_transpile/test_qasmbench.py::TestWorkoutAbstractQasmBenchMedium::test_QASMBench_medium[qft_n18-linear] | 2 | 3 | D2 | 145 | 111 | -38 | 0.7454545454545455 | +25.45% |
| benchpress/qiskit_gym/abstract_transpile/test_qasmbench.py::TestWorkoutAbstractQasmBenchMedium::test_QASMBench_medium[qft_n18-linear] | 2 | 3 | N2 | 513 | 459 | -50 | 0.9025341130604289 | +9.75% |
| benchpress/qiskit_gym/abstract_transpile/test_qasmbench.py::TestWorkoutAbstractQasmBenchMedium::test_QASMBench_medium[qft_n18-linear] | 2 | 3 | runtime_s | 0.03786124987527728 | 0.04165029199793935 | 0.0031874170526862144 | 1.0828699637565598 | -8.29% |
| benchpress/qiskit_gym/abstract_transpile/test_qasmbench.py::TestWorkoutAbstractQasmBenchMedium::test_QASMBench_medium[qft_n18-linear] | 3 | 3 | D2 | 157 | 117 | -40 | 0.7452229299363057 | +25.48% |
| benchpress/qiskit_gym/abstract_transpile/test_qasmbench.py::TestWorkoutAbstractQasmBenchMedium::test_QASMBench_medium[qft_n18-linear] | 3 | 3 | N2 | 526 | 462 | -64 | 0.8783269961977186 | +12.17% |
| benchpress/qiskit_gym/abstract_transpile/test_qasmbench.py::TestWorkoutAbstractQasmBenchMedium::test_QASMBench_medium[qft_n18-linear] | 3 | 3 | runtime_s | 0.04731458402238786 | 0.04815908404998481 | 0.0010249170009046793 | 1.0217446719666743 | -2.17% |
| benchpress/qiskit_gym/abstract_transpile/test_qasmbench.py::TestWorkoutAbstractQasmBenchMedium::test_QASMBench_medium[qft_n18-square] | 2 | 3 | D2 | 214 | 183 | -18 | 0.9227467811158798 | +7.73% |
| benchpress/qiskit_gym/abstract_transpile/test_qasmbench.py::TestWorkoutAbstractQasmBenchMedium::test_QASMBench_medium[qft_n18-square] | 2 | 3 | N2 | 526 | 460 | -56 | 0.895910780669145 | +10.41% |
| benchpress/qiskit_gym/abstract_transpile/test_qasmbench.py::TestWorkoutAbstractQasmBenchMedium::test_QASMBench_medium[qft_n18-square] | 2 | 3 | runtime_s | 0.0441958331502974 | 0.04685849999077618 | 0.002662666840478778 | 1.0602470108759758 | -6.02% |
| benchpress/qiskit_gym/abstract_transpile/test_qasmbench.py::TestWorkoutAbstractQasmBenchMedium::test_QASMBench_medium[qft_n18-square] | 3 | 3 | D2 | 217 | 192 | -16 | 0.9219512195121952 | +7.80% |
| benchpress/qiskit_gym/abstract_transpile/test_qasmbench.py::TestWorkoutAbstractQasmBenchMedium::test_QASMBench_medium[qft_n18-square] | 3 | 3 | N2 | 512 | 450 | -46 | 0.907070707070707 | +9.29% |
| benchpress/qiskit_gym/abstract_transpile/test_qasmbench.py::TestWorkoutAbstractQasmBenchMedium::test_QASMBench_medium[qft_n18-square] | 3 | 3 | runtime_s | 0.06124199996702373 | 0.060677999863401055 | -0.0008533340878784657 | 0.9873027492576004 | +1.27% |
| benchpress/qiskit_gym/abstract_transpile/test_qasmbench.py::TestWorkoutAbstractQasmBenchSmall::test_QASMBench_small[adder_n10-all-to-all] | 2 | 3 | D2 | 55 | 55 | 0 | 1.0 | +0.00% |
| benchpress/qiskit_gym/abstract_transpile/test_qasmbench.py::TestWorkoutAbstractQasmBenchSmall::test_QASMBench_small[adder_n10-all-to-all] | 2 | 3 | N2 | 65 | 65 | 0 | 1.0 | +0.00% |
| benchpress/qiskit_gym/abstract_transpile/test_qasmbench.py::TestWorkoutAbstractQasmBenchSmall::test_QASMBench_small[adder_n10-all-to-all] | 2 | 3 | runtime_s | 0.007070917170494795 | 0.006746707949787378 | -0.0001272088848054409 | 0.9814939738337733 | +1.85% |
| benchpress/qiskit_gym/abstract_transpile/test_qasmbench.py::TestWorkoutAbstractQasmBenchSmall::test_QASMBench_small[adder_n10-all-to-all] | 3 | 3 | D2 | 55 | 55 | 0 | 1.0 | +0.00% |
| benchpress/qiskit_gym/abstract_transpile/test_qasmbench.py::TestWorkoutAbstractQasmBenchSmall::test_QASMBench_small[adder_n10-all-to-all] | 3 | 3 | N2 | 65 | 65 | 0 | 1.0 | +0.00% |
| benchpress/qiskit_gym/abstract_transpile/test_qasmbench.py::TestWorkoutAbstractQasmBenchSmall::test_QASMBench_small[adder_n10-all-to-all] | 3 | 3 | runtime_s | 0.039461584063246846 | 0.038573124911636114 | -0.0005827920977026224 | 0.985116116740067 | +1.49% |
| benchpress/qiskit_gym/abstract_transpile/test_qasmbench.py::TestWorkoutAbstractQasmBenchSmall::test_QASMBench_small[adder_n10-heavy-hex] | 2 | 3 | D2 | 87 | 87 | 0 | 1.0 | +0.00% |
| benchpress/qiskit_gym/abstract_transpile/test_qasmbench.py::TestWorkoutAbstractQasmBenchSmall::test_QASMBench_small[adder_n10-heavy-hex] | 2 | 3 | N2 | 96 | 96 | 0 | 1.0 | +0.00% |
| benchpress/qiskit_gym/abstract_transpile/test_qasmbench.py::TestWorkoutAbstractQasmBenchSmall::test_QASMBench_small[adder_n10-heavy-hex] | 2 | 3 | runtime_s | 0.006999750155955553 | 0.007533167023211718 | 0.0003154156729578972 | 1.0416690556063966 | -4.17% |
| benchpress/qiskit_gym/abstract_transpile/test_qasmbench.py::TestWorkoutAbstractQasmBenchSmall::test_QASMBench_small[adder_n10-heavy-hex] | 3 | 3 | D2 | 87 | 87 | 0 | 1.0 | +0.00% |
| benchpress/qiskit_gym/abstract_transpile/test_qasmbench.py::TestWorkoutAbstractQasmBenchSmall::test_QASMBench_small[adder_n10-heavy-hex] | 3 | 3 | N2 | 96 | 96 | 0 | 1.0 | +0.00% |
| benchpress/qiskit_gym/abstract_transpile/test_qasmbench.py::TestWorkoutAbstractQasmBenchSmall::test_QASMBench_small[adder_n10-heavy-hex] | 3 | 3 | runtime_s | 0.00783962500281632 | 0.00879533402621746 | 0.0006264590192586184 | 1.0766885303943265 | -7.67% |
| benchpress/qiskit_gym/abstract_transpile/test_qasmbench.py::TestWorkoutAbstractQasmBenchSmall::test_QASMBench_small[adder_n10-linear] | 2 | 3 | D2 | 84 | 84 | 0 | 1.0 | +0.00% |
| benchpress/qiskit_gym/abstract_transpile/test_qasmbench.py::TestWorkoutAbstractQasmBenchSmall::test_QASMBench_small[adder_n10-linear] | 2 | 3 | N2 | 94 | 94 | 0 | 1.0 | +0.00% |
| benchpress/qiskit_gym/abstract_transpile/test_qasmbench.py::TestWorkoutAbstractQasmBenchSmall::test_QASMBench_small[adder_n10-linear] | 2 | 3 | runtime_s | 0.0064917500130832195 | 0.0076208331156522036 | 0.0011863340623676777 | 1.18274487772585 | -18.27% |
| benchpress/qiskit_gym/abstract_transpile/test_qasmbench.py::TestWorkoutAbstractQasmBenchSmall::test_QASMBench_small[adder_n10-linear] | 3 | 3 | D2 | 84 | 84 | 0 | 1.0 | +0.00% |
| benchpress/qiskit_gym/abstract_transpile/test_qasmbench.py::TestWorkoutAbstractQasmBenchSmall::test_QASMBench_small[adder_n10-linear] | 3 | 3 | N2 | 94 | 94 | 0 | 1.0 | +0.00% |
| benchpress/qiskit_gym/abstract_transpile/test_qasmbench.py::TestWorkoutAbstractQasmBenchSmall::test_QASMBench_small[adder_n10-linear] | 3 | 3 | runtime_s | 0.0073659580666571856 | 0.008085333043709397 | 0.000899334205314517 | 1.1202747322893736 | -12.03% |
| benchpress/qiskit_gym/abstract_transpile/test_qasmbench.py::TestWorkoutAbstractQasmBenchSmall::test_QASMBench_small[adder_n10-square] | 2 | 3 | D2 | 79 | 79 | 0 | 1.0 | +0.00% |
| benchpress/qiskit_gym/abstract_transpile/test_qasmbench.py::TestWorkoutAbstractQasmBenchSmall::test_QASMBench_small[adder_n10-square] | 2 | 3 | N2 | 91 | 91 | 0 | 1.0 | +0.00% |
| benchpress/qiskit_gym/abstract_transpile/test_qasmbench.py::TestWorkoutAbstractQasmBenchSmall::test_QASMBench_small[adder_n10-square] | 2 | 3 | runtime_s | 0.007244249805808067 | 0.007972917053848505 | 0.0006051249802112579 | 1.0821311152870967 | -8.21% |
| benchpress/qiskit_gym/abstract_transpile/test_qasmbench.py::TestWorkoutAbstractQasmBenchSmall::test_QASMBench_small[adder_n10-square] | 3 | 3 | D2 | 79 | 79 | 0 | 1.0 | +0.00% |
| benchpress/qiskit_gym/abstract_transpile/test_qasmbench.py::TestWorkoutAbstractQasmBenchSmall::test_QASMBench_small[adder_n10-square] | 3 | 3 | N2 | 90 | 90 | 0 | 1.0 | +0.00% |
| benchpress/qiskit_gym/abstract_transpile/test_qasmbench.py::TestWorkoutAbstractQasmBenchSmall::test_QASMBench_small[adder_n10-square] | 3 | 3 | runtime_s | 0.00934620900079608 | 0.009445250034332275 | 0.0003182082436978817 | 1.03203425315117 | -3.20% |
| benchpress/qiskit_gym/abstract_transpile/test_qasmbench.py::TestWorkoutAbstractQasmBenchSmall::test_QASMBench_small[qaoa_n6-all-to-all] | 2 | 3 | D2 | 22 | 22 | 0 | 1.0 | +0.00% |
| benchpress/qiskit_gym/abstract_transpile/test_qasmbench.py::TestWorkoutAbstractQasmBenchSmall::test_QASMBench_small[qaoa_n6-all-to-all] | 2 | 3 | N2 | 36 | 36 | 0 | 1.0 | +0.00% |
| benchpress/qiskit_gym/abstract_transpile/test_qasmbench.py::TestWorkoutAbstractQasmBenchSmall::test_QASMBench_small[qaoa_n6-all-to-all] | 2 | 3 | runtime_s | 0.002827208023518324 | 0.0031007088255137205 | 0.0002735008019953966 | 1.0967388319926448 | -9.67% |
| benchpress/qiskit_gym/abstract_transpile/test_qasmbench.py::TestWorkoutAbstractQasmBenchSmall::test_QASMBench_small[qaoa_n6-all-to-all] | 3 | 3 | D2 | 22 | 22 | 0 | 1.0 | +0.00% |
| benchpress/qiskit_gym/abstract_transpile/test_qasmbench.py::TestWorkoutAbstractQasmBenchSmall::test_QASMBench_small[qaoa_n6-all-to-all] | 3 | 3 | N2 | 36 | 36 | 0 | 1.0 | +0.00% |
| benchpress/qiskit_gym/abstract_transpile/test_qasmbench.py::TestWorkoutAbstractQasmBenchSmall::test_QASMBench_small[qaoa_n6-all-to-all] | 3 | 3 | runtime_s | 0.005258040968328714 | 0.005249291891232133 | -8.879206143319607e-05 | 0.983366304797649 | +1.66% |
| benchpress/qiskit_gym/abstract_transpile/test_qasmbench.py::TestWorkoutAbstractQasmBenchSmall::test_QASMBench_small[qaoa_n6-heavy-hex] | 2 | 3 | D2 | 48 | 48 | 0 | 1.0 | +0.00% |
| benchpress/qiskit_gym/abstract_transpile/test_qasmbench.py::TestWorkoutAbstractQasmBenchSmall::test_QASMBench_small[qaoa_n6-heavy-hex] | 2 | 3 | N2 | 63 | 63 | 0 | 1.0 | +0.00% |
| benchpress/qiskit_gym/abstract_transpile/test_qasmbench.py::TestWorkoutAbstractQasmBenchSmall::test_QASMBench_small[qaoa_n6-heavy-hex] | 2 | 3 | runtime_s | 0.005455042002722621 | 0.0059037909377366304 | 4.954100586473942e-05 | 1.0090816910007316 | -0.91% |
| benchpress/qiskit_gym/abstract_transpile/test_qasmbench.py::TestWorkoutAbstractQasmBenchSmall::test_QASMBench_small[qaoa_n6-heavy-hex] | 3 | 3 | D2 | 48 | 48 | 0 | 1.0 | +0.00% |
| benchpress/qiskit_gym/abstract_transpile/test_qasmbench.py::TestWorkoutAbstractQasmBenchSmall::test_QASMBench_small[qaoa_n6-heavy-hex] | 3 | 3 | N2 | 60 | 60 | 0 | 1.0 | +0.00% |
| benchpress/qiskit_gym/abstract_transpile/test_qasmbench.py::TestWorkoutAbstractQasmBenchSmall::test_QASMBench_small[qaoa_n6-heavy-hex] | 3 | 3 | runtime_s | 0.006955625023692846 | 0.006982000079005957 | 2.637505531311035e-05 | 1.0037919029883395 | -0.38% |
| benchpress/qiskit_gym/abstract_transpile/test_qasmbench.py::TestWorkoutAbstractQasmBenchSmall::test_QASMBench_small[qaoa_n6-linear] | 2 | 3 | D2 | 49 | 49 | 0 | 1.0 | +0.00% |
| benchpress/qiskit_gym/abstract_transpile/test_qasmbench.py::TestWorkoutAbstractQasmBenchSmall::test_QASMBench_small[qaoa_n6-linear] | 2 | 3 | N2 | 72 | 72 | 0 | 1.0 | +0.00% |
| benchpress/qiskit_gym/abstract_transpile/test_qasmbench.py::TestWorkoutAbstractQasmBenchSmall::test_QASMBench_small[qaoa_n6-linear] | 2 | 3 | runtime_s | 0.005162958055734634 | 0.005249499808996916 | 0.00021758396178483963 | 1.0463758639620944 | -4.64% |
| benchpress/qiskit_gym/abstract_transpile/test_qasmbench.py::TestWorkoutAbstractQasmBenchSmall::test_QASMBench_small[qaoa_n6-linear] | 3 | 3 | D2 | 53 | 53 | 0 | 1.0 | +0.00% |
| benchpress/qiskit_gym/abstract_transpile/test_qasmbench.py::TestWorkoutAbstractQasmBenchSmall::test_QASMBench_small[qaoa_n6-linear] | 3 | 3 | N2 | 72 | 72 | 0 | 1.0 | +0.00% |
| benchpress/qiskit_gym/abstract_transpile/test_qasmbench.py::TestWorkoutAbstractQasmBenchSmall::test_QASMBench_small[qaoa_n6-linear] | 3 | 3 | runtime_s | 0.006315083941444755 | 0.007122958078980446 | 0.0001785841304808855 | 1.0295255637968677 | -2.95% |
| benchpress/qiskit_gym/abstract_transpile/test_qasmbench.py::TestWorkoutAbstractQasmBenchSmall::test_QASMBench_small[qaoa_n6-square] | 2 | 3 | D2 | 40 | 40 | 0 | 1.0 | +0.00% |
| benchpress/qiskit_gym/abstract_transpile/test_qasmbench.py::TestWorkoutAbstractQasmBenchSmall::test_QASMBench_small[qaoa_n6-square] | 2 | 3 | N2 | 54 | 54 | 0 | 1.0 | +0.00% |
| benchpress/qiskit_gym/abstract_transpile/test_qasmbench.py::TestWorkoutAbstractQasmBenchSmall::test_QASMBench_small[qaoa_n6-square] | 2 | 3 | runtime_s | 0.004674084018915892 | 0.005211582873016596 | 0.00025479099713265896 | 1.0545114285711439 | -5.45% |
| benchpress/qiskit_gym/abstract_transpile/test_qasmbench.py::TestWorkoutAbstractQasmBenchSmall::test_QASMBench_small[qaoa_n6-square] | 3 | 3 | D2 | 45 | 45 | 0 | 1.0 | +0.00% |
| benchpress/qiskit_gym/abstract_transpile/test_qasmbench.py::TestWorkoutAbstractQasmBenchSmall::test_QASMBench_small[qaoa_n6-square] | 3 | 3 | N2 | 54 | 54 | 0 | 1.0 | +0.00% |
| benchpress/qiskit_gym/abstract_transpile/test_qasmbench.py::TestWorkoutAbstractQasmBenchSmall::test_QASMBench_small[qaoa_n6-square] | 3 | 3 | runtime_s | 0.005806416971608996 | 0.006019458873197436 | 0.00021304190158843994 | 1.0366907686151594 | -3.67% |
| benchpress/qiskit_gym/device_transpile/test_feynman.py::TestWorkoutDeviceFeynman::test_feynman_transpile[adder_8.qasm] | 2 | 3 | D2 | 307 | 300 | -6 | 0.9774436090225563 | +2.26% |
| benchpress/qiskit_gym/device_transpile/test_feynman.py::TestWorkoutDeviceFeynman::test_feynman_transpile[adder_8.qasm] | 2 | 3 | N2 | 755 | 743 | -12 | 0.9841059602649007 | +1.59% |
| benchpress/qiskit_gym/device_transpile/test_feynman.py::TestWorkoutDeviceFeynman::test_feynman_transpile[adder_8.qasm] | 2 | 3 | runtime_s | 0.05960908415727317 | 0.061717832926660776 | 0.002108748769387603 | 1.0353762987504365 | -3.54% |
| benchpress/qiskit_gym/device_transpile/test_feynman.py::TestWorkoutDeviceFeynman::test_feynman_transpile[adder_8.qasm] | 3 | 3 | D2 | 279 | 276 | -3 | 0.989247311827957 | +1.08% |
| benchpress/qiskit_gym/device_transpile/test_feynman.py::TestWorkoutDeviceFeynman::test_feynman_transpile[adder_8.qasm] | 3 | 3 | N2 | 752 | 742 | -8 | 0.9890260631001372 | +1.10% |
| benchpress/qiskit_gym/device_transpile/test_feynman.py::TestWorkoutDeviceFeynman::test_feynman_transpile[adder_8.qasm] | 3 | 3 | runtime_s | 0.08474641595967114 | 0.09065904188901186 | 0.003670876147225499 | 1.040184815109383 | -4.02% |
| benchpress/qiskit_gym/device_transpile/test_feynman.py::TestWorkoutDeviceFeynman::test_feynman_transpile[barenco_tof_5.qasm] | 2 | 3 | D2 | 92 | 92 | 0 | 1.0 | +0.00% |
| benchpress/qiskit_gym/device_transpile/test_feynman.py::TestWorkoutDeviceFeynman::test_feynman_transpile[barenco_tof_5.qasm] | 2 | 3 | N2 | 117 | 117 | 0 | 1.0 | +0.00% |
| benchpress/qiskit_gym/device_transpile/test_feynman.py::TestWorkoutDeviceFeynman::test_feynman_transpile[barenco_tof_5.qasm] | 2 | 3 | runtime_s | 0.0103964579757303 | 0.011645708000287414 | 0.0011919999960809946 | 1.1140265249040198 | -11.40% |
| benchpress/qiskit_gym/device_transpile/test_feynman.py::TestWorkoutDeviceFeynman::test_feynman_transpile[barenco_tof_5.qasm] | 3 | 3 | D2 | 92 | 92 | 0 | 1.0 | +0.00% |
| benchpress/qiskit_gym/device_transpile/test_feynman.py::TestWorkoutDeviceFeynman::test_feynman_transpile[barenco_tof_5.qasm] | 3 | 3 | N2 | 117 | 117 | 0 | 1.0 | +0.00% |
| benchpress/qiskit_gym/device_transpile/test_feynman.py::TestWorkoutDeviceFeynman::test_feynman_transpile[barenco_tof_5.qasm] | 3 | 3 | runtime_s | 0.01293249987065792 | 0.014125666813924909 | 0.001110791927203536 | 1.085347875939771 | -8.53% |
| benchpress/qiskit_gym/device_transpile/test_feynman.py::TestWorkoutDeviceFeynman::test_feynman_transpile[gf2^8_mult.qasm] | 2 | 3 | D2 | 487 | 483 | -2 | 0.9966887417218543 | +0.33% |
| benchpress/qiskit_gym/device_transpile/test_feynman.py::TestWorkoutDeviceFeynman::test_feynman_transpile[gf2^8_mult.qasm] | 2 | 3 | N2 | 1139 | 1133 | -6 | 0.9947322212467077 | +0.53% |
| benchpress/qiskit_gym/device_transpile/test_feynman.py::TestWorkoutDeviceFeynman::test_feynman_transpile[gf2^8_mult.qasm] | 2 | 3 | runtime_s | 0.08587887487374246 | 0.091796041931957 | 0.005642166826874018 | 1.0654894143762215 | -6.55% |
| benchpress/qiskit_gym/device_transpile/test_feynman.py::TestWorkoutDeviceFeynman::test_feynman_transpile[gf2^8_mult.qasm] | 3 | 3 | D2 | 533 | 525 | -4 | 0.9921875 | +0.78% |
| benchpress/qiskit_gym/device_transpile/test_feynman.py::TestWorkoutDeviceFeynman::test_feynman_transpile[gf2^8_mult.qasm] | 3 | 3 | N2 | 1161 | 1152 | -6 | 0.9948320413436692 | +0.52% |
| benchpress/qiskit_gym/device_transpile/test_feynman.py::TestWorkoutDeviceFeynman::test_feynman_transpile[gf2^8_mult.qasm] | 3 | 3 | runtime_s | 0.1132422499358654 | 0.11795274983160198 | 0.0040619587525725365 | 1.036782040692432 | -3.68% |
| benchpress/qiskit_gym/device_transpile/test_feynman.py::TestWorkoutDeviceFeynman::test_feynman_transpile[qft_4.qasm] | 2 | 3 | D2 | 75 | 75 | 0 | 1.0 | +0.00% |
| benchpress/qiskit_gym/device_transpile/test_feynman.py::TestWorkoutDeviceFeynman::test_feynman_transpile[qft_4.qasm] | 2 | 3 | N2 | 78 | 78 | 0 | 1.0 | +0.00% |
| benchpress/qiskit_gym/device_transpile/test_feynman.py::TestWorkoutDeviceFeynman::test_feynman_transpile[qft_4.qasm] | 2 | 3 | runtime_s | 0.008572291815653443 | 0.00858766702003777 | 0.000524790957570076 | 1.0665911441542455 | -6.66% |
| benchpress/qiskit_gym/device_transpile/test_feynman.py::TestWorkoutDeviceFeynman::test_feynman_transpile[qft_4.qasm] | 3 | 3 | D2 | 75 | 75 | 0 | 1.0 | +0.00% |
| benchpress/qiskit_gym/device_transpile/test_feynman.py::TestWorkoutDeviceFeynman::test_feynman_transpile[qft_4.qasm] | 3 | 3 | N2 | 78 | 78 | 0 | 1.0 | +0.00% |
| benchpress/qiskit_gym/device_transpile/test_feynman.py::TestWorkoutDeviceFeynman::test_feynman_transpile[qft_4.qasm] | 3 | 3 | runtime_s | 0.00961166713386774 | 0.010110832983627915 | 0.0005485410802066326 | 1.057365021455826 | -5.74% |
| benchpress/qiskit_gym/device_transpile/test_feynman.py::TestWorkoutDeviceFeynman::test_feynman_transpile[rc_adder_6.qasm] | 2 | 3 | D2 | 97 | 95 | -2 | 0.979381443298969 | +2.06% |
| benchpress/qiskit_gym/device_transpile/test_feynman.py::TestWorkoutDeviceFeynman::test_feynman_transpile[rc_adder_6.qasm] | 2 | 3 | N2 | 154 | 142 | -12 | 0.922077922077922 | +7.79% |
| benchpress/qiskit_gym/device_transpile/test_feynman.py::TestWorkoutDeviceFeynman::test_feynman_transpile[rc_adder_6.qasm] | 2 | 3 | runtime_s | 0.015421833144500852 | 0.01676658308133483 | 0.0010131248272955418 | 1.0656941893873884 | -6.57% |
| benchpress/qiskit_gym/device_transpile/test_feynman.py::TestWorkoutDeviceFeynman::test_feynman_transpile[rc_adder_6.qasm] | 3 | 3 | D2 | 88 | 86 | -2 | 0.9772727272727273 | +2.27% |
| benchpress/qiskit_gym/device_transpile/test_feynman.py::TestWorkoutDeviceFeynman::test_feynman_transpile[rc_adder_6.qasm] | 3 | 3 | N2 | 152 | 142 | -10 | 0.9342105263157895 | +6.58% |
| benchpress/qiskit_gym/device_transpile/test_feynman.py::TestWorkoutDeviceFeynman::test_feynman_transpile[rc_adder_6.qasm] | 3 | 3 | runtime_s | 0.018026583129540086 | 0.019623500062152743 | 0.0020165001042187214 | 1.1145283187957329 | -11.45% |
| benchpress/qiskit_gym/device_transpile/test_hamiltonians.py::TestWorkoutDeviceHamlibHamiltonians::test_hamlib_hamiltonians_transpile[ham_bh_graph-1D-grid-pbc-qubitnodes_Lx-14_U-10_enc-stdbinary_d-4] | 2 | 3 | D2 | 961 | 961 | 0 | 1.0 | +0.00% |
| benchpress/qiskit_gym/device_transpile/test_hamiltonians.py::TestWorkoutDeviceHamlibHamiltonians::test_hamlib_hamiltonians_transpile[ham_bh_graph-1D-grid-pbc-qubitnodes_Lx-14_U-10_enc-stdbinary_d-4] | 2 | 3 | N2 | 1066 | 1066 | 0 | 1.0 | +0.00% |
| benchpress/qiskit_gym/device_transpile/test_hamiltonians.py::TestWorkoutDeviceHamlibHamiltonians::test_hamlib_hamiltonians_transpile[ham_bh_graph-1D-grid-pbc-qubitnodes_Lx-14_U-10_enc-stdbinary_d-4] | 2 | 3 | runtime_s | 0.05777787487022579 | 0.06047074985690415 | 0.004516832996159792 | 1.0654595441828905 | -6.55% |
| benchpress/qiskit_gym/device_transpile/test_hamiltonians.py::TestWorkoutDeviceHamlibHamiltonians::test_hamlib_hamiltonians_transpile[ham_bh_graph-1D-grid-pbc-qubitnodes_Lx-14_U-10_enc-stdbinary_d-4] | 3 | 3 | D2 | 961 | 961 | 0 | 1.0 | +0.00% |
| benchpress/qiskit_gym/device_transpile/test_hamiltonians.py::TestWorkoutDeviceHamlibHamiltonians::test_hamlib_hamiltonians_transpile[ham_bh_graph-1D-grid-pbc-qubitnodes_Lx-14_U-10_enc-stdbinary_d-4] | 3 | 3 | N2 | 1030 | 1030 | 0 | 1.0 | +0.00% |
| benchpress/qiskit_gym/device_transpile/test_hamiltonians.py::TestWorkoutDeviceHamlibHamiltonians::test_hamlib_hamiltonians_transpile[ham_bh_graph-1D-grid-pbc-qubitnodes_Lx-14_U-10_enc-stdbinary_d-4] | 3 | 3 | runtime_s | 0.08478887495584786 | 0.08599116699770093 | 0.0012022920418530703 | 1.0141798324659825 | -1.42% |
| benchpress/qiskit_gym/device_transpile/test_hamiltonians.py::TestWorkoutDeviceHamlibHamiltonians::test_hamlib_hamiltonians_transpile[ham_complbipart-n-10_a-5_b-5] | 2 | 3 | D2 | 222 | 208 | -18 | 0.9243697478991597 | +7.56% |
| benchpress/qiskit_gym/device_transpile/test_hamiltonians.py::TestWorkoutDeviceHamlibHamiltonians::test_hamlib_hamiltonians_transpile[ham_complbipart-n-10_a-5_b-5] | 2 | 3 | N2 | 277 | 259 | -18 | 0.9350180505415162 | +6.50% |
| benchpress/qiskit_gym/device_transpile/test_hamiltonians.py::TestWorkoutDeviceHamlibHamiltonians::test_hamlib_hamiltonians_transpile[ham_complbipart-n-10_a-5_b-5] | 2 | 3 | runtime_s | 0.01683941693045199 | 0.01676316699013114 | -7.624994032084942e-05 | 0.9954719370251496 | +0.45% |
| benchpress/qiskit_gym/device_transpile/test_hamiltonians.py::TestWorkoutDeviceHamlibHamiltonians::test_hamlib_hamiltonians_transpile[ham_complbipart-n-10_a-5_b-5] | 3 | 3 | D2 | 229 | 209 | -16 | 0.9272727272727272 | +7.27% |
| benchpress/qiskit_gym/device_transpile/test_hamiltonians.py::TestWorkoutDeviceHamlibHamiltonians::test_hamlib_hamiltonians_transpile[ham_complbipart-n-10_a-5_b-5] | 3 | 3 | N2 | 288 | 266 | -18 | 0.9379310344827586 | +6.21% |
| benchpress/qiskit_gym/device_transpile/test_hamiltonians.py::TestWorkoutDeviceHamlibHamiltonians::test_hamlib_hamiltonians_transpile[ham_complbipart-n-10_a-5_b-5] | 3 | 3 | runtime_s | 0.021976625081151724 | 0.02125500002875924 | -0.0007216250523924828 | 0.9671639730974259 | +3.28% |
| benchpress/qiskit_gym/device_transpile/test_hamiltonians.py::TestWorkoutDeviceHamlibHamiltonians::test_hamlib_hamiltonians_transpile[ham_ham_JW14] | 2 | 3 | D2 | 5394 | 5370 | -24 | 0.9955506117908788 | +0.44% |
| benchpress/qiskit_gym/device_transpile/test_hamiltonians.py::TestWorkoutDeviceHamlibHamiltonians::test_hamlib_hamiltonians_transpile[ham_ham_JW14] | 2 | 3 | N2 | 6275 | 6259 | -16 | 0.9974501992031872 | +0.25% |
| benchpress/qiskit_gym/device_transpile/test_hamiltonians.py::TestWorkoutDeviceHamlibHamiltonians::test_hamlib_hamiltonians_transpile[ham_ham_JW14] | 2 | 3 | runtime_s | 0.40519541688263416 | 0.45161254215054214 | 0.042323625879362226 | 1.1079207822015573 | -10.79% |
| benchpress/qiskit_gym/device_transpile/test_hamiltonians.py::TestWorkoutDeviceHamlibHamiltonians::test_hamlib_hamiltonians_transpile[ham_ham_JW14] | 3 | 3 | D2 | 4975 | 4938 | -28 | 0.9943718592964824 | +0.56% |
| benchpress/qiskit_gym/device_transpile/test_hamiltonians.py::TestWorkoutDeviceHamlibHamiltonians::test_hamlib_hamiltonians_transpile[ham_ham_JW14] | 3 | 3 | N2 | 5832 | 5810 | -22 | 0.9962186318322448 | +0.38% |
| benchpress/qiskit_gym/device_transpile/test_hamiltonians.py::TestWorkoutDeviceHamlibHamiltonians::test_hamlib_hamiltonians_transpile[ham_ham_JW14] | 3 | 3 | runtime_s | 0.5066018339712173 | 0.5606529170181602 | 0.05797266704030335 | 1.115327123042644 | -11.53% |
| benchpress/qiskit_gym/device_transpile/test_hamiltonians.py::TestWorkoutDeviceHamlibHamiltonians::test_hamlib_hamiltonians_transpile[ham_tsp_prob-ts225_Ncity-5_enc-unary] | 2 | 3 | D2 | 153 | 138 | -15 | 0.9019607843137255 | +9.80% |
| benchpress/qiskit_gym/device_transpile/test_hamiltonians.py::TestWorkoutDeviceHamlibHamiltonians::test_hamlib_hamiltonians_transpile[ham_tsp_prob-ts225_Ncity-5_enc-unary] | 2 | 3 | N2 | 473 | 450 | -24 | 0.9493670886075949 | +5.06% |
| benchpress/qiskit_gym/device_transpile/test_hamiltonians.py::TestWorkoutDeviceHamlibHamiltonians::test_hamlib_hamiltonians_transpile[ham_tsp_prob-ts225_Ncity-5_enc-unary] | 2 | 3 | runtime_s | 0.05369708314538002 | 0.053458709036931396 | -0.0007676249369978905 | 0.9860195325922209 | +1.40% |
| benchpress/qiskit_gym/device_transpile/test_hamiltonians.py::TestWorkoutDeviceHamlibHamiltonians::test_hamlib_hamiltonians_transpile[ham_tsp_prob-ts225_Ncity-5_enc-unary] | 3 | 3 | D2 | 167 | 149 | -16 | 0.9064327485380117 | +9.36% |
| benchpress/qiskit_gym/device_transpile/test_hamiltonians.py::TestWorkoutDeviceHamlibHamiltonians::test_hamlib_hamiltonians_transpile[ham_tsp_prob-ts225_Ncity-5_enc-unary] | 3 | 3 | N2 | 509 | 471 | -38 | 0.925343811394892 | +7.47% |
| benchpress/qiskit_gym/device_transpile/test_hamiltonians.py::TestWorkoutDeviceHamlibHamiltonians::test_hamlib_hamiltonians_transpile[ham_tsp_prob-ts225_Ncity-5_enc-unary] | 3 | 3 | runtime_s | 0.06691991700790823 | 0.07206708309240639 | 0.004576625069603324 | 1.0663355108758898 | -6.63% |
| benchpress/qiskit_gym/device_transpile/test_summit.py::TestWorkoutDeviceTranspile100Q::test_BV_100_transpile | 2 | 3 | D2 | 196 | 196 | 0 | 1.0 | +0.00% |
| benchpress/qiskit_gym/device_transpile/test_summit.py::TestWorkoutDeviceTranspile100Q::test_BV_100_transpile | 2 | 3 | N2 | 196 | 196 | 0 | 1.0 | +0.00% |
| benchpress/qiskit_gym/device_transpile/test_summit.py::TestWorkoutDeviceTranspile100Q::test_BV_100_transpile | 2 | 3 | runtime_s | 0.061060083797201514 | 0.05869900016114116 | -0.0021914588287472725 | 0.9641097965730648 | +3.59% |
| benchpress/qiskit_gym/device_transpile/test_summit.py::TestWorkoutDeviceTranspile100Q::test_BV_100_transpile | 3 | 3 | D2 | 196 | 196 | 0 | 1.0 | +0.00% |
| benchpress/qiskit_gym/device_transpile/test_summit.py::TestWorkoutDeviceTranspile100Q::test_BV_100_transpile | 3 | 3 | N2 | 196 | 196 | 0 | 1.0 | +0.00% |
| benchpress/qiskit_gym/device_transpile/test_summit.py::TestWorkoutDeviceTranspile100Q::test_BV_100_transpile | 3 | 3 | runtime_s | 15.169834875036031 | 14.895481124985963 | 0.08192649972625077 | 1.0055909813243056 | -0.56% |
| benchpress/qiskit_gym/device_transpile/test_summit.py::TestWorkoutDeviceTranspile100Q::test_BVlike_simplification_transpile | 2 | 3 | D2 | 0 | 0 | 0 | unavailable | unavailable |
| benchpress/qiskit_gym/device_transpile/test_summit.py::TestWorkoutDeviceTranspile100Q::test_BVlike_simplification_transpile | 2 | 3 | N2 | 0 | 0 | 0 | unavailable | unavailable |
| benchpress/qiskit_gym/device_transpile/test_summit.py::TestWorkoutDeviceTranspile100Q::test_BVlike_simplification_transpile | 2 | 3 | runtime_s | 0.00522537506185472 | 0.005132042104378343 | 0.00011270889081060886 | 1.0215695312731492 | -2.16% |
| benchpress/qiskit_gym/device_transpile/test_summit.py::TestWorkoutDeviceTranspile100Q::test_BVlike_simplification_transpile | 3 | 3 | D2 | 0 | 0 | 0 | unavailable | unavailable |
| benchpress/qiskit_gym/device_transpile/test_summit.py::TestWorkoutDeviceTranspile100Q::test_BVlike_simplification_transpile | 3 | 3 | N2 | 0 | 0 | 0 | unavailable | unavailable |
| benchpress/qiskit_gym/device_transpile/test_summit.py::TestWorkoutDeviceTranspile100Q::test_BVlike_simplification_transpile | 3 | 3 | runtime_s | 0.005532125011086464 | 0.005475458921864629 | -1.6584061086177826e-05 | 0.9970022258981959 | +0.30% |
| benchpress/qiskit_gym/device_transpile/test_summit.py::TestWorkoutDeviceTranspile100Q::test_QAOA_100_transpile | 2 | 3 | D2 | 1552 | 1532 | -24 | 0.9842001316655694 | +1.58% |
| benchpress/qiskit_gym/device_transpile/test_summit.py::TestWorkoutDeviceTranspile100Q::test_QAOA_100_transpile | 2 | 3 | N2 | 8743 | 8665 | -78 | 0.9910785771474322 | +0.89% |
| benchpress/qiskit_gym/device_transpile/test_summit.py::TestWorkoutDeviceTranspile100Q::test_QAOA_100_transpile | 2 | 3 | runtime_s | 0.7534398750867695 | 0.7714447500184178 | 0.018004874931648374 | 1.0238968967889772 | -2.39% |
| benchpress/qiskit_gym/device_transpile/test_summit.py::TestWorkoutDeviceTranspile100Q::test_QAOA_100_transpile | 3 | 3 | D2 | 1499 | 1475 | -23 | 0.9839893262174784 | +1.60% |
| benchpress/qiskit_gym/device_transpile/test_summit.py::TestWorkoutDeviceTranspile100Q::test_QAOA_100_transpile | 3 | 3 | N2 | 8455 | 8363 | -92 | 0.9891188645771732 | +1.09% |
| benchpress/qiskit_gym/device_transpile/test_summit.py::TestWorkoutDeviceTranspile100Q::test_QAOA_100_transpile | 3 | 3 | runtime_s | 1.0147661659866571 | 1.0292155421338975 | 0.02581070689484477 | 1.0268756768458753 | -2.69% |
| benchpress/qiskit_gym/device_transpile/test_summit.py::TestWorkoutDeviceTranspile100Q::test_QFT_100_transpile | 2 | 3 | D2 | 1879 | 1730 | -93 | 0.9524053224155579 | +4.76% |
| benchpress/qiskit_gym/device_transpile/test_summit.py::TestWorkoutDeviceTranspile100Q::test_QFT_100_transpile | 2 | 3 | N2 | 9774 | 9088 | -686 | 0.9298137916922448 | +7.02% |
| benchpress/qiskit_gym/device_transpile/test_summit.py::TestWorkoutDeviceTranspile100Q::test_QFT_100_transpile | 2 | 3 | runtime_s | 0.89914166694507 | 0.9263425408862531 | 0.03567929193377495 | 1.0396203660753038 | -3.96% |
| benchpress/qiskit_gym/device_transpile/test_summit.py::TestWorkoutDeviceTranspile100Q::test_QFT_100_transpile | 3 | 3 | D2 | 1755 | 1677 | -78 | 0.9555555555555556 | +4.44% |
| benchpress/qiskit_gym/device_transpile/test_summit.py::TestWorkoutDeviceTranspile100Q::test_QFT_100_transpile | 3 | 3 | N2 | 9099 | 8718 | -494 | 0.9457083195955599 | +5.43% |
| benchpress/qiskit_gym/device_transpile/test_summit.py::TestWorkoutDeviceTranspile100Q::test_QFT_100_transpile | 3 | 3 | runtime_s | 1.2421731250360608 | 1.2224892920348793 | -0.019683833001181483 | 0.9841537120676234 | +1.58% |
| benchpress/qiskit_gym/device_transpile/test_summit.py::TestWorkoutDeviceTranspile100Q::test_QV_100_transpile | 2 | 3 | D2 | 10395 | 10395 | 0 | 1.0 | +0.00% |
| benchpress/qiskit_gym/device_transpile/test_summit.py::TestWorkoutDeviceTranspile100Q::test_QV_100_transpile | 2 | 3 | N2 | 95718 | 95718 | 0 | 1.0 | +0.00% |
| benchpress/qiskit_gym/device_transpile/test_summit.py::TestWorkoutDeviceTranspile100Q::test_QV_100_transpile | 2 | 3 | runtime_s | 16.236916417023167 | 16.454631624976173 | 0.22038304223679006 | 1.0135778152810115 | -1.36% |
| benchpress/qiskit_gym/device_transpile/test_summit.py::TestWorkoutDeviceTranspile100Q::test_QV_100_transpile | 3 | 3 | D2 | 10404 | 10404 | 0 | 1.0 | +0.00% |
| benchpress/qiskit_gym/device_transpile/test_summit.py::TestWorkoutDeviceTranspile100Q::test_QV_100_transpile | 3 | 3 | N2 | 95730 | 95730 | 0 | 1.0 | +0.00% |
| benchpress/qiskit_gym/device_transpile/test_summit.py::TestWorkoutDeviceTranspile100Q::test_QV_100_transpile | 3 | 3 | runtime_s | 20.311147917062044 | 20.547748625045642 | 0.2366007079835981 | 1.0116488102469505 | -1.16% |
| benchpress/qiskit_gym/device_transpile/test_summit.py::TestWorkoutDeviceTranspile100Q::test_circSU2_100_transpile | 2 | 3 | D2 | 300 | 300 | 0 | 1.0 | +0.00% |
| benchpress/qiskit_gym/device_transpile/test_summit.py::TestWorkoutDeviceTranspile100Q::test_circSU2_100_transpile | 2 | 3 | N2 | 300 | 300 | 0 | 1.0 | +0.00% |
| benchpress/qiskit_gym/device_transpile/test_summit.py::TestWorkoutDeviceTranspile100Q::test_circSU2_100_transpile | 2 | 3 | runtime_s | 0.07104895799420774 | 0.06814737501554191 | -0.0029015829786658287 | 0.9591607947451899 | +4.08% |
| benchpress/qiskit_gym/device_transpile/test_summit.py::TestWorkoutDeviceTranspile100Q::test_circSU2_100_transpile | 3 | 3 | D2 | 300 | 300 | 0 | 1.0 | +0.00% |
| benchpress/qiskit_gym/device_transpile/test_summit.py::TestWorkoutDeviceTranspile100Q::test_circSU2_100_transpile | 3 | 3 | N2 | 300 | 300 | 0 | 1.0 | +0.00% |
| benchpress/qiskit_gym/device_transpile/test_summit.py::TestWorkoutDeviceTranspile100Q::test_circSU2_100_transpile | 3 | 3 | runtime_s | 0.29178916616365314 | 0.28999870806001127 | -0.0010030411649495363 | 0.9963697968385223 | +0.36% |
| benchpress/qiskit_gym/device_transpile/test_summit.py::TestWorkoutDeviceTranspile100Q::test_circSU2_89_transpile | 2 | 3 | D2 | 312 | 312 | 0 | 1.0 | +0.00% |
| benchpress/qiskit_gym/device_transpile/test_summit.py::TestWorkoutDeviceTranspile100Q::test_circSU2_89_transpile | 2 | 3 | N2 | 318 | 318 | 0 | 1.0 | +0.00% |
| benchpress/qiskit_gym/device_transpile/test_summit.py::TestWorkoutDeviceTranspile100Q::test_circSU2_89_transpile | 2 | 3 | runtime_s | 3.206397916888818 | 3.1405245000496507 | -0.09153445903211832 | 0.9714032466159557 | +2.86% |
| benchpress/qiskit_gym/device_transpile/test_summit.py::TestWorkoutDeviceTranspile100Q::test_circSU2_89_transpile | 3 | 3 | D2 | 312 | 312 | 0 | 1.0 | +0.00% |
| benchpress/qiskit_gym/device_transpile/test_summit.py::TestWorkoutDeviceTranspile100Q::test_circSU2_89_transpile | 3 | 3 | N2 | 318 | 318 | 0 | 1.0 | +0.00% |
| benchpress/qiskit_gym/device_transpile/test_summit.py::TestWorkoutDeviceTranspile100Q::test_circSU2_89_transpile | 3 | 3 | runtime_s | 35.262829957995564 | 35.96152983303182 | 0.604634832823649 | 1.0172534067399035 | -1.73% |
| benchpress/qiskit_gym/device_transpile/test_summit.py::TestWorkoutDeviceTranspile100Q::test_clifford_100_transpile | 2 | 3 | D2 | 20464 | 20175 | -301 | 0.9852305300490696 | +1.48% |
| benchpress/qiskit_gym/device_transpile/test_summit.py::TestWorkoutDeviceTranspile100Q::test_clifford_100_transpile | 2 | 3 | N2 | 58170 | 57642 | -528 | 0.9909231562661166 | +0.91% |
| benchpress/qiskit_gym/device_transpile/test_summit.py::TestWorkoutDeviceTranspile100Q::test_clifford_100_transpile | 2 | 3 | runtime_s | 3.189904124941677 | 3.311809833161533 | 0.11351133300922811 | 1.0354911628804575 | -3.55% |
| benchpress/qiskit_gym/device_transpile/test_summit.py::TestWorkoutDeviceTranspile100Q::test_clifford_100_transpile | 3 | 3 | D2 | 20162 | 19880 | -282 | 0.9860080665239257 | +1.40% |
| benchpress/qiskit_gym/device_transpile/test_summit.py::TestWorkoutDeviceTranspile100Q::test_clifford_100_transpile | 3 | 3 | N2 | 58232 | 57734 | -506 | 0.9913231360175595 | +0.87% |
| benchpress/qiskit_gym/device_transpile/test_summit.py::TestWorkoutDeviceTranspile100Q::test_clifford_100_transpile | 3 | 3 | runtime_s | 4.524565165862441 | 4.619430458871648 | 0.09709475096315145 | 1.0214700449578202 | -2.15% |
| benchpress/qiskit_gym/device_transpile/test_summit.py::TestWorkoutDeviceTranspile100Q::test_square_heisenberg_100_transpile | 2 | 3 | D2 | 339 | 339 | 0 | 1.0 | +0.00% |
| benchpress/qiskit_gym/device_transpile/test_summit.py::TestWorkoutDeviceTranspile100Q::test_square_heisenberg_100_transpile | 2 | 3 | N2 | 1548 | 1548 | 0 | 1.0 | +0.00% |
| benchpress/qiskit_gym/device_transpile/test_summit.py::TestWorkoutDeviceTranspile100Q::test_square_heisenberg_100_transpile | 2 | 3 | runtime_s | 0.16740208282135427 | 0.16900262492708862 | -0.0004245832096785307 | 0.9974940081091592 | +0.25% |
| benchpress/qiskit_gym/device_transpile/test_summit.py::TestWorkoutDeviceTranspile100Q::test_square_heisenberg_100_transpile | 3 | 3 | D2 | 342 | 342 | 0 | 1.0 | +0.00% |
| benchpress/qiskit_gym/device_transpile/test_summit.py::TestWorkoutDeviceTranspile100Q::test_square_heisenberg_100_transpile | 3 | 3 | N2 | 1554 | 1554 | 0 | 1.0 | +0.00% |
| benchpress/qiskit_gym/device_transpile/test_summit.py::TestWorkoutDeviceTranspile100Q::test_square_heisenberg_100_transpile | 3 | 3 | runtime_s | 0.20526737510226667 | 0.20676562492735684 | 0.006074874196201563 | 1.0318492847784402 | -3.18% |

</details>

Invocation outcomes: {&quot;passed&quot;: 600}. Raw records: stages/benchpress/raw/; paired records: stages/benchpress/pairs/.

