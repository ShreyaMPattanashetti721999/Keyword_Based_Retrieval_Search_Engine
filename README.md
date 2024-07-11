# Keyword-Based Retrieval Search Engine

This project implements a keyword-based retrieval search engine that indexes Wikipedia articles. The engine uses a Vector Space Model (VSM) enhanced with K-Means clustering to facilitate efficient and precise information retrieval.

## Table of Contents
- [Overview](#overview)
- [Aim](#aim)
- [Task and Dataset](#task-and-dataset)
- [Architecture](#architecture)
- [Data Preprocessing](#data-preprocessing)
- [Clustering](#clustering)
- [Search Function](#search-function)
- [Evaluation](#evaluation)
- [Comparison of Retrieval Models](#comparison-of-retrieval-models)
- [Installation](#installation)
- [Usage](#usage)
- [References](#references)

## Overview
This project is developed by Group 13, comprising Abhishek Vijaykumar Mane, Andrew Graham Porter, Mohammad Asghar, and Shreya Murigendra Pattanashetti. It focuses on designing and implementing a sophisticated search engine to index Wikipedia articles for efficient keyword-based searches.

## Aim
The objective is to develop a sophisticated search engine that indexes Wikipedia articles for precise and efficient information retrieval.

## Task and Dataset
- **Task**: Create a streamlined indexing framework using 'wiki-articles.json'. This includes implementing a foundational Vector Space Model (VSM) enhanced with K-Means clustering.
- **Dataset**: The dataset consists of Wikipedia articles with fields: ID, URL, title, and body text.

## Architecture
The search engine architecture incorporates several key components:
1. **Document Loading**
2. **Preprocessing**:
    - Tokenization
    - Stop Words Removal
    - Lemmatization
    - Stemming
3. **Clustering**:
    - K-Means
4. **Vectorization**:
    - TF-IDF
5. **Dimensionality Reduction**:
    - SVD
6. **Index Creation**
7. **Query Processing**:
    - Vectorization
    - Dimensionality Reduction
    - Relevant Cluster Retrieval

## Data Preprocessing
- **Tokenization**: Breaking text into words or tokens.
- **Stop Words Removal**: Removing common words with minimal semantic value.
- **Lemmatization**: Converting words to their base form.
- **Stemming**: Trimming words to their root form.
- **TF-IDF Vectorization**: Transforming text into vectors.
- **Dimensionality Reduction (SVD)**: Simplifying features to the most significant ones.

## Clustering
- **Spherical K-Means**: Used for clustering documents.
- **Silhouette Score**: Used to determine optimal clusters.

## Search Function
1. **Query Vectorization**
2. **Dimensionality Reduction of Query**
3. **Compute Similarities to Cluster Centroids**
4. **Identify Most Relevant Cluster**
5. **Compute Similarities to Documents in the Cluster**
6. **Retrieve Most Similar Documents**

## Evaluation
- **Silhouette Coefficient**: Used to measure cluster quality.
- **Comparison Metrics**:
    - Efficiency of VSM vs. BM25 models
    - Relevance of search results

## Comparison of Retrieval Models
- **Efficiency**: Runtime comparison
- **Effectiveness**: Mean Average Precision (mAP)

## Installation
1. Clone the repository:
    ```bash
    git clone https://github.com/yourusername/keyword-based-retrieval-search-engine.git
    ```
2. Navigate to the project directory:
    ```bash
    cd keyword-based-retrieval-search-engine
    ```
3. Install the required dependencies:
    ```bash
    pip install -r requirements.txt
    ```

## Usage
1. Preprocess the data and build the index:
    ```bash
    python preprocess_and_index.py
    ```
2. Perform a search query:
    ```bash
    python search.py "Your query here"
    ```

## References
- Cambridge University Press (2008) Tokenization. Available at: https://nlp.stanford.edu/IR-book/html/htmledition/tokenization-1.html
- Hornik et al. (2012) Spherical k-means clustering. Journal of Statistical Software.
- Huang, A. (2008) Similarity measures for text document clustering.
- Otten, N.V. (2023) Text normalization techniques in NLP with Python.
- Salton et al. (1975) A vector space model for automatic indexing. Communications of the ACM.
- Zhang, Q. (2024) Indexing and TF-IDF. Queen Mary University of London.
- Zhong, S. (2005) Efficient online spherical k-means clustering.

