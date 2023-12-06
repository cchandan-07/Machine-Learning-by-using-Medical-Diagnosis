

# Medical Diagnosis by using Machine Learning

## Overview

Welcome to the Medical Diagnosis Machine Learning! This project aims to provide Collect diverse and comprehensive medical datasets for targeted conditions. Clean and preprocess data to ensure accuracy and completeness. Identify and optimize key diagnostic features for each medical condition. Select and train machine learning models tailored to each diagnosis for optimal accuracy. Define and measure performance metrics specific to each medical condition for effective model evaluation. Validate models rigorously using diverse datasets to ensure reliability and generalizability. Establish mechanisms for ongoing monitoring, updates, and incorporation of the latest medical knowledge.

## Table of Contents

1. [Getting Started](#getting-started)
   - [Prerequisites](#prerequisites)
   - [Installation](#installation)
2. [Usage](#usage)
   - [Input](#input)
   - [Output](#output)
4. [Data Preperation](#model-training)
3. [Model Training](#model-training)
   - [Dataset](#dataset)
   - [Training](#training)
4. [Evaluation](#evaluation)
5. [Contributing](#contributing)

## Getting Started

### Prerequisites

Before using this tool, make sure you have the following installed:

- Python (version >= 3.6)
-  numpy
-  Pandas
-  matplotlib

### Installation

1. Install dependencies:

   ```bash
   pip install -r requirements.txt 
   ```

## Usage

To use the pre-trained model for medical diagnosis, follow these steps:

1. Provide input data (medical images) following the guidelines in the [Input](#input) section.
2. Run the prediction script:

   ```bash
   python predict.py --input_path /path/to/input_data
   ```

### Input

The input data should be a collection of medical images in a supported format (e.g., JPEG, PNG). Place the images in a directory and provide the path to that directory as the input.

### Output

The prediction script will output the diagnosis results for each input image, indicating the likelihood of specific medical conditions.

## Data Preparation

### 1. Loading the Raw Dataset:
The first step in any data science project is to load the raw dataset into a format suitable for analysis. This allows us to examine the structure and content of the data.
Loading the raw dataset involves using appropriate data-loading functions provided by libraries like pandas in Python. This step enables us to read data from various sources such as CSV files, Excel spreadsheets, databases, or other formats. Once loaded, the dataset is typically stored in a DataFrame or a similar data structure, making it easy to manipulate and analyze.

### 2. Exploratory Data Analysis (EDA):

Exploratory Data Analysis (EDA) is the process of visually and statistically summarizing the main characteristics of a dataset. It helps us understand the underlying patterns, relationships, and potential issues within the data.
We create visualizations and summary statistics during EDA to gain insights into the dataset. Common EDA tasks include visualizing the distribution of target classes, examining correlations between features, detecting outliers, and understanding the central tendencies of numerical variables. EDA is crucial for informing subsequent steps in the data preparation process.

### 3. Data Cleaning:
Data cleaning involves handling missing values, duplicates, and any inconsistencies in the dataset. The goal is to ensure that the data is in a suitable form for analysis and modeling.
During this step, we identify and address missing values by imputing them or removing the corresponding rows or columns. Duplicates are removed to avoid redundancy in the dataset. Other cleaning tasks may include handling outliers and ensuring data integrity. The cleaned dataset provides a more accurate representation of the underlying phenomena.

### 4. Feature Scaling:
Feature scaling aims to standardize the range of independent variables or features of the dataset. This is important because machine learning models often perform better when features are on a similar scale.
Scaling is necessary when the features in the dataset have different ranges. Common scaling methods include Standard Scaling (Z-score normalization) and Min-Max Scaling. These techniques ensure that each feature contributes proportionally to the model's learning process, preventing some features from dominating due to their larger magnitudes.

### 5. Splitting Data into Features and Targets:
Separating the dataset into features and the target variable is a crucial step before training a machine learning model. Features are the independent variables used for prediction, while the target is the variable to be predicted.
The features (X) typically include all columns in the dataset except the target variable, while the target (y) is the specific variable we want the model to predict. This separation allows us to train the model on the features and evaluate its performance based on its ability to predict the target.

### 6. Train-Test Split:
Dividing the dataset into training and testing sets is essential to assess the model's generalization performance on unseen data.
The dataset is split into two subsets: the training set, used to train the machine learning model, and the testing set, reserved for evaluating the model's performance. The split ratio is often determined based on best practices. This ensures that the model is tested on data it has not seen during training, providing a more realistic assessment of its predictive capabilities.

## Model Training

### Dataset

To train the model on dataset, follow these steps:

1. Diabetes:  https://www.kaggle.com/datasets/uciml/pima-indians-diabetes-database
2. Cancer: https://www.kaggle.com/datasets/uciml/breast-cancer-wisconsin-data
3. liver: https://www.kaggle.com/datasets/uciml/indian-liver-patient-records
4. Kidney: https://www.kaggle.com/datasets/mansoordaku/ckdisease


### Training

Run the training script:

```bash
python train.py --config_path /path/to/config.yaml
```

## Evaluation

Evaluate the model's performance using the evaluation script:

```bash
python evaluate.py --model_path /path/to/saved_model --test_data /path/to/test_data
```
## Reference

Article
https://ieeexplore.ieee.org/document/9170733

## Contributing
It would like to contribute to this project by Chandanakumar and Kusuma
