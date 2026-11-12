# Parameter search

`LaTSEC-Parameter-Selection-v2.2-fixedtailbound.ipynb` selects the LaTSEC parameter sets of Section 7 (Tables 4 and 5) and estimates their concrete security.

- Lattice estimator: commit `27a581b` of https://github.com/malb/lattice-estimator.
- Modulus: for each tuple, q is the largest prime below 2^b_q with q ≡ 1 (mod 2d) and q > 2B_MSIS + 1, where b_q = ⌈lg q⌉.
- `estimator-calibration/`: security estimates for Kyber and Dilithium computed with the same lattice-estimator setup (commit `27a581b`), as a sanity check of the attack and cost models used for LaTSEC. Not required to reproduce the LaTSEC parameters.