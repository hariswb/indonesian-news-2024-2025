# Jupyter Notebook - Vectorize Indonesian News

A jupyter notebook for vectorizing indonesian news using Scikit Learn's TF-IDF.

## Input

News title in Indonesian.

## Output

- 1000 Dimension vector.
- Manifest JSON `out/manifest.json`
- Data type: float32
- Output Shards: every 10k vectors
- Roughly 32Mb/shard

## Preprocess

It includes:
- Replace acronyms
- Lowercase
- Remove HTML image tags
- Remove mentions, URLs, numbers
- Clean punctuation and excess whitespace
- Remove specific unwanted terms

## Vectorizing

Uses Scikit-Learn's TF-IDF with stop words

## Dataset

[Indonesia News January 2024 - October 2025 by Sh1zuka](https://www.kaggle.com/datasets/sh1zuka/indonesia-news-dataset-2024)

Note: This data is not included in this repo.
