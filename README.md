# MRSI Analysis: Spectral Pattern Differences in MS vs Non-Hyperintensity Controls
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![Python 3.8+](https://img.shields.io/badge/Python-3.8%2B-blue.svg)](https://www.python.org/downloads/)
[![Jupyter Notebook](https://img.shields.io/badge/Notebook-Jupyter-orange.svg)](https://jupyter.org/)

This repository contains code for analyzing Magnetic Resonance Spectroscopic Imaging (MRSI) data to identify spectral pattern differences between Multiple Sclerosis (MS) lesions and non-hyperintensity controls using Contrastive PCA (cPCA).

This repository contains the code and data processing pipeline for a research project focused on identifying spectral pattern differences between individuals with Multiple Sclerosis (MS) and non-hyperintensity controls using Magnetic Resonance Spectroscopic Imaging (MRSI). We apply Contrastive Principal Component Analysis (cPCA) to highlight variations unique to the MS cohort.

# Project Overview
Goal:
To detect distinct spectral signatures associated with MS lesions compared to healthy-appearing brain tissue.
Approach:
Preprocess and normalize MRSI spectral data.
Apply Contrastive PCA (cPCA) to enhance differences specific to MS by contrasting against control data.
Visualize and interpret low-dimensional embeddings that distinguish MS pathology from normal controls.

# Requirements

You can install the required Python packages using:

```
pip install -r requirements.txt
```

# Key libraries:
numpy

pandas

matplotlib

scikit-learn

seaborn

contrastive (or custom implementation of contrastive PCA)

# How to Run

1. Clone the repository:
```
git clone https://github.com/your-username/MRSI-contrastivePCA.git
cd MRSI-contrastivePCA
```
2. Open the main notebook:
```
jupyter notebook notebooks/D2M.ipynb
```
3. Follow the step-by-step code cells to preprocess, perform cPCA, and visualize results

# Methodology
Preprocessing:
Spectra were normalized to account for intensity differences and denoised to reduce acquisition artifacts.
Contrastive PCA:
cPCA was used to find principal components that vary significantly more in MS patients than in controls, focusing on lesion-specific patterns.
Visualization:
Scatter plots of the contrastive principal components help in visualizing the separability between MS and control samples.

# Results
Clear clustering of MS lesion spectra distinct from control spectra in low-dimensional space.
Identification of key metabolites and spectral regions that drive group differences.
