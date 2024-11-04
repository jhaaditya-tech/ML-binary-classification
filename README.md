# Binary Text Classification Using 20 Newsgroups Dataset

This project is part of CS 640 and involves implementing a binary text classifier using a modified version of the well-known [20 Newsgroups dataset](https://scikit-learn.org/0.19/datasets/twenty_newsgroups.html). The classifier is designed to distinguish between two groups of newsgroups, categorized broadly into technology & science and sports, politics & miscellaneous.

## Table of Contents
- [Project Overview](#project-overview)
- [Dataset Information](#dataset-information)
- [Requirements](#requirements)
- [Installation](#installation)
- [Usage](#usage)
- [Evaluation Metrics](#evaluation-metrics)
- [Results](#results)

## Project Overview
The objective of this assignment is to build a binary classifier that identifies if a given document from the 20 Newsgroups dataset belongs to:
- **Class 1:** Technology & Science (e.g., computers, electronics, science topics).
- **Class 2:** Sports, Politics, & Miscellaneous (e.g., sports, political topics, religion).

## Dataset Information
The 20 Newsgroups dataset includes approximately 18,846 documents divided into 20 classes. For this project, these classes have been combined into two broad categories:
- **Class 1:** `comp.graphics`, `comp.os.ms-windows.misc`, `comp.sys.ibm.pc.hardware`, `comp.sys.mac.hardware`, `comp.windows.x`, `sci.crypt`, `sci.electronics`, `sci.med`, `sci.space`
- **Class 2:** `rec.autos`, `rec.motorcycles`, `rec.sport.baseball`, `rec.sport.hockey`, `talk.politics.misc`, `talk.politics.guns`, `talk.politics.mideast`, `talk.religion.misc`, `misc.forsale`, `alt.atheism`, `soc.religion.christian`

The dataset is split into training (11,314 samples) and test data.

## Requirements
- Python 3.7 or higher
- Jupyter Notebook
- Libraries:
  - scikit-learn
  - nltk
  - pandas
  - numpy

## Installation
1. Clone the repository:
    ```bash
    git clone https://github.com/yourusername/binary-text-classifier.git
    cd binary-text-classifier
    ```

2. Install required packages:
    ```bash
    pip install -r requirements.txt
    ```

3. Open the Jupyter Notebook:
    ```bash
    jupyter notebook Homework3.ipynb
    ```

## Usage
1. Run all cells in `Homework3.ipynb` to:
   - Download and preprocess the dataset.
   - Split data into training and validation sets.
   - Train the model and select the best-performing model based on validation accuracy.
   - Evaluate the model on the test dataset.

2. View final evaluation metrics like accuracy, precision, recall, and F1-score for model performance assessment.

## Evaluation Metrics
The classifier's performance is measured on the test dataset using:
- **Accuracy**
- **Precision**
- **Recall**
- **F1 Score**

## Results
The models were evaluated on the test dataset, with the following results:

| Model               | Accuracy | Precision | Recall | F1-Score |
|---------------------|----------|-----------|--------|----------|
| Logistic Regression | 86.45%   | 0.8493    | 0.8420 | 0.8456   |
| Naive Bayes         | 84.42%   | 0.8263    | 0.8181 | 0.8221   |

- **Logistic Regression** was selected as the final model due to its superior performance, achieving higher accuracy and F1-score compared to Naive Bayes.
- Logistic Regression demonstrated a balanced trade-off between precision and recall, making it robust across varying class distributions.


