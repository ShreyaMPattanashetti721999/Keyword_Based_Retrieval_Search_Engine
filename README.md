# Keyword-Based Retrieval Search Engine

This repository contains the implementation of a sophisticated search engine that indexes Wikipedia articles for precise and efficient information retrieval. It enhances text analysis and retrieval capabilities, improving scalability across extensive textual content.

## Overview

This project builds a streamlined indexing framework using the `wiki-articles-small.json` dataset. The foundation is the Vector Space Model (VSM) enhanced with K-Means clustering to enable efficient keyword-based searches by cataloging word occurrences.

### Features

- **Data Preprocessing:** Includes tokenization, stop word removal, lemmatization, and stemming.
- **Vectorization:** Uses TF-IDF to transform text into vectors.
- **Dimensionality Reduction:** Implements SVD to simplify features.
- **Clustering:** Applies K-Means to group similar documents, enhancing search efficiency.
- **Search Functionality:** Allows for keyword-based querying with refined search results based on cluster analysis.

### Architecture

The general architecture involves the following steps:
1. **Document Loading**
2. **Preprocessing** (Tokenization, Stop Words Removal, Lemmatization, Stemming)
3. **Vectorization** (TF-IDF)
4. **Dimensionality Reduction** (SVD)
5. **Clustering** (K-Means)
6. **Index Creation**
7. **Query Processing** (Vectorization, Reduction, Relevant Cluster Retrieval)

## Usage

Run the Jupyter notebooks (`BM25_Comparison_Search_Engine.ipynb` and `VSM_Search_Engine.ipynb`) to see the implementation and comparison of the search models.

## Evaluation

The system is evaluated using the Silhouette Coefficient to determine the optimal number of clusters and the mean average precision (mAP) to assess the retrieval effectiveness.

## Contribution

Contributions are welcome! For major changes, please open an issue first to discuss what you would like to change.

## License

Distributed under the MIT License. See `LICENSE` for more information.

## References

Tokenization and text preprocessing techniques referenced from Cambridge University Press and various academic papers listed in the repository.

