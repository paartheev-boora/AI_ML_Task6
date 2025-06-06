
# KNN Classification on Iris Dataset

## Frameworks and Libraries Used
- **scikit-learn**: For data preprocessing, model training, evaluation, and metrics (train_test_split, StandardScaler, KNeighborsClassifier, confusion_matrix, cross_val_score).
- **pandas**: For dataset manipulation and DataFrame operations.
- **numpy**: For numerical operations.
- **matplotlib**: For plotting evaluation curves and visualizing decision boundaries.
- **seaborn**: For enhanced data visualization.

## Models Used
- **K-Nearest Neighbors (KNN)** classifier: A simple, yet effective, non-parametric algorithm for classification tasks.

## Dataset
- **Iris dataset**: A classic dataset containing measurements of sepal length, sepal width, petal length, and petal width for three Iris species (setosa, versicolor, virginica).

## Methods Used
- **Data Preprocessing**:
  - Loaded the Iris dataset using scikit-learn.
  - Normalized features using `StandardScaler` for improved model performance.
  - Converted to pandas DataFrame for easy manipulation.
- **Train/Test Split**:
  - Used `train_test_split` to partition the data into training and testing sets.
- **Model Training and Evaluation**:
  - Trained a KNN classifier with various values of K (1 to 20).
  - Used 10-fold cross-validation (`cross_val_score`) to determine the optimal K.
  - Used the Elbow method to visually identify the best K based on accuracy.
- **Confusion Matrix and Metrics**:
  - Computed the confusion matrix to evaluate classification performance.
- **Visualization**:
  - Plotted decision boundaries using a custom function with `ListedColormap`.
  - Created a pair plot with histograms on the diagonal and decision boundaries on scatter plots for each feature pair.

## Insights Revealed
- The Iris dataset is well-separated, especially between setosa and other species, with minor overlaps between versicolor and virginica.
- The Elbow method suggested that **K=5** is a consistent choice with high accuracy, though higher K values (14–15) also performed well.
- Visualizing decision boundaries revealed how KNN partitions the feature space and how each species occupies distinct regions.
- The confusion matrix showed high classification accuracy with minimal misclassifications.

## Additional Insights from Visualizations
- Pair plots with decision boundaries highlighted:
  - **Setosa** is linearly separable from the other two species.
  - **Versicolor** and **Virginica** exhibit some overlap, but can be distinguished using petal measurements.
  - Feature pairs like petal length vs. petal width showed clear separation.
  - Sepal features alone provide less separation compared to petal features.

## Summary
This project demonstrates the implementation of a KNN classifier from start to finish, covering data preprocessing, model selection, evaluation, and visualization. The analysis confirms that KNN is highly effective for the Iris dataset and highlights the importance of proper feature selection and data visualization in understanding model behavior.

