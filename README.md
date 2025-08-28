# Biodiversity Assessment via Unsupervised Learning: A Cluster Analysis of eDNA Datasets

_A Project for Data Analytics & Visualization (DAV) Course_

This project explores the SIH25042 problem statement from the Smart India Hackathon, adapted for the Data Analytics & Visualization (DAV) course at Rashtriya Raksha University.

---

## 1. Project Overview

The objective is to use unsupervised machine learning—specifically cluster analysis—to identify and categorize species from environmental DNA (eDNA) samples. By analyzing raw genetic sequences from sources such as water or soil, we can assess biodiversity without direct observation of organisms. This approach supports conservation, environmental monitoring, and ecological research.

---

## 2. Core Objectives

- **Data Pre-processing:** Clean and transform raw eDNA sequence data into a usable numerical format.
- **Feature Engineering:** Extract meaningful features from DNA sequences (e.g., k-mer frequency analysis).
- **Unsupervised Learning:** Apply clustering algorithms (K-Means, Hierarchical, DBSCAN) to group similar sequences and identify species clusters.
- **Data Visualization:** Create interactive visualizations to represent clusters and biodiversity metrics.
- **Interpretation:** Analyze results to draw conclusions about the sampled environment's biodiversity.

---

## 3. Methodology

The workflow includes:

1. **Data Acquisition:** Use public eDNA datasets from repositories like the NCBI Sequence Read Archive (SRA).
2. **Data Cleaning & Transformation:** Parse sequence files and convert them into a k-mer frequency matrix.
3. **Dimensionality Reduction:** Apply PCA to reduce feature space for improved visualization and performance.
4. **Clustering:** Apply and evaluate clustering models to group the data.
5. **Visualization & Analysis:** Interpret clusters as species and calculate biodiversity metrics.

---

## 4. Technologies Used

- **Language:** Python 3.x
- **Libraries:**
    - `pandas`, `numpy` for data manipulation
    - `scikit-learn` for machine learning (Clustering, PCA)
    - `biopython` for biological data handling
    - `matplotlib`, `seaborn`, `plotly` for data visualization

---

## 5. How to Run This Project

1. **Clone the repository:**
     ```bash
     git clone [your-repo-link]
     ```
2. **Install dependencies:**
     ```bash
     pip install -r requirements.txt
     ```
3. **Run the Jupyter Notebooks:**
     - The analysis is detailed in the notebooks in the `/notebooks` directory, numbered in the order they should be run.

---

## Acknowledgement

Special thanks to Gemini, a large language model from Google, for assistance in structuring the project plan, guiding the methodology, and generating documentation templates.