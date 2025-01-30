California Housing Dataset


Regression Task:
• Objective: Predict median house values.

• Steps:
1. Dataset Preparation:
Loaded the California Housing Dataset using fetch_california_housing() from
sklearn.datasets.
Preprocessed the data using StandardScaler.
Split the data into training and test sets.
Converted the data into PyTorch tensors.

2. Neural Network Definition:
Replicated the neural network used for the Diabetes Dataset regression task.
Input layer size = number of features (8 for California Housing Dataset).

3. Training:
Used MSELoss as the loss function and Adam as the optimizer.
Trained for 100 epochs and log the loss every 10 epochs.

4. Evaluation:
Calculated mean squared error and R-squared.
Visualized predictions vs. true values.

Classification Task:
• Objective: Classify houses into "low value" or "high value" based on a threshold.

• Steps:
1. Dataset Preparation:
Used the same California Housing Dataset but create binary labels:
Labeled houses as 1 (high value) or 0 (low value) based on the
median value threshold.
Preprocessed and split the data as in the regression task.
Converted the data into PyTorch tensors.

2. Neural Network Definition:
Replicated the neural network used for the Diabetes Dataset classification
task.
Input layer size = number of features (8 for California Housing Dataset).
3. Training:
Used CrossEntropyLoss as the loss function and Adam as the optimizer.
Trained for 100 epochs and log the loss every 10 epochs.

4. Evaluation:
Calculated metrics such as accuracy, precision, recall, and F1-score.
Generated a confusion matrix and visualized it.



