# MRSI-CPCA
This repository contains the code and data processing pipeline for a research project focused on identifying spectral pattern differences between individuals with Multiple Sclerosis (MS) and non-hyperintensity controls using Magnetic Resonance Spectroscopic Imaging (MRSI). We apply Contrastive Principal Component Analysis (cPCA) to highlight variations unique to the MS cohort.

Project Overview

Goal:
To detect distinct spectral signatures associated with MS lesions compared to healthy-appearing brain tissue.
Approach:
Preprocess and normalize MRSI spectral data.
Apply Contrastive PCA (cPCA) to enhance differences specific to MS by contrasting against control data.
Visualize and interpret low-dimensional embeddings that distinguish MS pathology from normal controls.
Repository Structure

📁 data/
    Raw and processed MRSI spectra (not included here for privacy)
📁 notebooks/
    D2M.ipynb — Main analysis notebook (cleaned and annotated)
📁 results/
    Figures, plots, and statistical outputs
📄 README.md
Requirements

You can install the required Python packages using:

pip install -r requirements.txt
Key libraries:

numpy
pandas
matplotlib
scikit-learn
seaborn
contrastive (or custom implementation of contrastive PCA)
Note: Include a requirements.txt file listing exact versions if you want full reproducibility.

How to Run

Clone the repository:
git clone https://github.com/your-username/MRSI-contrastivePCA.git
cd MRSI-contrastivePCA
Open the main notebook:
jupyter notebook notebooks/D2M.ipynb
Follow the step-by-step code cells to preprocess, perform cPCA, and visualize results.
Methodology

Preprocessing:
Spectra were normalized to account for intensity differences and denoised to reduce acquisition artifacts.
Contrastive PCA:
cPCA was used to find principal components that vary significantly more in MS patients than in controls, focusing on lesion-specific patterns.
Visualization:
Scatter plots of the contrastive principal components help in visualizing the separability between MS and control samples.
Results

Clear clustering of MS lesion spectra distinct from control spectra in low-dimensional space.
Identification of key metabolites and spectral regions that drive group differences.
Citation

If you use this work or build on it, please cite:

[Your Paper Title Here]
Author Names
Year
Journal
Acknowledgements

We thank [Institution/Group] for providing the MRSI data and [Advisor/Collaborators] for their guidance throughout this project.
