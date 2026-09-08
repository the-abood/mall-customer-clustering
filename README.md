# Mall Customer Segmentation Using Clustering

An unsupervised machine-learning project applying **K-Means, Agglomerative Hierarchical Clustering, and DBSCAN** to the Mall Customers dataset, with EDA, scaling, clustering evaluation, visual metric comparisons, and a second experiment on the Iris dataset.

## Assignment coverage

- Exploratory Data Analysis
- K-Means clustering
- Agglomerative Hierarchical Clustering
- DBSCAN
- Silhouette Score
- Calinski-Harabasz Index
- Davies-Bouldin Index
- Visual comparison of evaluation metrics
- Clustering on a second dataset (Iris)
- Post-hoc reference against Iris species labels

## Repository structure

```text
mall-customer-clustering-repository/
├── data/
│   └── Mall_Customers.csv       # place the dataset here
├── notebooks/
│   ├── Mall_Customer_Clustering_Analysis.ipynb
│   └── Mall_Customer_Clustering_Original.ipynb
├── reports/
├── src/
├── .gitignore
├── README.md
└── requirements.txt
```

## Dataset

The uploaded notebook referenced `Mall_Customers.csv`, but the CSV itself was not included with the notebook. Place the file in `data/` with this exact name:

`Mall_Customers.csv`

The cleaned notebook reads:

`../data/Mall_Customers.csv`

The second assignment dataset, Iris, is loaded directly from scikit-learn and therefore requires no additional download.

## Running the notebook

```bash
pip install -r requirements.txt
```

Then open:

`notebooks/Mall_Customer_Clustering_Analysis.ipynb`

and run the cells after placing `Mall_Customers.csv` in the `data/` folder.

## Key methodological fixes

- Portable dataset path for GitHub use.
- Clear preprocessing and feature-selection explanation.
- Reproducible K-Means configuration with `n_init=10`.
- Safe DBSCAN metric evaluation that excludes noise points.
- Avoids metric errors when an algorithm produces fewer than two valid clusters.
- Completes both assignment tasks with visual comparisons and interpretation.
