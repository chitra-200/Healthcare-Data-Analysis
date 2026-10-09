# Healthcare Data Analysis: Exploratory Analysis and Heart Disease Classification

**Student:** Chitrakshi Arya  
**Internship:** AICTE | IBM SkillsBuild Data Analytics with AI Internship 2026 | BharatCares

## Project description
A beginner-friendly Python project that explores a public heart disease dataset. The notebook inspects data quality, summarizes features, visualizes distributions and correlations, handles missing values through a reproducible preprocessing pipeline, and evaluates a baseline logistic regression classifier.

> **Disclaimer:** This project is for education only. It is not a medical diagnostic tool and must not be used to make clinical decisions.

## Dataset
- **Name:** Heart Disease
- **Publisher:** UCI Machine Learning Repository
- **Dataset page:** https://archive.ics.uci.edu/dataset/45/heart+disease
- **DOI:** https://doi.org/10.24432/C52P4X
- **Dataset notes:** UCI describes 303 instances and 13 input features for the commonly used dataset; some features contain missing values.
- **Retrieval:** The notebook downloads the dataset through the `ucimlrepo` Python package, so internet access is needed.

## Technologies
- Python 3
- Jupyter Notebook
- pandas and NumPy
- Matplotlib and Seaborn
- scikit-learn
- ucimlrepo

## Files
- `ChitrakshiArya_HealthcareDataAnalysis.ipynb` — full project code and analysis
- `requirements.txt` — Python dependencies
- `ChitrakshiArya_HealthcareDataAnalysis_ProjectReport.docx` — project report

## Setup and run
1. Install Python 3.10 or newer.
2. Download or extract all project files into one folder.
3. Open a terminal in that folder.
4. Create and activate a virtual environment (recommended):

   **Windows**
   ```bash
   python -m venv .venv
   .venv\Scripts\activate
   ```

   **macOS/Linux**
   ```bash
   python3 -m venv .venv
   source .venv/bin/activate
   ```

5. Install dependencies:
   ```bash
   python -m pip install --upgrade pip
   pip install -r requirements.txt
   ```
6. Start Jupyter:
   ```bash
   jupyter notebook
   ```
7. Open `ChitrakshiArya_HealthcareDataAnalysis.ipynb` and choose **Kernel → Restart & Run All**.

## Reproducibility
- The train/test split uses `random_state=42` and stratifies by target class.
- Preprocessing is included in a scikit-learn pipeline to avoid fitting imputers/scalers on the test set.
- Results may vary slightly across library versions. Run all notebook cells to generate the actual metrics and charts.
- Do not report metric values before running the notebook.

## Target definition
The original target has values 0 through 4. This project defines target 0 as “no recorded disease” and values greater than 0 as “recorded disease” for a binary classification exercise.

## Limitations
- The dataset is historical and relatively small.
- It may not represent today's patient populations or clinical practice.
- A simple train/test split gives only a rough estimate of generalization.
- No model output should be interpreted as a diagnosis.

## Dataset citation
Janosi, A., Steinbrunn, W., Pfisterer, M., & Detrano, R. (1989). Heart Disease [Dataset]. UCI Machine Learning Repository. https://doi.org/10.24432/C52P4X.
