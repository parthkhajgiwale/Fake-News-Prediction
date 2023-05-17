# Fake News Prediction: Dataset

This repository contains a dataset and code for predicting fake news using machine learning techniques. The dataset consists of news articles with corresponding labels indicating whether the article is potentially unreliable (fake news) or reliable (real news).

## Dataset

The dataset includes the following fields:

- **id**: Unique ID for a news article.
- **title**: The title of a news article.
- **author**: The author of the news article.
- **text**: The text of the article, which may be incomplete.
- **label**: A label that marks the article as potentially unreliable.
    - `1` indicates fake news.
    - `0` indicates real news.

## Code

The code provided in this repository demonstrates how to build a fake news prediction model using logistic regression. Here's an overview of the code:

1. Import the necessary libraries and modules:
   - `pandas` for data manipulation and analysis.
   - `numpy` for numerical operations.
   - `re` for regular expressions.
   - `nltk` for natural language processing.
   - `sklearn` for machine learning algorithms and evaluation metrics.

2. Download the required NLTK stopwords.

3. Load the news dataset from the provided CSV file using `pd.read_csv`.

4. Perform data preprocessing:
   - Remove non-alphabetic characters and convert text to lowercase.
   - Tokenize the text and remove stopwords using stemming.

5. Separate the dataset into features (`X`) and labels (`Y`).

6. Create a TF-IDF vectorizer using `TfidfVectorizer` from sklearn.

7. Transform the textual data into numerical features using the TF-IDF vectorizer.

8. Split the dataset into training and testing sets using `train_test_split`.

9. Train a logistic regression model using `LogisticRegression`.

10. Evaluate the model's accuracy on the training data using `accuracy_score`.

11. Print the accuracy score of the test data.

12. Make predictions on a sample news article.

13. Print the prediction result.

## Usage

To use the code provided, follow these steps:

1. Install the required libraries mentioned in the code (if not already installed).

2. Download the dataset and place it in the appropriate directory.

3. Update the code to specify the correct path to the dataset file (`train.csv`).

4. Run the code to train the model and evaluate its performance.

5. Use the trained model to predict the reliability of new news articles.

Please note that this code serves as a starting point and can be further enhanced or customized based on specific requirements.
