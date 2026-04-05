# Customer Segmentation: Multi-Algorithmic Clustering Analysis

## Project Overview

This project focuses on identifying distinct customer segments within a retail environment using advanced unsupervised machine learning techniques. By analyzing Annual Income and Spending Behavior, we move beyond broad demographics to understand the underlying behavioral patterns of shoppers.

To ensure the highest level of accuracy and cluster stability, this project utilizes a dual-model approach, comparing K-Means Clustering and Agglomerative Hierarchical Clustering, optimized via Principal Component Analysis (PCA).

## The Business Question

"How can we segment customers based on income and spending behavior to improve targeted marketing strategies?"

By answering this, the project provides a data-driven roadmap for marketing teams to transition from "mass-marketing" to "personalized engagement," ensuring that promotional budgets are allocated to the segments where they will yield the highest ROI.

## Key Features & Technical Workflow

1. Dimensionality Reduction: Implementation of PCA to reduce noise and concentrate variance, ensuring more defined cluster boundaries.
2. Dual-Algorithm Approach:  K-Means: For efficient, centroid-based partitioning.
3. Hierarchical Clustering: Utilizing Ward's Linkage and Dendrograms to visualize the natural hierarchy of the data.

### Statistical Validation: Both models were rigorously evaluated using:

1. Silhouette Score (Measure of cluster separation)

2. Davies-Bouldin Index (Measure of cluster tightness)

3. Calinski-Harabasz Score (Variance ratio criterion)

### Inference Pipeline: A dedicated system to process new, unseen customer data and automatically assign them to a business persona.

## Business Personas Identified

The analysis successfully categorized customers into **five actionable segments:**

- Premium: High Income, High Spending (Loyalty focus).

- Untapped Potential: High Income, Low Spending (Luxury awareness focus).

- Balanced: Average Income, Average Spending (Consistency focus).

- Promotion-Driven: Low Income, High Spending (Flash-sale focus).

- Budget: Low Income, Low Spending (Value-proposition focus).

## Model Performance Highlights

Both models showed high consistency, proving the robustness of the segments:

- K-Means Silhouette Score: 0.550

- Hierarchical Silhouette Score: 0.554

- Davies-Bouldin Index: ~0.57 (Indicates excellent separation)

## Why This Matters

In the modern retail landscape, "one-size-fits-all" marketing is no longer effective. This project matters because:

- Resource Optimization: It prevents wasting premium marketing spend on price-sensitive customers.

- Customer Experience: It improves the shopping experience by providing relevant offers to the right people.

- Scalability: The pipeline is built to handle new data, allowing the mall to categorize thousands of new members automatically as they join the loyalty program.

## Tech Stack

- Language: Python

- Environment: VS Code / Jupyter Notebooks

- Libraries: Pandas, NumPy, Scikit-Learn, Matplotlib, Seaborn, Scipy

## How to Use

Clone the repository.

Install requirements: pip install -r requirements.txt.

Run the kmeans_business_question.ipynb to see the full analysis and visualizations.

Use the inference script to test your own customer data!
