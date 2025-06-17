# Predicting Electronic Properties of Molecules

---

### A Stacking Ensemble Model for HOMO and LUMO Energy Estimation

Welcome to **HLP-Stack (HOMO-LUMO Predictor via Stacking)**, a cutting-edge stacking ensemble machine learning regressor designed to predict HOMO and LUMO energy values. Our model leverages diverse molecular descriptors from the QM9 dataset to achieve superior predictive accuracy.

**Key Features:**

* **Hybrid Descriptor Integration:** Combines **2D molecular properties** from RDKit with **3D quantum mechanical descriptors** derived from DFT calculations for comprehensive molecular representation.
* **Intelligent Feature Selection:** Employs the **SelectKBest** algorithm alongside **mutual information regression** to pinpoint the most influential molecular descriptors.
* **Interpretability with SHAP:** Utilizes **SHAP Tree Explainer** to reveal the key features driving HOMO and LUMO energy predictions, offering transparent insights into molecular contributions.
* **HOMO-LUMO Gap Analysis:** Provides in-depth analysis demonstrating how specific molecular frameworks and functional groups impact critical electronic properties.

![HLP-Stack Architecture](/media/omid/HDD2/Manuscript/Word_format/Figures/Main_Architecture.png)

---

## Repository Structure
```
HLP-Stack/
├── notebooks/          # Jupyter notebooks for analysis and model development
├── models/             # Saved machine learning models (.pkl files)
├── figures/            # Visualizations and project-related images
├── data/               # Raw and processed datasets (.csv files)
├── environment.yml     # Conda environment configuration for reproducibility
└── README.md           # Project overview and documentation
```

---

## Installation

Getting started with HLP-Stack is straightforward:

1.  **Clone the repository:**

    ```bash
    git clone [https://github.com/college-of-pharmacy-gachon-university/HLP-Stack.git](https://github.com/college-of-pharmacy-gachon-university/HLP-Stack.git)
    cd HLP-Stack
    ```

2.  **Create and activate the Conda environment:**

    ```bash
    conda env create -f environment.yml
    conda activate hlp-stack
    ```

3.  **Launch JupyterLab:**

    ```bash
    jupyter lab
    ```

