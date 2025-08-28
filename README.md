# Biodiversity Assessment via Unsupervised Learning: A Cluster Analysis of eDNA Datasets

_A Project for Data Analytics & Visualization (DAV) Course_

This project explores the problem statement SIH25042 from the Smart India Hackathon, adapted for the Data Analytics & Visualization (DAV) course at Rashtriya Raksha University.

---

## 1. Project Overview

The objective is to use unsupervised machine learning—specifically cluster analysis—to identify and categorize species from environmental DNA (eDNA) samples. By analyzing raw genetic sequences from estuaries in Goa, India, we assess biodiversity without direct observation. This method supports conservation, environmental monitoring, and ecological research.

---

## 2. Core Objectives

- **Data Pre-processing:** Clean and transform raw eDNA sequence data into a usable numerical format.
- **Feature Engineering:** Extract meaningful features from DNA sequences using k-mer frequency analysis.
- **Unsupervised Learning:** Apply clustering algorithms (K-Means) to group similar sequences and identify species clusters.
- **Data Visualization:** Create informative visualizations to represent clusters and biodiversity metrics.
- **Interpretation:** Analyze results to draw conclusions about the sampled environment's biodiversity.

---

## 3. Technologies Used

- **Language:** Python 3.x
- **Libraries:**
     - `pandas`, `numpy` for data manipulation
     - `scikit-learn` for clustering and PCA
     - `biopython` for biological data handling
     - `matplotlib`, `seaborn` for visualization
- **Tools:**
     - NCBI SRA Toolkit for data acquisition

---

## 4. How to Reproduce This Project

This project uses a large public dataset not stored in this repository. To run the analysis, follow these steps:

### Step 1: Environment Setup

Clone the repository:
```sh
git clone [your-repo-link]
```

Create and activate a Python virtual environment, then install dependencies:
```sh
pip install -r requirements.txt
```

### Step 2: Data Acquisition

Install the NCBI SRA Toolkit (see official instructions for your OS).

Download the data by navigating to `data/01_raw/` and running:
```sh
# Download the compressed SRA file
prefetch SRR26872904

# Unpack to .fastq format
fastq-dump --split-files SRR26872904
```
This creates `SRR26872904_1.fastq` and `SRR26872904_2.fastq` in the correct directory.

### Step 3: Run the Analysis

With the data in place, run the Jupyter Notebooks in `/notebooks` in this order:

1. `01_data_exploration.ipynb`
2. `02_data_preprocessing.ipynb`
3. `03_model_development.ipynb`
4. `04_results_visualization.ipynb`

The final notebook generates the cluster visualizations and summary outputs.

---

## Acknowledgement

Special thanks to Gemini, a large language model from Google, for assistance in structuring the project plan, methodology guidance, and documentation templates.