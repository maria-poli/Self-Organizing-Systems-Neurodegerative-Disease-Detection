# Self Organizing Systems Neurodegerative Disease Detection

## Introduction
This repository explores Self-Organizing Systems for neurodegenerative disease detection, specifically focusing on Alzheimer's disease (AD) and Huntingon's disease (HD) classification using gene expression data (GSE33000). The project implements two complementary approaches: Artificial Immune System (AIS) algorithms and Self-Organizing Maps (SoMs). These bio-inspired computational methods are evaluated for their ability to identify disease patterns in genetic datasets, yielding competitive results and performance compared to conventional machine learning techniques.

## Setup

### Install Dependencies
```bash
pip install -r requirements.txt
```

### Unzip the Dataset
```bash
unzip GSE33000_Top10000_Var.zip
```

## Artifical Immune System

### AIS-clonal-selection.ipynb
This Notebook implements the Clonal Selection Algorithm (CSA) for optimization problems. It demonstrates how to utilize the principles of immune system clonal selection to enhance the search for optimal solutions. The notebook includes detailed explanations of the algorithm's steps, parameter tuning, and performance evaluation.

### AIS-competitive.ipynb
This notebook explores the Competitive Selection Algorithm, an approach that comes as an extension to the previous code. It focuses on the competitive mechanisms that drive the selection of solutions inside the detectors' population. Affinity measure is changed from euclidean distance to cosine similarity to better suit the genetic data.

### AIS-best-cross-check.ipynb
This notebook designs the best found framework for this usecase. is designed to validate and compare the results obtained from different AIS algorithms. It adds robustness but not relying on sole samples, but their neighborhoods and k-NN smoothing. At the end of this notebook, a cross-dissease generalization was attempted but because there was no dataset found that used a similar genetic probe measurement for another neurodegenerative disease, GSE44770 was chosen, a later dataset also based on Alzheimer's disease samples, making this a temporal-cross generalization.  

## Self Organizing Maps

### SoM-cluster-classification.ipynb
This Notebook implements unsupervised clustering techniques using Self-Organizing Maps (SoMs) and an indirect extiension for a classification task. It demonstrates how to preprocess data, train the SoM, and visualize the clustering results. The notebook includes examples of applying SoMs, highlighting their effectiveness in identifying patterns and classifying data points based on learned features.

### SoM-deep-learning.ipynb
The SoM-deep-learning notebook explores the integration of Self-Organizing Maps with deep learning methodologies. It discusses how deep learning techniques (Encoders) can assist SoMs, enhancing feature extraction and representation learning. The notebook provides insights into the architecture, training process, and performance evaluation of deep learning models that leverage SoMs for improved clustering visualizations.
>>>>>>> 97c2be1 (Updated ReadMe file)
