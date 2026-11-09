# Predictive Maintenance – Machine Failure Prediction

## Project Overview

Predictive Maintenance is a Machine Learning project that predicts potential machine failures using operational sensor data.

The project analyzes machine parameters such as air temperature, process temperature, rotational speed, torque, and tool wear to identify whether a machine is likely to experience failure.

The main objective is to identify potential machine failures in advance, helping industries reduce unexpected downtime, improve equipment reliability, and optimize maintenance activities.

## Problem Statement

Unexpected machine failures can lead to production delays, increased maintenance costs, and reduced operational efficiency.

This project uses Machine Learning classification algorithms to predict machine failure based on historical sensor data.

The prediction problem is classified into two categories:

- **0 – No Failure:** The machine is predicted to operate without failure.
- **1 – Failure:** The machine is predicted to experience failure.

## Dataset

**Dataset:** AI4I 2020 Predictive Maintenance Dataset

The dataset contains machine operational parameters and machine failure information.

### Dataset Features

| Feature | Description |
|---|---|
| Type | Machine quality type (L, M, H) |
| Air temperature [K] | Air temperature in Kelvin |
| Process temperature [K] | Process temperature in Kelvin |
| Rotational speed [rpm] | Machine rotational speed |
| Torque [Nm] | Machine torque |
| Tool wear [min] | Tool wear in minutes |
| Machine failure | Target variable (0 or 1) |

The sensor parameters are used as input features, while `Machine failure` is the target variable.

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Google Colab
- Git
- GitHub

## Exploratory Data Analysis (EDA)

Exploratory Data Analysis is performed to understand the dataset, identify patterns, and analyze relationships between machine sensor parameters and machine failure.

### Data Visualization

- Machine Failure Distribution
- Machine Type vs Failure
- Sensor Feature Distributions
- Correlation Heatmap
- Boxplot Analysis
- Torque vs Rotational Speed
- Air Temperature vs Process Temperature

These visualizations help identify patterns and understand how sensor measurements relate to machine failure.

## Machine Learning Algorithms

Two Machine Learning classification algorithms are implemented and compared.

### 1. Logistic Regression

Logistic Regression is a classification algorithm used to predict the probability of machine failure.

It is implemented as a baseline model for evaluating machine failure prediction performance.

### 2. Random Forest Classifier

Random Forest is an ensemble learning algorithm that combines multiple decision trees to make predictions.

It is used to identify patterns in machine sensor data and predict machine failure.

## Project Workflow

1. Import required libraries
2. Load the dataset
3. Inspect the dataset
4. Handle duplicate records
5. Perform Exploratory Data Analysis
6. Identify input features and target variable
7. Split the dataset into training and testing sets
8. Apply data preprocessing
9. Train Logistic Regression and Random Forest models
10. Evaluate model performance
11. Compare the models
12. Select the best-performing model
13. Analyze feature importance
14. Predict machine failure using new sensor inputs

## Data Preprocessing

The following preprocessing techniques are implemented:

- Removal of duplicate records
- Separation of input features and target variable
- Train-test splitting
- One-Hot Encoding for categorical machine type
- Standard Scaling for numerical features
- Pipeline-based preprocessing and model training

The dataset is divided into 80% training data and 20% testing data.

Stratified splitting is used to maintain the class distribution between the training and testing datasets.

## Model Evaluation

The Machine Learning models are evaluated using the following metrics:

| Metric | Description |
|---|---|
| Accuracy | Measures overall prediction correctness |
| Precision | Measures how many predicted failures are actual failures |
| Recall | Measures how many actual failures are correctly identified |
| F1 Score | Balances precision and recall |
| Confusion Matrix | Shows correct and incorrect predictions |
| ROC Curve | Evaluates classification performance |
| Precision-Recall Curve | Evaluates the trade-off between precision and recall |

Both models are compared using these evaluation metrics.

The model with the highest F1 Score is selected as the best-performing model.

## Feature Importance

Feature importance analysis is performed using the Random Forest Classifier.

It helps identify the sensor parameters that contribute most to machine failure prediction.

The analysis provides insights into the relationship between machine operating conditions and potential failures.

## Machine Failure Prediction

The project allows users to enter new machine sensor values:

- Machine Type
- Air Temperature
- Process Temperature
- Rotational Speed
- Torque
- Tool Wear

The selected Machine Learning model processes the input values and predicts the machine status.

### Prediction Output

The final prediction report includes:

- Selected Machine Learning Model
- Machine Failure Prediction
- Estimated Failure Probability

The output indicates whether the machine is predicted to experience failure based on the provided sensor measurements.

## Project Structure

```text
Predictive-Maintenance/
│
├── Predictive_Maintenance.ipynb
├── requirements.txt
├── README.md
│
└── dataset/
    └── ai4i2020.csv
```

*Update the file names and folder structure according to your actual project.*

## Installation and Execution

### Step 1: Clone the Repository

```bash
git clone https://github.com/your-username/Predictive-Maintenance.git
```

### Step 2: Navigate to the Project Folder

```bash
cd Predictive-Maintenance
```

### Step 3: Install Required Libraries

```bash
pip install -r requirements.txt
```

### Step 4: Execute the Project

Open the Jupyter Notebook in Google Colab or Jupyter Notebook.

1. Load the dataset.
2. Execute the notebook cells sequentially.
3. Perform data analysis and visualization.
4. Train and evaluate the Machine Learning models.
5. Enter machine sensor values to generate predictions.

## Requirements

```text
pandas
numpy
matplotlib
seaborn
scikit-learn
```

Install the required libraries using:

```bash
pip install -r requirements.txt
```

## Author

**Predictive Maintenance – Machine Failure Prediction**

Machine Learning | Python | Data Analysis | Scikit-learn

## License

This project is developed for educational and portfolio purposes.
