# cluster-analysis-based-on-the-wine-dataset
Clustering Algorithms in Practice  
_by Jakub Nowacki_

1. **Dataset Description**  
The Red Wine Quality dataset contains information on 1599 varieties of Portuguese red wine. Each object in the dataset represents one wine and is described by 12 variables.

Attributes:

    fixed acidity: most acids involved with wine or fixed or nonvolatile
    volatile acidity: the amount of acetic acid in wine, which at high levels can lead to an unpleasant, vinegar taste
    citric acid: found in small quantities, citric acid can add "freshness" and flavor to wines
    residual sugar: the amount of sugar remaining after fermentation stops
    chlorides: the amount of salt in the wine
    free sulfur dioxide: prevents microbial growth and oxidation of wine
    total sulfur dioxide: amount of free and bound forms of SO2
    density: density
    pH: describes the acidity or basicity of the wine on a scale from 0 (very acidic) to 14 (very basic); most wines fall within the range of 3-4 on the pH scale.
    sulphates: additives to wine that can contribute to sulfur dioxide (SO2) levels, which acts as an antimicrobial and antioxidant.
    alcohol: alcohol content
    quality: rating of wine quality (from 0 to 10)

2. **Hierarchical Clustering**  
The chosen hierarchical clustering algorithm is the agglomerative hierarchical clustering (AHC) algorithm. The algorithm was run 6 times for different combinations of linkage methods and distance measures.

3. **Divisive Clustering**  
The chosen divisive clustering algorithm is the K-medoids algorithm. It was run 4 times for two distance measures - Euclidean and Cosine - and for two different numbers of clusters.

4. **Density-based Clustering**  
The DBSCAN algorithm was used for density-based clustering. It was run 4 times for two Epsilon values and two different MinPts values.

5. **Comparison of Algorithm Results**  

    **AHC:** Generally good results, especially with single linkage and Euclidean distance.  
    **K-medoids:** Very good results, especially with Euclidean distance and 5 clusters.  
    **DBSCAN:** Mixed results, often with a significant portion of the dataset treated as noise.  

In summary, the most effective results for the Red Wine Quality dataset were achieved using the AHC algorithm with Euclidean distance and single linkage, as well as the K-medoids algorithm, especially with Euclidean distance and 5 clusters.  

**Repository Contents**

    README.md: This file provides an overview of the report and code contained in the repository.

    cluster-analysis-based-on-the-wine-dataset-report.pdf: The detailed report outlining the analysis of clustering algorithms applied to the Red Wine Quality dataset. It includes descriptions of the dataset, explanations of the clustering algorithms used (hierarchical, divisive, and density-based), results of the clustering analysis, and a comparison of the performance of the different algorithms.

    cluster-analysis-based-on-the-wine-dataset.ipynb: Python script containing code for the clustering analysis. It includes implementations of hierarchical clustering, divisive clustering (K-medoids), and density-based clustering (DBSCAN). The script also includes functions for data preprocessing, clustering, and evaluation using the Davies-Bouldin index and silhouette scores.
