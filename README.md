# LexRank-Summarization-on-Billsum-data
LexRank-Based Summarization and ROUGE Evaluation for BillSum Dataset

## Overview

This repository contains an implementation of the LexRank model for text summarization. The script processes legislative bill texts, generates extractive summaries, and evaluates their quality using ROUGE score metrics. Additionally, the script supports saving summaries to a JSONL file and visualizing ROUGE score trends across multiple datasets.

## Features
1. LexRank Summarization: Uses a graph-based ranking algorithm to extract key sentences from legislative texts.

2. ROUGE Score Evaluation: Computes ROUGE-1, ROUGE-2, and ROUGE-L scores to assess summary quality.

3. File Saving Support: Summarized outputs are stored in JSONL format.

4. Graphical Analysis: Generates ROUGE score trend graphs for different datasets.

5. Comparison Across Datasets: Evaluates summarization performance on US Train, US Test, and CA Test datasets.

## Installation
To run the script, install the required dependencies:


```bash
pip install pandas numpy networkx rouge-score scikit-learn nltk matplotlib
```

## Dataset Structure
Each dataset should be formatted as a JSONL file, with each line containing:

```bash
{
    "bill_id": "12345",
    "text": "Full text of the legislative bill...",
    "summary": "Reference summary..."
}
```

## Datasets Used
us_train_data.jsonl (US legislative bills - training set)

us_test_data.jsonl (US legislative bills - test set)

ca_test_data.jsonl (Canadian legislative bills - test set)

## Author
Developed for BillSum dataset summarization using LexRank by Sumit Sonar.

## License
This project is open-source and free to use.
