# Diabetes Prediction using Multilayer Perceptron (MLP)

## Project Overview
This project implements a Multilayer Perceptron (MLP) neural network for predicting diabetes using medical tabular data. The model classifies patients into diabetic and non-diabetic categories based on several medical features.

---

## Problem Description
Diabetes is a common medical condition that can be identified using different health indicators. This project aims to build an Artificial Neural Network capable of predicting whether a patient has diabetes using medical measurements from the dataset.

---

## Dataset

### Dataset Name
Pima Indians Diabetes Dataset

### Dataset Link
https://www.kaggle.com/datasets/uciml/pima-indians-diabetes-database

### Dataset Features
- Pregnancies
- Glucose
- Blood Pressure
- Skin Thickness
- Insulin
- BMI
- Diabetes Pedigree Function
- Age

### Target Variable
- 0 → Non-diabetic
- 1 → Diabetic

---

## Data Preprocessing

The following preprocessing techniques were applied:

- Replaced invalid values (0 values) with mean values
- Handled missing values
- Applied feature scaling using StandardScaler
- Split dataset into:
  - Training Set: 80%
  - Testing Set: 20%

---

## Model Architecture

The implemented model is a Multilayer Perceptron (MLP):

- Input Layer: 8 features
- Hidden Layer 1: 16 neurons + ReLU activation
- Hidden Layer 2: 8 neurons + ReLU activation
- Output Layer: 1 neuron + Sigmoid activation

### Loss Function
- Binary Cross Entropy Loss (BCELoss)

### Optimizer
- Adam Optimizer

### Epochs
- 50

---

## Experiments

Two experiments were performed by changing the learning rate.

| Experiment | Learning Rate | Test Accuracy | Final Loss |
|------------|--------------|---------------|------------|
| Experiment 1 | 0.001 | 75% | 0.52 |
| Experiment 2 | 0.01 | 80% | 0.40 |

---

## Final Results

- Best Test Accuracy: 80%
- Final Test Loss: 0.40

---

## Visualizations

### Experiment 1 (Learning Rate = 0.001)

#### Accuracy Curve

![Accuracy Exp1](RESULT_1.png)

#### Loss Curve

![Loss Exp1](RESULT_2.png)

---

### Experiment 2 (Learning Rate = 0.01)

#### Accuracy Curve

![Accuracy Exp2](RESULT_3.png)

#### Loss Curve

![Loss Exp2](RESULT_4.png)

---

## Technologies Used

- Python
- PyTorch
- Pandas
- NumPy
- Scikit-learn
- Matplotlib

---

## Files Included

- diabetes.csv
- diabetes_mlp_project.ipynb
- README.md
- RESULT_1.png
- RESULT_2.png
- RESULT_3.png
- RESULT_4.png

---

## How to Run

Install required libraries:

pip install numpy pandas matplotlib scikit-learn torch
Run the notebook:

jupyter notebook
Open the notebook:

diabetes_mlp_project.ipynb
Run all notebook cells from top to bottom.

