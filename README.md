## Overview
This project was conducted for a drug discovery competition.
I developed machine learning models to predict molecular properties using molecular descriptors and fingerprints.

## Problem Definition
- Goal: Predict molecular properties for drug candidate screening
- Input: SMILES-based molecular representations
- Output: Regrtession prediction of molecular activity

## Methods
- Feature extraction:
    - Molecular descriptors
    - Morgan fingerprint
- Models:
    - XGBoost
    - Random Forest
    - LGBM
    - CatBoost
- Emsemble:
    - Stacking Regressor

## Evauluation
- Cross-validation
- RMSE / R2
- Comparison between single models and ensemble models

## What I Learned
- I observed that different machine learning models benefited from different molecular representations.
- Tree-based models (e.g., Random Forest, XGBoost) showed stronger performance with fingerprint-based features, while other models benefited more from descriptor-based features.
- This motivated me to apply model-specific feature selection and combine them using ensemble learning.

## Experiments
Multiple feature combinations and models were tested during the competition.
The final version reflects the best-performing configuration based on cross-validation results.

## Tech Stack
- Language: Python
- Environment: Google Colab