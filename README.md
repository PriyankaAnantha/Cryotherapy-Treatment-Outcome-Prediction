# Cryotherapy Treatment Prediction using Machine Learning

Developed a predictive model to determine the success of cryotherapy treatment using patient attributes.

## Project Overview
This project aims to develop a machine learning model to predict the success of cryotherapy treatment based on patient-specific characteristics. The dataset includes multiple factors such as patient age, gender, time elapsed before treatment, number of warts, types of warts, and wart surface area. The target variable is binary, indicating whether the treatment was successful (1) or unsuccessful (0).

## Dataset Details
- **Dataset**: Cryotherapy Dataset
- **Total Samples**: 90 patients
- **Features**:
  - **Sex**: Binary (1: Male, 2: Female)
  - **Age**: Continuous (15–67 years)
  - **Time Before Treatment**: Continuous (0–12 months)
  - **Number of Warts**: Continuous (1–12)
  - **Type of Wart**: Categorical (1: Common, 2: Plantar, 3: Both)
  - **Surface Area**: Continuous (4–750 mm²)
  - **Result of Treatment**: Binary (0: Unsuccessful, 1: Successful)

## Models Implemented
### 1. Baseline Model
- **Logistic Regression**
- **Accuracy**: 86.96%

### 2. Machine Learning Algorithms
- **Support Vector Machines (SVM)**
  - Linear Kernel: 86.96%
  - Polynomial Kernel: 73.91%
  - RBF Kernel: 91.30% (Best performing)
- **Decision Tree**
  - Accuracy: 82.61%
- **Random Forest**
  - Accuracy: 86.96%
- **AdaBoost**
  - Accuracy: 82.61%
- **Gradient Boosting**
  - Accuracy: 82.61%

## Hyperparameter Tuning
- **SVM (RBF Kernel)**
  - Best Parameters: C=10, gamma=0.1
  - Accuracy After Tuning: 91.30%
- **Decision Tree**
  - Best Parameters: max_depth=10, min_samples_split=2, min_samples_leaf=4
  - Accuracy After Tuning: 86.96%
- **Random Forest**
  - Best Parameters: n_estimators=200, max_features=log2
  - Accuracy After Tuning: 82.61%
- **AdaBoost**
  - Best Parameters: learning_rate=1, n_estimators=100
  - Accuracy After Tuning: 82.61%
- **Gradient Boosting**
  - Best Parameters: learning_rate=0.1, max_depth=3, n_estimators=200
  - Accuracy After Tuning: 82.61%

## Feature Selection & Reduction
- **PCA (50% dimensionality reduction)**: Accuracy = 69.57%
- **SelectPercentile (Top 50% features retained)**: Accuracy = 86.96%

## Results Summary
- **SVM with RBF Kernel** achieved the highest accuracy (91.30%), making it the most suitable model for predicting cryotherapy treatment success.
- **Feature scaling** significantly improved model performance.
- **Hyperparameter tuning** helped refine model accuracy.
- **Feature selection methods** demonstrated the impact of retaining the most important features while maintaining accuracy.

## File Structure
```
Project_Files/
│── ML_CourseProject_FinalReport.pdf
│── MLProjectReport_P1_PriyankaA.pdf
│── MLProject_P1_PriyankaA.ipynb
│── MLProject_Final_PriyankaA.ipynb
│── README.md  # Project documentation
```

## How to Run
1. **Enable GPU Runtime** in Google Colab or run locally.
2. Train models using Scikit-Learn by running the provided code.
3. Perform evaluation based on accuracy and performance metrics.
4. Compare results before and after hyperparameter tuning.

## Author
**Priyanka A**

