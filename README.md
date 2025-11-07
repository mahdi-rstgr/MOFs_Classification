# MOFs Classification: Machine Learning for Carbon Capture

## Overview
This project applies machine learning classification models to identify promising metal–organic frameworks (MOFs) for carbon capture applications. The focus is on two key properties:
- **CO₂ uptake at low pressure** (adsorption capacity and selectivity)
- **Water stability** (material durability and reusability)

By leveraging data-driven methods, the project aims to accelerate the discovery of MOFs suitable for carbon capture.

## Project Structure
- `MOFs_classifications.ipynb`: Main Jupyter notebook for data analysis, model building, and evaluation.
- `MOF_descriptors.py`: Python module containing lists of geometric, linker, metal center, and functional group descriptors used for feature engineering.
- `Data/`
  - `MOF_CoRE2019.csv`: Dataset with MOF features and simulated CO₂ uptake values, based on ["Understanding the diversity of the metal-organic framework ecosystem"](https://doi.org/10.1038/s41467-020-17755-8).
  - `all_data_ws.csv`: Dataset with MOF features and experimental water stability labels, from ["MOF-ChemUnity: Unifying metal-organic framework data using large language models"](https://chemrxiv.org/engage/chemrxiv/article-details/6838df8bc1cb1ecda036f363).

## Key Features
- **Descriptor Engineering**: Uses a comprehensive set of geometric, linker, metal center, and functional group descriptors (see `MOF_descriptors.py`).
- **Data Cleaning & Preparation**: Handles missing values, duplicates, and class creation (e.g., promising vs. non-promising MOFs based on CO₂ uptake > 2 mmol/g).
- **Modeling**: Implements various machine learning models (e.g., Kernel Ridge Regression, XGBoost, Linear Regression, Dummy Classifiers) using scikit-learn and XGBoost.
- **Evaluation**: Assesses models using accuracy, precision, recall, F1-score, and confusion matrices.
- **Reproducibility**: Sets random seeds and saves models for future use.

## Getting Started
1. **Clone the repository**
2. **Install dependencies** (see notebook for package list, e.g., pandas, numpy, scikit-learn, xgboost, seaborn, matplotlib, ydata-profiling)
3. **Run `MOFs_classifications.ipynb`** to reproduce the analysis and results.

## References
- [Understanding the diversity of the metal-organic framework ecosystem](https://doi.org/10.1038/s41467-020-17755-8)
- [MOF-ChemUnity: Unifying metal-organic framework data using large language models](https://chemrxiv.org/engage/chemrxiv/article-details/6838df8bc1cb1ecda036f363)

---

*For questions or contributions, please open an issue or pull request on this GitHub repository.*
