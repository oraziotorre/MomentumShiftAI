# MomentumShiftAI

MomentumShiftAI is a machine learning project focused on detecting and predicting **momentum shifts** and **comebacks** in tennis and table tennis matches. It leverages detailed information about point-by-point score progressions to train models capable of identifying when a player is likely to turn the match around.

## 🚀 Project Goals

- Detect *momentum shifts* during a match
- Predict potential *comebacks* before they fully materialize
- Explore the psychological and tactical dimensions of match dynamics through data

## 🏓 Sports Covered

- **Tennis**
- **Table Tennis**

Each sport has its own dataset structure and progression patterns, which are handled accordingly in the preprocessing pipeline.

## 📊 Datasets

- `raw_dataset_TT`: Raw dataset of table tennis matches  
- `singles_TT`: Cleaned dataset of singles-only table tennis matches  
- `TT`: Cleaned dataset of all table tennis matches  
- `tennis`: Cleaned dataset of all tennis matches  
- `tennis_2010-now`: Subset of the tennis dataset containing only matches from 2010 onwards

### Dataset Ordering

- Table tennis datasets are ordered **from oldest to most recent**
- Tennis datasets are ordered **from most recent to oldest**
- **Inverted instances** (i.e., mirrored match records) start from the midpoint of each dataset

> ⚠️ In the `tennis` dataset, the **last value of the score progression must be removed** during preprocessing.

## 🧠 Models

The project experiments with various model architectures including:

- Recurrent Neural Networks (RNNs)
- Transformer-based sequence models
- Gradient boosting models with engineered features

Models are trained to classify whether a comeback or momentum shift occurs within a match window, using scoring sequences and contextual match metadata.

## 📦 Structure
