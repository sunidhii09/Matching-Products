# Entity Matching System

This system uses TF-IDF with cosine similarity, for finding matching products across two e-commerce platforms: Amazon and Flipkart by Named Entity Recognition (NER) on the input text using a predefined NER pipeline. The process involves data preprocessing, calculating text similarities using TF-IDF cosine similarity, and identifying matching products based on a defined similarity threshold.

## Data Preprocessing

Data preprocessing was essential to handle the diverse nature of data types and formats in both datasets. The following steps were applied:

- **Lowercasing:** Converting all text to lowercase for standardization.
- **Tokenization:** Breaking down text into individual words.
- **Stopwords Removal:** Removing common words that carry little significance.
- **Stemming and Lemmatization:** Reducing words to their root forms.
- **Special Characters and Numbers Removal:** Removing special characters and numerical values for uniformity.

## Matching Algorithm

The matching algorithm used for entity resolution included:

- **TF-IDF Vectorization:** Transforming product descriptions into TF-IDF vectors.
- **Cosine Similarity Calculation:** Measuring the similarity between product descriptions using cosine similarity.
- **Thresholding:** Identifying matches based on a similarity threshold.

## Analysis

The algorithm successfully identified matching products, but some mismatches occurred due to:

- **Semantic Variations:** Differences in terminology and product descriptions.
- **Data Quality Issues:** Incomplete or inaccurate data.
- **Threshold Sensitivity:** Impact of similarity threshold on matching accuracy.

## Challenges and Solutions

- **Data Heterogeneity:** Addressed by applying robust preprocessing techniques.
- **Computational Efficiency:** Enhanced through parallel and batch processing.
- **Parameter Tuning:** Iteratively refined similarity thresholds for optimal performance.

Despite challenges, the system effectively matched products between datasets, providing a framework for further improvement and application in real-world scenarios.

