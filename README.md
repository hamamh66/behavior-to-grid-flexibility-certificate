# Behavior-to-Grid Flexibility Certificate

This repository notebook provides a self-contained synthetic demonstration of an abstention-aware flexibility certificate for workplace electric-vehicle charging on a linearized IEEE 33-bus feeder.

## Run the notebook

Open `BGFC_GitHub_Reproducible_Demo.ipynb` in Google Colab or a local Jupyter environment and run all cells in order.

Required packages:

- NumPy
- pandas
- Matplotlib

In Google Colab, results are written to:

```text
MyDrive/Outputs/BGFC/<timestamp>/
```

In a local environment, results are written to:

```text
Outputs/BGFC/<timestamp>/
```

## What the demonstration includes

- behavioral response bounds derived from a declared bunching input;
- a linearized 24-hour IEEE 33-bus feeder calculation;
- 400 reproducible synthetic uncertainty scenarios;
- separate calibration and held-out test sets;
- static and adaptive certificate policies;
- explicit abstention under synthetic distribution shift;
- Wilson confidence intervals and paired bootstrap inference;
- scenario-level CSV outputs, figures, tables, metadata, and a results archive.

## Evidence boundary

The bunching estimate is an imported numerical input. Load profiles, response draws, forecast errors, OOD labels, service values, and controller comparisons are synthetic. The code demonstrates certificate mechanics; it does not provide field validation, causal identification, or full AC-network certification.

## Reproducibility

The random seed is fixed at `20260719`. Each run records its configuration and writes timestamped outputs without overwriting prior runs.
