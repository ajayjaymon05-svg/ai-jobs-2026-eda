# AI Jobs 2026 — Exploratory Data Analysis

An exploratory data analysis (EDA) project exploring AI-related job postings in 2026. The notebook cleans and standardizes the raw data, investigates job-market patterns, visualizes salary and hiring trends, engineers useful features, detects outliers, and builds baseline models to explore salary prediction.

## Project objectives

- Inspect and clean the raw AI jobs dataset.
- Analyze the most common job titles, locations, skills, experience levels, employment types, company sizes, and education requirements.
- Explore salary patterns across roles, countries, industries, experience levels, education, company size, and work arrangements.
- Study relationships between numeric variables and identify outliers.
- Engineer features from dates, job titles, experience, work mode, and skills.
- Explore posting trends and application deadlines.
- Build baseline regression models to estimate salary and examine feature importance.

## Repository structure

```text
ai-jobs-2026-eda/
├── data/
│   └── ai_jobs_2026_unclean.csv
├── notebooks/
│   └── AI_Jobs_2026_EDA_Project.ipynb
├── visualizations/
├── ai_jobs_2026_clean.csv
├── README.md
└── requirements.txt
```

The folder layout above is a suggested structure. Keep the files in the locations that match your actual repository, or update the notebook's input path accordingly.

## Tools and libraries

- Python
- Pandas and NumPy for data preparation and analysis
- Matplotlib and Seaborn for visualization
- scikit-learn for train/test splitting, regression models, and evaluation
- Jupyter Notebook for running the analysis

## Getting started

### 1. Clone the repository

```bash
git clone https://github.com/YOUR-USERNAME/ai-jobs-2026-eda.git
cd ai-jobs-2026-eda
```

Replace `YOUR-USERNAME` with your GitHub username.

### 2. Create and activate a virtual environment (recommended)

Windows:

```bash
python -m venv .venv
.venv\Scripts\activate
```

macOS/Linux:

```bash
python3 -m venv .venv
source .venv/bin/activate
```

### 3. Install dependencies

```bash
python -m pip install --upgrade pip
pip install -r requirements.txt
```

### 4. Add the dataset

Place the raw CSV dataset in the location expected by the notebook. The notebook currently refers to `ai_jobs_2026_unclean (1).csv` through a local Windows path. For portability, change that line to a relative path, for example:

```python
df = pd.read_csv("data/ai_jobs_2026_unclean.csv", dtype=str)
```

Make sure the filename matches the CSV you actually have.

### 5. Run the notebook

```bash
jupyter notebook
```

Open the EDA notebook and run the cells from top to bottom. The notebook exports the cleaned dataset as `ai_jobs_2026_clean.csv`.

## Analysis workflow

1. Data collection and initial audit
2. Data cleaning and standardization
3. Data understanding
4. Univariate analysis
5. Bivariate analysis
6. Multivariate analysis
7. Feature engineering
8. Outlier detection
9. Trend and pattern analysis
10. Baseline salary prediction and feature-importance exploration
11. Export of cleaned data

## Important notes

- Results depend on the supplied dataset and the cleaning choices used in the notebook.
- Salary associations and model feature importance do not establish causation.
- The salary prediction models are exploratory baselines, not guaranteed salary estimates for real job offers.
- Do not commit private, licensed, or very large datasets to a public repository unless you have permission. If needed, provide instructions for obtaining the dataset instead.
- Before publishing, remove personal computer paths and verify that all notebook cells run from a clean environment.

## Author

Add your name and GitHub profile here.
