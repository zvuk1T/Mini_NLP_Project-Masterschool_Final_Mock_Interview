# Mini project

# Introduction

Before starting these task, please note that they are designed to fully prepare you for your upcoming mock interview. 

<aside>
🔥 You are expected to complete each step in a well-organized notebook, documenting all code, outputs, and explanations. During the interview, you’ll be asked to discuss your approach and build upon these solutions, so it is crucial that your work is detailed and clear.

</aside>

# **Task 4: Natural Language Processing (NLP)**

Natural Language Processing (NLP): Build an NLP pipeline for sentiment analysis using the IMDb dataset. This includes data preparation, text cleaning, converting text to numerical vectors, and training a classifier to predict sentiment.

1. Load and Prepare the Dataset
    - Download the IMDb dataset [here](https://drive.google.com/file/d/1yQQsg7ExFyJvVxzB9DQ5g_18kZV8dp0J/view?usp=drive_link).
    - Read the IMDb dataset from a CSV file.
    - Ensure that the dataset contains two essential columns: `review` (text reviews) and `sentiment` (labels indicating positive or negative sentiment).
2. Download Required NLTK Resources
    - Install, download and import necessary NLTK resources, including stopwords, wordnet, and punkt for text processing.
3. Preprocess the Text Data
    - Convert all text to lowercase.
    - Remove special characters and punctuation.
    - Tokenize the text into words.
    - Remove stopwords to filter out unimportant words.
    - Apply lemmatization to reduce words to their base form (e.g., "running" → "run").
    - Store the cleaned text in a new column named `cleaned_review`.
4. Convert Sentiment Labels to Numeric Format
    - Map `positive` reviews to `1` and `negative` reviews to `0`.
5. Split the Dataset into Training and Testing Sets
    - Divide the dataset into `80%` training data and `20%` testing data.
    - Use `train_test_split` from `sklearn.model_selection`.
6. Convert Text Data into Numerical Vectors
    - Use `TfidfVectorizer` to transform text into numerical representations for machine learning.
7. Train a Naive Bayes Classifier
    - Train a `MultinomialNB` model using the transformed text data.