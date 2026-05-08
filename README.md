# Scratch Assay Analysis

Automated quantification of wound healing progression using image processing. Segments the scratch (wound) area from time-lapse microscopy images and tracks closure over time.

## Method

1. Convert to grayscale
2. Apply entropy filter (disk radius=5) to enhance texture contrast
3. Threshold with Yen method to segment the scratch region
4. Compute scratch area as percentage of total image
5. Fit a 3rd-degree polynomial to model healing kinetics

## Results

- Polynomial regression fit: **R² = 0.97**
- Healing tracked across 6 timepoints: 0, 1, 3, 12, 18, 24 hours

## Files

- `Scratch_Assay.ipynb` — full analysis notebook

## Stack

Python · scikit-image · NumPy · matplotlib · scipy · scikit-learn
