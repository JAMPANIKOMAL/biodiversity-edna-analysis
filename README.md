# Biodiversity Assessment via Unsupervised Learning: A Cluster Analysis of eDNA Datasets

_A Project for Data Analytics & Visualization (DAV) Course_

This project explores the SIH25042 problem statement from the Smart India Hackathon, adapted for the Data Analytics & Visualization (DAV) course at Rashtriya Raksha University.

---

## 1. Project Overview

The objective is to use unsupervised machine learning—specifically cluster analysis—to identify and categorize species from environmental DNA (eDNA) samples. By analyzing raw genetic sequences from Goa estuaries, we assess biodiversity without direct organism observation. This method supports conservation, environmental monitoring, and ecological research.

---

## 2. Core Objectives

- **Data Pre-processing:** Clean and transform raw eDNA sequence data into a usable numerical format.
- **Feature Engineering:** Extract features from DNA sequences using k-mer frequency analysis.
- **Unsupervised Learning:** Apply clustering algorithms (K-Means) to group similar sequences and identify species clusters.
- **Data Visualization:** Create interactive visualizations to represent clusters and biodiversity metrics.
- **Interpretation:** Analyze results to draw conclusions about the sampled environment's biodiversity.

---

## 3. Technologies Used

- **Language:** Python 3.x
- **Libraries:**
     - `pandas`, `numpy` for data manipulation
     - `scikit-learn` for machine learning (Clustering, PCA)
     - `biopython` for biological data handling
     - `matplotlib`, `seaborn` for visualization
- **Tools:** NCBI SRA Toolkit for data acquisition

---

## 4. How to Reproduce This Project

This project uses a large public dataset not stored in this repository. To run the analysis:

### Step 1: Environment Setup

Clone the repository:
```bash
git clone [your-repo-link]
```

Create and activate a Python virtual environment, then install dependencies:
```bash
pip install -r requirements.txt
```

### Step 2: Data Acquisition

Install the NCBI SRA Toolkit (see [official instructions](https://github.com/ncbi/sra-tools/wiki/01.-Downloading-SRA-Toolkit)).

Download the data by running:
```bash
# Download the compressed SRA file
prefetch SRR26872904

# Unpack to .fastq format
fastq-dump --split-files SRR26872904
```
This will generate `SRR26872904_1.fastq` and `SRR26872904_2.fastq` in `data/01_raw/`.

### Step 3: Run the Analysis

Run the Jupyter Notebooks in `/notebooks` in order:
1. `01_data_exploration.ipynb`
2. `02_data_preprocessing.ipynb`
3. `03_model_development.ipynb`

The final notebook generates the cluster visualizations and summary outputs.

---

## Acknowledgement

Assistance from Gemini, a large language model by Google, was instrumental in structuring the project plan, methodology guidance, and documentation templates.