# AeroSentinel

AeroSentinel is a multi-source trust layer for detecting data-quality
anomalies and adversarial sensor manipulation in airport environmental
monitoring.

The framework integrates METAR surface observations with CAMS/EAC4 and
ERA5 atmospheric reanalysis data and uses cross-source consistency,
temporal, persistence, and aerosol-context features to identify corrupted
or manipulated sensor observations.

## Study locations

- Abu Dhabi International Airport (OMAA)
- Dubai International Airport (OMDB)

Study period: 2020–2025.

## Main methodology

The repository contains code for:

- METAR, CAMS/EAC4, and ERA5 data preprocessing
- Cross-source feature engineering
- Synthetic attack injection
- Temporal train/test splitting
- Expanding-window cross-validation
- Baseline detector comparison
- ExtraTrees training and evaluation
- Feature ablation
- Cross-airport transfer experiments
- Leave-one-attack-type-out evaluation
- Unseen and adaptive attack evaluation
- SHAP interpretability analysis

## Attack types

Five primary synthetic attack types are evaluated:

- Spike
- Drift
- Offset
- Stuck sensor
- Noise

Additional experiments evaluate unseen, adaptive, replay, and coordinated
attack scenarios.

## Reproducibility

Install the required Python packages using:

```bash
pip install -r requirements.txt
