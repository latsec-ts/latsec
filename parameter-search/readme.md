# Parameter search

`LaTSEC-Parameter-Selection-v2.2-fixedtailbound.ipynb` selects the LaTSEC parameter sets of Section 7 (Tables 4 and 5) and estimates their concrete security.

- Lattice estimator: commit `27a581b` of https://github.com/malb/lattice-estimator.
- Modulus: for each tuple, q is the largest prime below 2^b_q with q ≡ 1 (mod 2d) and q > 2B_MSIS + 1, where b_q = ⌈lg q⌉.
- `estimator-calibration/`: the CRYSTALS security-estimation scripts for Kyber and Dilithium (https://github.com/pq-crystals/security-estimates), with their output for Dilithium (`output_for_Dilithium.py`) and two small example scripts (`my_LWE_estimate.sage`, `my_SIS_estimate.sage`). Included for reference only; the LaTSEC parameters are computed with the lattice estimator above.