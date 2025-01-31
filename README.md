# Tweets-Classification-Using-NLP

Disaster Tweet Classification is a machine learning project designed to classify tweets as either disaster-related or non-disaster-related. This project demonstrates the use of natural language processing (NLP) techniques and machine learning models to assist emergency response teams in prioritizing and addressing critical information during disasters.

## Table of Contents
- [Overview](#overview)
- [Project Workflow](#project-workflow)
- [Features](#features)
- [Dataset](#dataset)
- [Models Used](#models-used)
- [Results](#results)
- [Installation](#installation)
- [Usage](#usage)
- [Future Work](#future-work)
- [Contributors](#contributors)
- [License](#license)

---

## Overview
The primary goal of this project is to classify tweets into two categories:
1. **Disaster**: Tweets that relate to real disaster events.
2. **Non-Disaster**: Tweets that are unrelated or do not provide relevant disaster information.

This classification is crucial for emergency services and organizations to quickly identify and act upon relevant information.

---

## Project Workflow
1. **Data Preprocessing**:
   - Cleaned text data by removing URLs, special characters, and irrelevant words.
   - Applied stemming to reduce words to their root forms.
   - Balanced the dataset using SMOTE (Synthetic Minority Oversampling Technique).

2. **Feature Extraction**:
   - Used TF-IDF vectorization to represent tweet text numerically.

3. **Model Training**:
   - Implemented Logistic Regression and Random Forest models.

4. **Evaluation**:
   - Assessed model performance using metrics such as accuracy, F1-score, precision, and recall.

---

## Features
- **Data Preprocessing**:
  - URL removal
  - Lowercasing
  - Stopword removal
  - Stemming

- **Class Balancing**:
  - Applied SMOTE to address class imbalance in disaster vs. non-disaster tweets.

- **Machine Learning Models**:
  - Logistic Regression
  - Random Forest

---

## Dataset
The dataset used in this project is sourced from the [Kaggle Competition - NLP Getting Started](https://www.kaggle.com/competitions/nlp-getting-started). It includes labeled tweets indicating whether they are related to disasters or not.

---

## Models Used
- **Logistic Regression**:
  - Accuracy: 79%
  - F1-Score: 0.75

- **Random Forest**:
  - Accuracy: 77%
  - F1-Score: 0.74

---

## Results
- **Best Model**: Logistic Regression outperformed Random Forest in terms of accuracy and F1-score.
- The project achieved strong balance between precision and recall for both disaster and non-disaster classes.

---

## Installation
To run this project locally, follow these steps:

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/disaster-tweet-classification.git
   cd disaster-tweet-classification
   ```

2. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Download the dataset from [Kaggle](https://www.kaggle.com/competitions/nlp-getting-started) and place it in the `/data` folder.

4. Run the preprocessing and model training script:
   ```bash
   python train.py
   ```

---

## Usage
1. Preprocess the dataset using the provided scripts.
2. Train the Logistic Regression or Random Forest models.
3. Use the trained model to classify new tweets as disaster-related or not.

---

## Future Work
- **Advanced Models**: Explore transformers like BERT for better text embeddings.
- **Additional Features**: Incorporate geolocation and timestamp data for more context.
- **Hyperparameter Tuning**: Optimize models for better performance.

---

## Contributors
- [Jewon Yeon](https://github.com/yeon971105)

---

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

This README provides a clear and comprehensive overview of your project, making it easy for others to understand and contribute.
