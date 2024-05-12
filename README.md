# NLP Tasks in Python

This repository contains Python code for performing various Natural Language Processing (NLP) tasks using the Gensim library and pre-trained word2vec models.

 The tasks include generating lists of similar words, analyzing polysemous words, comparing synonyms and antonyms, examining the effects of different corpora, and plotting word vectors in 2D.

## Requirements

- Python 3.x
- Gensim library
- NumPy library
- Matplotlib library
- scikit-learn library

## Installation

1. Install Python 3.x from the official website: https://www.python.org/downloads/

2. Install the required libraries using pip:
pip install gensim numpy matplotlib scikit-learn
## Tasks

### 1. Generating Lists of Similar Words

This task demonstrates how to load a pre-trained word2vec model and generate lists of the most similar words for a given set of words. The code retrieves the top 20 similar words for each word in the `chosen_words` list and prints them along with their similarity scores.

### 2. Analyzing Polysemous Words

Polysemous words are words that have multiple meanings. This task analyzes a set of polysemous words and their top-10 neighbors to determine if the neighbors reflect the different meanings of the words. The code defines two groups of polysemous words and uses the `analyze_words` function to retrieve and print the top-10 neighbors for each word.

### 3. Comparing Synonyms and Antonyms

This task compares the similarity scores between a word and its synonym and antonym using the word2vec model. The code calculates the similarity scores between the word pairs and prints the results.

### 4. Examining the Effects of Different Corpora

This task explores the impact of using different corpora for training word2vec models. It loads two pre-trained models: one trained on Wikipedia and news data, and another trained on Twitter data. The code defines a list of words to test and calculates the average similarity between the top-10 neighbors of each word in both models. It then identifies the words whose neighbors are most similar and most different between the two corpora.

### 5. Plotting Word Vectors in 2D

This task demonstrates how to visualize word vectors in a 2D space using Principal Component Analysis (PCA). The code filters the first 5000 words from the model's vocabulary, keeping only those ending with 'ed' or 'ing'. It then applies PCA to reduce the dimensionality of the word vectors to 2D and plots the words using different colors based on their suffixes.
