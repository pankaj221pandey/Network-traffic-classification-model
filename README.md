# Network Traffic Classification Model

This repository contains code for building a network traffic
classification model using deep learning. The model is designed to
classify network traffic based on various features and detect potential
network attacks.

## Table of Contents

-   [Introduction](#introduction)
-   [Dataset](#dataset)
-   [Installation](#installation)
-   [Usage](#usage)
-   [Data Preprocessing](#data-preprocessing)
-   [Model Training](#model-training)
-   [Evaluation](#evaluation)
-   [Results](#results)
-   [Contributing](#contributing)
-   [License](#license)

## Introduction

The Network Traffic Classification Model aims to classify network
traffic into different categories and identify malicious activities.
This project involves data preprocessing, feature engineering, data
visualization, and building a deep learning model using LSTM (Long
Short-Term Memory) networks.

## Dataset

The dataset used for this project is a combination of two CSV files: -
`CIDDS-002-week1.csv` - `CIDDS-002-week2.csv`

These files contain network traffic data with various features such as
source and destination IP addresses, ports, protocols, and attack
descriptions.

## Installation

To run this project, you need to have Python installed along with the
necessary libraries. You can install the required libraries using the
following command:

```bash 
pip install -r requirements.txt 
```

## Usage 

1 Clone the repository:


```bash
git clone https://github.com/yourusername/network-traffic-classification-model.git
cd network-traffic-classification-model 
```

2 Place the dataset files
(CIDDS-002-week1.csv and CIDDS-002-week2.csv) in the repository
directory.

3 Run the main script:

```bash
 python main.py
 ``` 

## Data Preprocessing 
The data preprocessing steps include:

- Concatenating multiple CSV files into a single DataFrame. 
- Handling missing values and data types. 
- Creating new binary columns for specific flags. 
- Dropping unnecessary columns and renaming columns for clarity.
- Encoding categorical variables using LabelEncoder. 
- Visualizing data distributions and correlations. 

## Model Training 

### The model is built using Keras with the following architecture:

- Multiple LSTM layers with dropout for regularization. 
- Dense output layer for classification. 
- Compiled with Adam optimizer and mean squared error loss function. 

## Evaluation 

The model is evaluated using R-squared scores
for both training and test sets. The training process includes
validation to monitor the model's performance on unseen data.

## Result
Results The results of the model training and evaluation, including loss
plots and accuracy scores, are displayed to assess the model's
performance.

## Contributing
Contributing Contributions are welcome! Please open an issue or submit a
pull request for any improvements or new features.


## Licence
License This project is licensed under the MIT [License](/LICENSE). See the LICENSE
file for details.

