# Fraudulent Financial Transactions Detection

##University of Wollongong - Big Data Analytics Assignment

## Overview

This project, undertaken as part of the Big Data Analytics assignment at the University of Wollongong, is dedicated to the analysis of a synthetic transactional dataset. The dataset, sourced from Kaggle and resized for practicality (details available in the `data` folder), serves as the focal point for detecting fraudulent financial transactions.

### Project Objectives

- Analyze the network of money flow within mobile money services.
- Investigate transaction times, frequencies, and amounts for both fraudulent and normal accounts.
- Identify key factors influencing fraud detection.
- Propose early financial warning strategies from the perspective of the financial service provider.

### Dataset Details

The dataset is generated using PaySim, a simulator that utilizes aggregated data from real transactions extracted from one month of financial logs of a mobile money service in an African country. Provided by a multinational company offering mobile financial services across 14 countries worldwide, PaySim aims to simulate normal transaction operations while injecting malicious behavior for evaluating fraud detection methods.

### Dataset Scaling

To facilitate practical usage, the synthetic dataset has been scaled down to 1/4 of the original size specifically for Kaggle. For Assignment 3, a further reduction of 85% has been applied, allowing for easier handling and analysis.

## Project Structure

- **dataset**: Contains the dataset file (A3dataset.csv) and data description(data description.pdf).
- **analysis_notebooks**: Includes the Jupyter Notebook for analysis (Fraudulent Financial Transactions Detection.ipynb).
- **assignment_spec**: Holds the assignment specification document (Assignment 3 task sheet.pdf).
- **reference**: Contains the reference essay that explores the analysis of large-scale complex networks in banking transcations. (The Banking Transactions Dataset and its Comparative Analysis with Scale-free Networks.pdf).

## Key Findings

- Fraudulent transactions occur primarily in CASH-OUT and TRANSFER transactions.
- Fraudulent transactions often involve significantly larger amounts compared to normal transactions.
- The total transaction amounts of fraudulent transactions are notably higher than those of normal transactions.

## Models and Algorithms

We designed and implemented several models and algorithms based on analytical results:

1. **K-means:**
   - Used for classifying unlabelled data.
   - Successfully divided data into two clusters of similar sizes.

2. **Graph Algorithms:**
   - Node Classification by node2vec, node Classification by embeddings, and node Classification by GCN.
   - Achieved 93% accuracy on test sets with node Classification embeddings, but faced challenges with GCN.

3. **Artificial Neural Networks (ANN):**
   - Adopted for better results over balanced sample data.

4. **Classification Algorithms:**
   - Random Forest and eXtreme Gradient Boosting Trees (XGB Trees).
   - Demonstrated good performance with both Random Forest and XGB Trees.

## Data Preprocessing

Due to the highly unbalanced nature of the dataset, we addressed the data imbalance issue using sampling methods during preprocessing. However, it's important to note that the dataset's incompleteness and bias may impact our analysis and models.

## Instructions

To reproduce the analysis or explore the project, follow the steps outlined in the Jupyter Notebook (`Fraudulent Financial Transactions Detection.ipynb`). Refer to the assignment specification document for additional details.

## Acknowledgments

Special thanks to Kaggle for providing the synthetic dataset and PaySim for their contribution to simulating mobile money transactions.

---

Feel free to customize the structure and content based on your specific details. This template provides a starting point for your README, making it informative and user-friendly for anyone visiting your GitHub repository.
