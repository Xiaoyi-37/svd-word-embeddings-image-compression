# SVD for Word Embeddings and Image Compression

A statistical learning project exploring applications of **Singular Value Decomposition (SVD)** in word embeddings and image compression.

This project was completed for **MATH 308: Fundamentals of Statistical Learning** at McGill University.

## Overview

The project applies truncated SVD to two different problems:

- Learning low-dimensional word embeddings from a word co-occurrence matrix
- Compressing and reconstructing images using low-rank matrix approximations

The analysis focuses on how much information can be preserved when high-dimensional data are represented using a smaller number of singular components.

## Word Embeddings

A normalized word co-occurrence matrix was decomposed using SVD to construct low-dimensional word embeddings.

The analysis explored:

- Singular value decay and low-rank structure
- Interpretation of selected singular vectors
- Semantic similarity between words
- Gender-related directions and bias in embedding space
- Word analogy performance using cosine similarity
- Effects of different matrix transformations and embedding dimensions

The SVD-based embeddings achieved a **top-1 analogy accuracy of 0.5502** and a **top-5 accuracy of 0.7472**. Using `log(1 + M)` with embedding dimension 150 improved these results to **0.5783** and **0.7884**, respectively.

## Image Compression

SVD was also used to reconstruct an image using truncated low-rank approximations.

As the rank increased, more visual structure and detail were recovered. A rank-150 approximation retained the major structure of the image while requiring substantially less storage.

The rank-150 representation required approximately **22.2% of the storage** of the original image matrix, corresponding to about **4.5× greater memory efficiency**.

## Methods

Singular Value Decomposition · Low-Rank Approximation · Word Embeddings · Cosine Similarity · Image Compression

## Tools

R · Google Colab

## Repository Structure

```text
├── notebooks/
│   ├── word_embeddings.ipynb
│   └── image_compression.ipynb
└── README.md

## Collaboration

This project was completed collaboratively by ***Xiaoyi Xu & Jiaxuan Xu***.  
Most of the coding and implementation work was completed by **Xiaoyi Xu**.

## Note

The original assignment instructions and full submitted report are not included because the course restricts redistribution of instructor-generated materials, and the submitted report closely follows the original assignment structure. This repository therefore contains only a portfolio-oriented summary and selected notebooks.
