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

## Evaluation
- Cross-validation
- RMSE / R2
- Comparison between single models and ensemble models

## What I Learned
- Importance of molecular representation in prediction performance
- Effect of feature selection on ensemble models
- Limitations of classical ML for molecular data