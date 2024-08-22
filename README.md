# Sentiment Analysis in Python

This project demonstrates sentiment analysis in Python using two different techniques:

1. **VADER (Valence Aware Dictionary and sEntiment Reasoner)** - A bag-of-words approach that evaluates the sentiment of text by summing the intensity of individual words.
2. **Roberta Pretrained Model from 🤗 Huggingface** - A transformer model that accounts for context and relationships between words.


## Project Overview

### Dataset

The dataset used in this project is the **Amazon Fine Food Reviews** dataset, which contains over 500,000 food reviews. You can find and download the dataset from [Kaggle](https://www.kaggle.com/datasets/snap/amazon-fine-food-reviews).

### Step 0: Read in Data and NLTK Basics
- Loaded the Amazon Fine Food Reviews dataset.
- Performed basic Exploratory Data Analysis (EDA) to understand the distribution of review scores.
- Utilized NLTK for tokenizing and part-of-speech tagging on sample review text.

### Step 1: VADER Sentiment Scoring
- Used NLTK's `SentimentIntensityAnalyzer` to calculate sentiment scores (negative, neutral, positive, and compound) for the text.
- Applied the VADER model on the entire dataset and visualized the results using Seaborn.

### Step 2: Roberta Pretrained Model
- Leveraged the `cardiffnlp/twitter-roberta-base-sentiment` model from Huggingface to evaluate sentiment.
- Compared the results of the Roberta model with the VADER scores.

### Step 3: Combining and Comparing Results
- Merged VADER and Roberta sentiment scores into a single DataFrame.
- Visualized the differences between the two models across the dataset using pair plots.

### Step 4: Review Examples
- Analyzed instances where the sentiment scores differed significantly from the actual review scores.
- Highlighted reviews with high positive sentiment but low review scores, and vice versa.

### Huggingface Transformers Pipeline
- Demonstrated the use of the Huggingface `pipeline` for quick sentiment analysis with default models.

## What Did I Learn?

Through this project, I learned:

**Text Preprocessing:** The importance of text preprocessing and tokenization in Natural Language Processing (NLP) tasks.
**Sentiment Analysis Techniques:** How to apply and compare different sentiment analysis models, including a bag-of-words approach (VADER) and a transformer-based model (Roberta).
**Model Comparison:** How to combine and compare the results from different models to better understand their performance on real-world data.
**Visualization:** The significance of visualizing data to derive insights and communicate findings effectively.
**Transformers and Huggingface:** How to use state-of-the-art NLP models from the Huggingface library for various tasks, including sentiment analysis.


