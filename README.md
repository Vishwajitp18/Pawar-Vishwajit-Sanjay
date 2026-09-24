# EDA Course Project

**Name:** Pawar Vishwajit Sanjay
**Registration Number:** 23BDS0192  
**Institution:** Vellore Institute of Technology (VIT)

---

## Project Overview

This repository contains the implementation and documentation for the **Exploratory Data Analysis (EDA) Course Project**. The project focuses on analyzing the `Fertility2.csv` dataset using Python and various data science techniques, including data preprocessing, statistical analysis, data visualization, correlation analysis, and clustering.

The project is divided into two phases, covering both fundamental and advanced exploratory data analysis techniques.

---

## Libraries Used

- `pandas` & `numpy`: Data manipulation, preprocessing, and numerical calculations.
- `matplotlib.pyplot` & `seaborn`: Data visualization and statistical plotting.
- `scipy.stats`: Statistical analysis, correlation tests, t-tests, and chi-square tests.
- `mpl_toolkits.mplot3d`: Three-dimensional data visualization.
- `sklearn.preprocessing`: Data standardization and preprocessing.
- `sklearn.cluster`: K-Means clustering.
- `scipy.cluster.hierarchy`: Hierarchical clustering and dendrogram generation.
- `sklearn.metrics`: Silhouette score for cluster evaluation.

---

# Phase 1: Data Preprocessing and Initial EDA

The objective of this phase is to understand the structure of the `Fertility2.csv` dataset, perform the necessary preprocessing, and explore the underlying patterns using descriptive statistics and visualizations.

### Tasks Completed in Phase 1

1. **Loading the Dataset:** Imported the `Fertility2.csv` dataset directly from the GitHub raw URL using Pandas.

2. **Dataset Inspection:**
   - Examined the first few records using `.head()`.
   - Checked the number of rows and columns.
   - Inspected column names and data types.
   - Generated descriptive statistical summaries using `.describe()`.
   - Checked for missing values.

3. **Data Understanding:**
   - Identified numerical and categorical/binary variables.
   - Examined the distribution and frequency of individual variables.
   - Treated the `rownames` column as an identifier rather than an analytical feature.

4. **Descriptive Statistical Analysis:**
   - Calculated mean, median, mode, variance, and standard deviation.
   - Calculated minimum, maximum, range, and quartiles for numerical variables.

5. **Univariate Analysis:**
   - Generated histograms to study numerical distributions.
   - Used boxplots to examine spread and possible outliers.
   - Created frequency tables and bar plots for categorical/binary variables.

6. **Bivariate Exploration:**
   - Examined relationships between numerical and binary variables.
   - Used scatter plots and boxplots to visualize relationships between variables.

---

# Phase 2: Statistical Analysis & Clustering

The objective of this phase is to perform comprehensive **1D, 2D, and 3D statistical analyses**, followed by **K-Means and Hierarchical clustering** to identify patterns and groupings within the Fertility dataset.

### Tasks Completed in Phase 2

1. **1D Statistical Analysis:**  
   Computed descriptive statistics including mean, median, mode, variance, standard deviation, minimum, maximum, range, and quartiles. Visualized individual variable distributions using histograms, boxplots, frequency tables, and bar charts.

2. **2D Statistical Analysis:**  
   Analyzed relationships between pairs of variables using scatter plots, correlation analysis, boxplots, contingency tables, and statistical hypothesis testing. Pearson correlation and independent t-tests were used for numerical/binary relationships, while chi-square testing was used to examine associations between categorical variables.

3. **3D Statistical Analysis:**  
   Constructed a 3D scatter plot using `mpl_toolkits.mplot3d` to visualize the simultaneous relationship among **Age, Work, and More Kids**.

4. **Correlation & Multivariate Analysis:**  
   Generated a complete correlation matrix for the numerical/binary variables and visualized the relationships using a Seaborn heatmap. Pair plots were also generated to examine relationships across multiple variables.

5. **Data Standardization:**  
   Standardized the clustering features using `StandardScaler` so that variables with different scales would contribute appropriately to distance-based clustering methods.

6. **K-Means Clustering:**  
   Applied the K-Means clustering algorithm to the standardized dataset. Calculated **Within-Cluster Sum of Squares (WCSS)** for different values of K and generated an **Elbow Plot** to assist in selecting the number of clusters. Cluster assignments, cluster centers, and cluster sizes were analyzed.

7. **Cluster Evaluation:**  
   Calculated the **Silhouette Score** to evaluate the quality and separation of the generated K-Means clusters.

8. **Hierarchical Clustering:**  
   Performed hierarchical clustering using **Euclidean distance** and **Single Linkage**. Generated a dendrogram to visualize the hierarchical grouping of observations and divided the dataset into three clusters.

9. **Cluster Comparison:**  
   Compared the cluster assignments obtained from K-Means and Hierarchical Clustering using a cross-tabulation of cluster memberships.

---

## Dataset

The analysis is performed on the **Fertility2.csv** dataset.

### Variables Used

| Variable | Description |
|----------|-------------|
| `rownames` | Row identifier |
| `morekids` | Indicator for having more children |
| `gender1` | Gender indicator for first child |
| `gender2` | Gender indicator for second child |
| `age` | Age |
| `afam` | African-American indicator |
| `hispanic` | Hispanic indicator |
| `other` | Other ethnicity indicator |
| `work` | Work/employment indicator |

### Dataset Source

[Fertility2.csv](https://raw.githubusercontent.com/salemprakash/EDA/main/Data/Fertility2.csv)

---

## Project Notebooks

### Phase 1

[Open Phase 1 EDA Notebook](./Phase_1_EDA_Project.ipynb)

### Phase 2

[Open Phase 2 Statistical Analysis & Clustering Notebook](./EDA_PhaseII.ipynb)

---

## Analysis Workflow

```text
Fertility Dataset
       ↓
Data Loading & Inspection
       ↓
Data Preprocessing
       ↓
Descriptive Statistics
       ↓
1D Statistical Analysis
       ↓
2D Statistical Analysis
       ↓
3D Statistical Analysis
       ↓
Correlation & Hypothesis Testing
       ↓
Data Standardization
       ↓
K-Means Clustering
       ↓
Hierarchical Clustering
       ↓
Cluster Evaluation & Comparison
