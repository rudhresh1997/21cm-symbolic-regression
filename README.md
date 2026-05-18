# 21 cm Symbolic Regression

Interpretable symbolic regression for parameter recovery from simulated 21 cm power spectra.

This project investigates symbolic recoverability in nonlinear 21 cm cosmology using semi-numerical simulations, machine-learning baselines, symbolic regression, ablation studies, robustness tests, and bootstrap uncertainty diagnostics.

## Current Status

This repository currently contains the validated `n=100` prototype pipeline.

Completed notebooks:

- `00_environment_check.ipynb`
- `01_21cmfast_single_simulation_test.ipynb`
- `02_parameter_sampling_lhs.ipynb`
- `03_dataset_generation_power_spectra.ipynb`
- `04_preprocessing_feature_matrix.ipynb`
- `05_baselines_rf_mlp.ipynb`
- `06_pysr_symbolic_regression.ipynb`
- `07_redshift_scale_ablations.ipynb`
- `08_robustness_noise_missing_channels.ipynb`
- `09_bootstrap_uncertainty.ipynb`
- `10_complexity_recoverability_figures.ipynb`

## Scientific Goal

To study whether compact symbolic expressions can recover cosmological and astrophysical parameters from simulated 21 cm power spectra, and how symbolic recoverability changes with inverse-problem complexity.

## Parameters

The current parameter set is:

- Ionizing efficiency, zeta
- Minimum virial temperature, log10(Tvir/K)
- Mean free path, R_mfp
- X-ray luminosity proxy, log10(L_X)
- Matter fluctuation amplitude, sigma8

## Main Observable

The input observable is the dimensionless 21 cm power spectrum:

Delta^2_21(k, z)

evaluated across multiple redshifts and k-bins.

## Repository Notes

Large generated datasets, model files, and raw simulation outputs are excluded from Git and should be archived separately using Zenodo or similar archival storage.

## Citation

A formal DOI will be added after archival release.
