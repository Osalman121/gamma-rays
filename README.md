This project applies machine learning classification models to the Magic04 dataset, a dataset containing information about gamma and hadron events observed by a high-energy physics experiment. The goal is to classify the events as either gamma or hadron based on multiple feature measurements.

Table of Contents
Introduction
Data Preparation
Classification Models
Model Parameter Tuning
Evaluation
Usage
Dependencies
Introduction
The dataset is preprocessed and balanced to ensure equal sizes for both classes (gamma and hadron events). Different classifiers are applied to the dataset, including Decision Tree, AdaBoost, Random Forests, and Naive Bayes. The code uses cross-validation and grid search to tune the model parameters, and the best-performing models are evaluated on a separate testing set.

Data Preparation

Data Loading: The dataset is loaded from the file magic04.data.
Class Balancing: The dataset is balanced by randomly undersampling the majority class (gamma events) to match the size of the minority class (hadron events).
Data Splitting: The balanced dataset is split into features (X) and target (y), and further split into training and testing sets using a 70-30 split.
Classification Models
Decision Tree: A decision tree classifier with no parameters to tune.
AdaBoost: An AdaBoost classifier with parameters to tune (n_estimators and learning_rate).
Random Forests: A Random Forests classifier with parameters to tune (n_estimators and max_depth).
Naive Bayes: A Naive Bayes classifier with no parameters to tune.
Model Parameter Tuning
Cross-Validation and Grid Search: Cross-validation with grid search is applied to each classifier to tune the model parameters. This process finds the best parameter values for each classifier based on accuracy.
Best Models: The best models and parameters are stored for further evaluation.
Evaluation
The best models are evaluated on the testing set.
Metrics: Accuracy, precision, recall, F1-score, and confusion matrix are calculated for each model.
Visualization: The confusion matrix is visualized using a heatmap.
Usage
Load the code in your Python environment.
Ensure you have the required dependencies installed (see below).
Run the code to perform the classification tasks and evaluate the models.
Dependencies
Python 3.x
NumPy
pandas
matplotlib
seaborn
sklearn
Ensure you have these libraries installed using pip:

pip install numpy pandas matplotlib seaborn scikit-learn
Contact:

For any issues, questions, or contributions, feel free to open an issue or submit a pull request.








