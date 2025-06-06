
# KNN Classification on Iris Dataset

## What was done
You implemented a K-Nearest Neighbors (KNN) classifier on the famous Iris dataset using Python and the scikit-learn library. Your workflow included data preprocessing, normalization, model training and testing, choosing the optimal value of K using cross-validation, evaluating the model using a confusion matrix, and visualizing decision boundaries with pair plots.

## How it was done

### 1. Data Loading
- You loaded the Iris dataset from scikit-learn's datasets module.
- The dataset contains 4 features: sepal length, sepal width, petal length, and petal width.

### 2. Preprocessing
- You converted the dataset to a pandas DataFrame for easy handling.
- You normalized the features using `StandardScaler` to improve model performance.

### 3. Model Training and Testing
- You split the data into training and testing sets using `train_test_split`.
- You trained the KNN classifier with different values of K (1-20) using 10-fold cross-validation to determine the best K.

### 4. Choosing K
- You evaluated accuracy for different values of K using the Elbow method.
- K values of 5, 14, and 15 emerged as good choices, with 5 being the most consistent.

### 5. Model Evaluation
- You computed the confusion matrix and classification report to assess model performance.

### 6. Visualizing Decision Boundaries
- You created a pair plot with scatter plots and overlaid decision boundaries for each feature pair using KNN.
- This helped you understand how the classifier performs on different pairs of features.

## Summary
This project demonstrated a complete KNN classification pipeline: from data loading and preprocessing to model training, hyperparameter tuning, evaluation, and visualization. It highlighted the importance of proper preprocessing and the effectiveness of the KNN classifier on simple yet popular datasets like Iris.

