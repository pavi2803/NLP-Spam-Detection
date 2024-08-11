# Spam Filtering Project using NLP

## Overview

This project focuses on building a Spam Filter using Natural Language Processing (NLP) techniques. The dataset used contains SMS messages labeled as either "ham" (non-spam) or "spam." The primary objective is to preprocess the text data, analyze the patterns in spam and ham messages, and build a Bag of Words (BOW) model to distinguish between spam and non-spam messages.

## Dataset

The dataset contains SMS messages labeled as "ham" or "spam." It includes the following columns:

- **label**: Indicates whether the message is spam or ham.
- **message**: The content of the SMS message.

The dataset can be found in `spam.csv`.

## Requirements

- Python 3.x
- NumPy
- Pandas
- Matplotlib
- Seaborn
- NLTK
- WordCloud
- Scikit-learn

To install the required libraries, run:

```bash
bashCopy code
pip install numpy pandas matplotlib seaborn nltk wordcloud scikit-learn

```

## Project Structure

1. **Data Loading and Exploration**:
    - The dataset is loaded using Pandas, and basic exploration is conducted to understand the structure and distribution of the data.
2. **Data Visualization**:
    - Visualizations include pie charts to compare the distribution of spam and ham messages and histograms to analyze the frequency distribution of message lengths.
3. **Text Preprocessing**:
    - Removal of punctuation, stopwords, and non-alphabetic characters.
    - Tokenization and lemmatization of words.
4. **Word Cloud Visualization**:
    - Word clouds are generated to visualize the most common words in spam and ham messages.
5. **Bag of Words (BOW) Model**:
    - Creation of a BOW model using Scikit-learn's `CountVectorizer` to transform the text data into a matrix of token counts.

## Code Explanation

### Data Loading and Exploration

The dataset is loaded using `pd.read_csv()` and cleaned by dropping unnecessary columns. Basic statistics are computed using `describe()` and `groupby()` functions.

### Data Visualization

Pie charts and histograms are created to visualize the distribution of labels and message lengths. The most common messages are also identified.

### Text Preprocessing

The `text_preprocess` function performs the following steps:

1. Removal of punctuation.
2. Removal of stopwords.
3. Conversion of text to lowercase.
4. Filtering non-alphabetic words.

### Word Cloud Visualization

Word clouds for spam and ham messages are generated using the `WordCloud` library, providing a visual representation of the most frequent words.

### Bag of Words Model

The BOW model is created using Scikit-learn's `CountVectorizer`. The text data is transformed into a matrix of token counts, which can be used as features for machine learning models.

### Sample Output

- Top 10 spam and ham words.
- Visualization of the frequency distribution of message lengths.
- Word cloud visualizations.

## How to Run

1. Clone the repository and navigate to the project directory.
2. Ensure that the required Python libraries are installed.
3. Run the Jupyter notebook or Python script to execute the code.

```bash
bashCopy code
python spam_filtering_project.py

```

## Conclusion

This project demonstrates how to preprocess text data, visualize patterns in spam and ham messages, and create a Bag of Words model for spam filtering. The techniques used here can be extended to more complex text classification tasks.
