# Rossmann Store Sales: Drivers of Daily Sales Across 1,115 Stores

Real daily sales data for 1,115 Rossmann drugstores across Germany, Jan 2013 - Jul 2015 -
from the Rossmann Store Sales Kaggle competition, not synthetic data.

## What's in this repo

[`notebooks/rossmann_analysis.ipynb`](notebooks/rossmann_analysis.ipynb) - exploratory
analysis of what actually drives daily sales: seasonality, day of week, promotions, store
type, and competition proximity.

## Key findings

- December sales run measurably above the yearly average (+14.5%), the clear seasonal peak.
- Promotions have a real, sizeable effect: promo days average 38.8% higher sales than days
  without one - the strongest single lever identified here.
- Store type 'b' stores substantially outsell the other types (50% above the lowest), despite
  being only 1.8% of store-days - a small, structurally different group.
- Distance to the nearest competitor has essentially no correlation with sales (r ≈ -0.036).
- Store-level performance varies widely (median ~€6,590/day, top store ~€21,757/day) even
  after accounting for type and promo activity.

Full detail and charts are in the notebook.

## Data

The dataset is not included in this repository (see the notebook for the source link) -
point `DATA_DIR` in the first code cell at your own local copy.

## Next steps

A natural follow-up is an actual sales forecasting model (the original Kaggle competition's
task) - likely gradient boosting on the features explored here, plus the store-level
variability identified in Section 8.
