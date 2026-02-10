## Overview
This project was conducted for a drug discovery competition.
I developed an end-to-end machine learning pipeline to predict molecular inhibition activity for drug candidate screening using multiple molecular representations and ensemble learning.

The pipeline integrates molecular feature engineering, model-specific feature selection, and ensemble modeling to improve predictive performance.

## Problem Definition
- Goal: Predict molecular properties for drug candidate screening
- Input: SMILES-based molecular representations
- Output: Regrtession prediction of molecular activity

## Methods

### Molecular Representation
Multiple molecular representations were explored to capture different aspects of chemical structures:
- Molecular descriptors (physicochemical properties)
- Morgan fingerprints (circular substructure patterns)
- Graph-based latent features extracted from a Graph Neural Network(GCN)

### Models
Several tree-based regression models were trained and compared:
- Random Forest
- XGBoost
- LightGBM
- CatBoost

### Ensemble Learning
- Stacking Regressor was used to combine predictions from multiple models
- Model-specific feature subsets were used as base learners to leverage complementary strengths of different representations

## Evaluation
- Cross-validation-based performance estimation
- RMSE and R²
- Comparative analyses between single models and ensemble models

## Key Findings
- Different machine learning models benefited from different molecular representations.
- Tree-based models (e.g., Random Forest, XGBoost) showed stronger performance with fingerprint-based features, while other models benefited more from descriptor-based or latent graph features.
- This highlighted the importance of model-feature compatibility rather than relying on a single universal representation.

## Experiments
Multiple feature combinations and models were tested during the competition.
For clarity and reproducibility, this repository contains the final best-performing pipeline selected based on cross-validation results.

## Tech Stack
- Language: Python
- Environment: Google Colab
- Libraries:
    - RDKit
    - PyTorch / PyTorch Geometric
    - scikit-learn
    - XGBoost, LightGBM, CatBoost