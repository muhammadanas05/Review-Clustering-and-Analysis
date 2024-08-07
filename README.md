# Review Clustering and Analysis

This repository contains a Python script for analyzing and clustering customer reviews using natural language processing (NLP) techniques. The script focuses on filtering and preprocessing negative reviews, vectorizing them using TF-IDF, and applying K-means clustering to identify common themes.

## Requirements

- Python 3.x
- Pandas
- Numpy
- Scikit-learn
- NLTK

You can install the required packages using pip:

```bash
pip install pandas numpy scikit-learn nltk
```

## Data

The script uses a dataset named `reviews.csv`. Ensure this file is located in the same directory as the script.

## Analysis Overview

### Load the Data

- Loads the customer reviews data from `reviews.csv`.

### Filter Negative Reviews

- Filters out reviews with scores of 1 or 2 to focus on negative feedback.

### Preprocess the Reviews

- Defines a function to preprocess text by tokenizing, converting to lowercase, removing non-alphabetic tokens, and eliminating stopwords.
- Applies this preprocessing to the negative reviews to clean the text.

### Vectorize the Cleaned Reviews

- Uses TF-IDF (Term Frequency-Inverse Document Frequency) to convert the cleaned review text into numerical features suitable for clustering.

### Apply K-means Clustering

- Applies K-means clustering to group the negative reviews into 5 clusters based on their TF-IDF features.

### Find the Most Frequent Terms in Each Cluster

- Defines a function to extract the top terms from each cluster.
- Identifies and counts the most frequent terms in each cluster and displays them.

## Results

- Outputs the preprocessed reviews and a DataFrame containing the most frequent terms in each cluster along with their frequencies.



Feel free to adjust the content based on any additional details or specific instructions for your project.
