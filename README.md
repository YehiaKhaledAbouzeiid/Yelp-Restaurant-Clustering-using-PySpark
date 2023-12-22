# Yelp Restaurant Clustering using PySpark

## Overview

This project employs PySpark for clustering Yelp restaurant data, with a focus on grouping similar restaurants based on various features. The primary clustering algorithm utilized is K-Means, complemented by data preprocessing, one-hot encoding, and visualization techniques. The analysis aims to provide insights into restaurant patterns and relationships within the dataset.

## Prerequisites

Ensure you have the following installed:

- Apache Spark
- PySpark
- Python 3.x
- Jupyter Notebook

## Getting Started

1. **Install Dependencies:**
   - Install the necessary dependencies using the following command:

     ```bash
     pip install pyspark numpy scipy pandas matplotlib scikit-learn
     ```

2. **Dataset:**
   - Download the Yelp restaurant dataset in CSV format and save it in the project directory. The provided notebook assumes the dataset is named `Food2.csv`.

3. **Run the Notebook:**
   - Open the Jupyter Notebook and execute each cell step by step. Adjust the `csv_path` variable if your dataset has a different name or location.

## Code Description

The notebook is structured as follows:

- **Data Loading and Exploration:**
  - The Yelp restaurant dataset is loaded into a PySpark DataFrame, and basic exploratory operations are performed.

- **Data Preprocessing:**
  - String columns are indexed using `StringIndexer`, and one-hot encoding is applied to transform categorical variables into numerical format.

- **Feature Engineering:**
  - Remaining string columns are converted to `DoubleType`, and a `VectorAssembler` is used to create a feature vector for clustering.

- **K-Means Clustering:**
  - The K-Means clustering algorithm is applied using PySpark's `KMeans` implementation. The number of clusters (`knum`) is set to 5.

- **Visualization:**
  - Cluster distribution is visualized using bar charts and pie charts. Additionally, Principal Component Analysis (PCA) is employed for dimensionality reduction and scatter plot visualization.

# 

## 

* 
* 
