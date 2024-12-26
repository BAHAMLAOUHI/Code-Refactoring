# Class-Level Code Refactoring Prediction

This project aims to predict the need for class-level code refactoring in software systems by leveraging machine learning and deep learning techniques. It provides an automated approach to detect areas in the codebase requiring improvement, enhancing maintainability and overall software quality.


### 1. Data Collection
- Extracted **class-level metrics** using the **SourceMeter** tool. These metrics include:
  - Number of Methods
  - Lack of Cohesion in Methods (LCOM)
  - Cyclomatic Complexity
  - Other relevant metrics reflecting class-level characteristics.

### 2. Feature Selection
- **Wilcoxon Rank Sum Test**: Used to identify significant features.
- **Pearson Correlation**: Applied to eliminate highly correlated features.
- **SelectKBest**: Retained the top K features based on statistical scores.

### 3. Data Normalization
- Applied **Min-Max Scaling** to standardize feature values to a range of [0, 1].

### 4. Handling Imbalanced Data
- Utilized **SMOTE (Synthetic Minority Over-sampling Technique)** to balance the dataset and improve model performance.

### 5. Experimenting with Different Algorithms
- **Machine Learning Models**:
  - Logistic Regression (LR)
  - Support Vector Machines (SVM) with various kernels
  - Decision Trees (DT)
  - Random Forest Classifier (RFC)
- **Deep Learning Model**:
  - Designed and trained a neural network for classification tasks.

### 6. Performance Comparison
- Evaluated models using metrics such as accuracy, precision, recall, and F1-score to determine the most effective approach.

### 7. Model Selection
- Chose the best-performing model based on its evaluation metrics and suitability for real-world applications.
