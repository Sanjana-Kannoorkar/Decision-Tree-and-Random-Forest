# Decision-Tree-and-Random-Forest

# Heart Disease Prediction using Machine Learning
A machine learning project that predicts heart disease using Decision Trees and Random Forests, with comprehensive model analysis and visualization.

## Dataset
- **Source**: [UCI Heart Disease Dataset](https://archive.ics.uci.edu/ml/datasets/Heart+Disease) (cleaned version)
- **Samples**: 1,025 patient records
- **Features**: 13 clinical features
- **Target**: Binary classification (0 = No disease, 1 = Disease)

## Features
Key features used in the analysis:
1. `age`: Patient age
2. `sex`: Gender (1 = male, 0 = female)
3. `cp`: Chest pain type (0-3)
4. `trestbps`: Resting blood pressure
5. `chol`: Serum cholesterol
6. `thalach`: Maximum heart rate achieved

## Models
### 1. Decision Tree Classifier
- Achieved **94.15% test accuracy** at optimal depth=4
- Key findings:
  - Prone to overfitting (100% training accuracy at max depth)
  - Most important feature: Chest pain type (`cp`)

### 2. Random Forest Classifier
- Achieved **95.12% test accuracy**
- 5-fold cross-validation score: **94.07% ± 0.79%**
- More robust performance than single Decision Tree

## Results
| Model               | Test Accuracy | Key Features |
|---------------------|---------------|--------------|
| Decision Tree       | 94.15%        | cp, thalach  |
| Random Forest       | 95.12%        | cp, oldpeak  |

Classification reports available in the Jupyter notebook.
