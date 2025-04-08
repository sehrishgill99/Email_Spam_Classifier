# SMS Spam Detection

A machine learning project to classify SMS messages as **Spam** or **Ham (Not Spam)** using natural language processing (NLP) techniques.

## Overview

This project uses a dataset of SMS messages to build a classifier that can detect spam messages. The primary goal is to process raw text data, extract meaningful features, and train a reliable machine learning model for spam detection.

## Dataset

The dataset used is `spam.csv.txt`, which contains the following columns:
- **v1**: Label (spam or ham)
- **v2**: The SMS text message


##   Primarily Language for Coding

- Python

# Libraries Used

- Pandas
- NumPy
- Scikit-learn
- Matplotlib & Seaborn (optional for Explotary Data Analysis(EDA))

## Project Workflow

1. **Data Loading**
   - Load the SMS dataset using Pandas.

2. **Data Cleaning**
   - Drop unnecessary columns.
   - Rename columns for clarity.
   - Handle missing values.
   - Remove Duplicates.

3. **Data Preprocessing**
   - Convert labels (`spam`, `ham`) to numerical format.
   - Perform text preprocessing (lowercasing, removing stopwords, Stemming etc.).

4. **Feature Extraction**
   - Use TF-IDF Vectorization to convert text data into numerical features.

5. **Model Building**
   - Train a **Multinomial Naive Bayes** classifier.Also tired on other ML algorithm like SVM, Random Forest and KNN but multinomial Naive Bayes gives the best precision and accuracy among the rest of the algorithm for model training.

6. **Model Evaluation**
   - Check accuracy score.
   - Generate confusion matrix.
   - Make sample predictions.

## Results

The model demonstrates good accuracy in classifying SMS messages as spam or ham. You can further improve performance by trying out other models or advanced NLP techniques

## How to Run

1. Clone this repository or download the notebook.
2. Install the required libraries:
   ```bash
   pip install pandas numpy scikit-learn matplotlib

## Additional Notes
I also tried running this project in PyCharm and developed an interactive version using Streamlit to explore web-based deployment and improve usability.For this purpose, meed to pip install streamlit,pip install nltk, pip install scikit-learn on Pycharm if it's not available.

## License
This Project is for education purposes.
