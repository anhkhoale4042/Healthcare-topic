# Vietnamese Medical QA Topic Extraction 

This project performs topic clustering on a Vietnamese medical Q&A dataset using K-Means and BERTopic.

## Overview
- **Dataset:** [hungnm/vietnamese-medical-qa](https://huggingface.co/datasets/hungnm/vietnamese-medical-qa)
- **Goal:** Discover common medical topics in user questions
- **Methods:** Text preprocessing, tokenization, embedding, clustering, and topic labeling

## Pipeline
- **Preprocessing:** remove emojis, greetings, and special characters  
- **Tokenization:** segment Vietnamese words using Underthesea and remove stopwords  
- **Embedding:** use `keepitreal/vietnamese-sbert` to generate sentence vectors  
- **Clustering:** apply both K-Means and BERTopic (UMAP + HDBSCAN)  
- **Topic Labeling:** extract top keywords for each cluster using TF-IDF  

## Results
- **KMeans:** 18 clusters with moderate separation  
- **BERTopic:** 20 well-defined topics related to common medical issues
