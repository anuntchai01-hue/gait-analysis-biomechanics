# Gait Analysis for Enhanced Gait Biomechanics Dataset

## Overview
This project analyses gait biomechanics data collected using GRAIL
(Gait Real-time Analysis Interactive Lab) across three conditions:
- Unbraced
- Knee-braced
- Ankle-braced
- 
## Objective
To investigate how knee and ankle bracing alter gait biomechanics
and to classify gait conditions using machine learning.

## Dataset
**Source:** [Enhanced Gait Biomechanics Dataset — Kaggle](https://www.kaggle.com/datasets/anitarostami/enhanced-gait-biomechanics-dataset)

- 10 subjects × 3 conditions × 10 replications
- 2 legs (left, right) × 3 joints (ankle, knee, hip)
- 178,200 total observations
- Variables: joint angle (°), normalised velocity, normalised acceleration
- Full gait cycle recorded (0–100%)

> **Note:** Download the dataset from Kaggle and rename it to
> `Gait_Biomechanics_Dataset.csv` before running the notebook.

## Analysis
- Exploratory Data Analysis (EDA)
- Visualisation — boxplots, line plots, correlation heatmap
- Machine Learning classification (Gradient Boosting — 92.5% accuracy)
- Statistical Analysis — Repeated Measures ANOVA

  ## Analysis
- Exploratory Data Analysis (EDA)
- Visualisation — boxplots, line plots, correlation heatmap
- Machine Learning classification (Gradient Boosting — 92.5% accuracy)
- Statistical Analysis — Repeated Measures ANOVA

## Skills Demonstrated
- Biomechanics interpretation
- Statistical analysis (Repeated Measures ANOVA)
- Machine learning classification
- Data visualization
- Feature importance analysis

## Results
| Model | Accuracy |
|---|---|
| Logistic Regression | 82.9% |
| Random Forest | 89.6% |
| Gradient Boosting | 92.5% |

Key findings:
- Acceleration was the most sensitive biomechanical measure (η²=0.576)
- Knee range of motion was the most important classification feature
- Combining all 3 joints improved accuracy by up to +29%

## Requirements
```python
pip install pandas numpy matplotlib seaborn scikit-learn pingouin
```

## How to Run
1. Clone this repository
2. Open `Gait_analysis.ipynb` in JupyterLab
3. Run all cells top to bottom (Kernel → Restart and Run All Cells)

## Tools Used
- Python 3.9
- JupyterLab
- pandas, numpy, matplotlib, seaborn
- scikit-learn
- pingouin
