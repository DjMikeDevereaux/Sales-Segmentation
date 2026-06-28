# Sales-Segmentation
Sales and Segmentation  project  where the full data analysis workflow is integrated: cleaning, source integration, variable creation, exploratory analysis, and preparation for segmentatide Ventas y Segmentación EBAC – Data Science &amp; Business Analytics

## Project Goal
The main goal is to analyze the weekly sales behavior of a partner company by integrating multiple data sources (sales, products, categories, and segments) to:

Build a unified and clean dataset.
Generate time-based variables from weeks and years.
Carry out an exploratory data analysis (EDA) to identify relevant patterns.
Prepare the data for clustering techniques (K-Means).
Obtain actionable insights for the business.

## Technologies Used
Python 3 – Jupyter Notebook
Pandas for data manipulation
Seaborn / Matplotlib for visualization
scikit-learn for scaling, imputation, and clustering
Stats and metrics like silhouette_score
Excel / CSV as data sources

## Repository Structure

 Sales-Segmentation/
│── README.md
│── data/
│     ├── FACT_SALES.csv
│     ├── DIM_PRODUCT.xlsx
│     ├── DIM_SEGMENT.xlsx
│     └── DIM_CATEGORY.csv
│── notebooks/
│     └── Sales-Segmentation.ipynb
│── outputs/
│     ├── graficas/
│     └── clustering/

Data Integration
The following sources were loaded:

FACT_SALES.csv – Weekly sales by product
DIM_PRODUCT.xlsx – Product information
DIM_SEGMENT.xlsx – Segmentation attributes
DIM_CATEGORY.csv – Main categories

## Integration Process
Conversion of WEEK to actual date
  Separation of week and year
  Normalization of years (2 digits → 4 digits)
  Construction of base date
  Adding weeks to get DATE
Merge 1: Product + Segment
Merge 2: Add up sales by ITEM

The result is a consolidated dataset with:
  Product information
  Segmentation attributes
  Weekly sales
  Exact date
  Region
  Category and format

## Exploratory Analysis (EDA)
EDA includes:

  Sales distributions
  Outlier identification
  Weekly trends
  Behavior by category, brand, and segment
  Correlations between numerical variables

Examples of questions analyzed:

  Which categories generate the highest sales volume?
  Which brands show the most weekly variability?
  Are there seasonal patterns by week or month?
  Which segments show differentiated behaviors?

Preparation for Modeling (K-Means)
The following steps were carried out:

  Selection of relevant variables
  Imputation of missing values
  Scaling with StandardScaler
  Evaluation of optimal number of clusters
  Calculation of silhouette score

The goal is to identify groups of products with similar behaviors to support decisions on:

  Portfolio
  Promotions
  Distribution
  Segment-specific strategies

Main Results
  Includes:
  Distribution charts
  Trends by category
  Correlation heatmaps
  Clustering results
  Interpretation of each cluster

Business Conclusions

  Identification of key categories for growth
  Segments with the greatest potential
  Products with unusual behavior
  Recommendations for optimizing inventory or promotions


