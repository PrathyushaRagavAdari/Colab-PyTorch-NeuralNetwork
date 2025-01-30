Diabetes Dataset

Regression Task:
•Objective: Predict the quantitative progression of diabetes.

• Steps:
1. Dataset Preparation:
Loaded the Diabetes Dataset using load_diabetes() from sklearn.datasets.
Preprocessed the data using StandardScaler.
Split the data into training and test sets using train_test_split.
Converted the data into PyTorch tensors.

2. Neural Network Definition:
Built a feedforward neural network:
Input layer size = number of features (10).
Two hidden layers with 64 and 32 units, using ReLU activation.
Output layer with one neuron for regression.

3. Training:
Used MSELoss as the loss function and Adam as the optimizer.
Trained for 100 epochs, logging the loss every 10 epochs.

4. Evaluation:
Calculated mean squared error and R-squared.
Visualized predictions vs. true values using matplotlib.

Classification Task:
• Objective: Classify patients into "low progression" or "high progression" based on a threshold.

• Steps:
1. Dataset Preparation:
Used the same Diabetes Dataset but create binary labels:
Labeled patients as 1 (high progression) or 0 (low progression).
Used the median progression value as the threshold.
Split the data into training and test sets and preprocessed it.
Converted the data into PyTorch tensors.

2. Neural Network Definition:
Built a feedforward neural network:
Input layer size = number of features (10).
Two hidden layers with 64 and 32 units, using ReLU activation.
Output layer with 2 neurons for binary classification (softmax
activation).

3. Training:
Used CrossEntropyLoss as the loss function and Adam as the optimizer.
Trained for 100 epochs, logging the loss every 10 epochs.

4. Evaluation:
Calculated metrics such as accuracy, precision, recall, and F1-score.
Generated a confusion matrix and visualized it.