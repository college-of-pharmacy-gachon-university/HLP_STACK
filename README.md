# Predicting Electronic Properties of Molecules  
### A Stacking Ensemble Model for HOMO and LUMO Energy Estimation

In this study, we developed a stacking ensemble machine learning regressor named **HLP-Stack (HOMO-LUMO Predictor via stacking)** to predict HOMO and LUMO energy values using molecular descriptors from the QM9 dataset.

![](/media/omid/HDD2/Manuscript/Word_format/Figures/Main_Architecture.png)

We achieved superior predictive accuracy by combining:
- **2D molecular properties** from RDKit
- **3D quantum mechanical descriptors** from DFT calculations

Feature selection was performed using the **SelectKBest** algorithm with **mutual information regression** to identify the most relevant descriptors.

To interpret feature importance, we used **SHAP Tree Explainer**, revealing key molecular features that significantly influence HOMO and LUMO energy levels.

Finally, our **HOMO-LUMO gap analysis** demonstrated how molecular frameworks and functional groups impact electronic properties.

## Repository Structure

HLP-Stack/

├── notebooks/ # Jupyter notebooks

├── models/ # Saved ML models (.pkl)

├── figures/ # Visualization images

├── data/ # Input and processed datasets (.csv)

├── environment.yml # Reproducible environment

└── README.md # Project overview

## Installation

1. Clone the repository:

git clone https://github.com/college-of-pharmacy-gachon-university/HLP-Stack.git

cd HLP-Stack

2. Create and activate the conda environment:

conda env create -f environment.yml

conda activate hlp-stack

3. Launch JupyterLab

