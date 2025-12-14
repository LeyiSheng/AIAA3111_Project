# AIAA3111 Project

Mini project for the AIAA3111 Data Mining course. The notebook trains several classifiers on the San Francisco crime dataset (`sf-crime/train.csv`) to predict crime categories and explore temporal/spatial patterns. You ccan douwload the dataset from https://www.kaggle.com/competitions/sf-crime/data?select=train.csv.zip.

## Environment setup and dependencies
- Python 3.10+ recommended
- Required libraries: pandas, numpy, matplotlib, seaborn, scikit-learn, xgboost, scipy, jupyter
- Data files expected under `sf-crime/` (`train.csv`, `test.csv`, `sampleSubmission.csv`)

## Installation instructions
1) Create and activate a virtual environment:
   ```bash
   python -m venv .venv
   source .venv/bin/activate  # Windows: .venv\Scripts\activate
   ```
2) Install dependencies:
   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn xgboost scipy jupyter
   ```
3) Ensure the dataset CSVs remain in `sf-crime/` relative to the project root.

## How to execute or reproduce results
1) Activate the virtual environment:
   ```bash
   source .venv/bin/activate
   ```
2) Launch Jupyter and open the notebook:
   ```bash
   jupyter notebook project.ipynb
   ```
3) Run the cells from top to bottom. The notebook:
   - Loads and cleans `sf-crime/train.csv`
   - Trains Logistic Regression, Decision Tree, Random Forest, and XGBoost models (with cross-validation and grid search)
   - Generates feature-importance and temporal analyses
4) Optional: adjust hyperparameters or random seeds in the modeling cells to replicate or extend the reported scores.
