# Household Energy Consumption Analysis and Prediction

An Applied Machine Learning project analyzing the **UCI Individual Household Electric Power Consumption** dataset to predict household power consumption and discover temporal energy usage patterns.

---

## 📌 Project Overview

This project explores electrical power consumption measurements recorded at 1-minute intervals over a 4-year period (December 2006 to November 2010). 

### Key Objectives:
1. **Data Preprocessing & Resampling:** Cleaning missing sensor values and downsampling ~2.07 million minute-by-minute records into hourly averages (~34,500 samples) for robust analysis.
2. **Correlation Analysis:** Evaluating relationships using **Pearson**, **Spearman**, and **Kendall Tau** methods against `Global_active_power`.
3. **Regression Modeling (Supervised Learning):** Training and benchmarking 5 regression models:
   - Linear Regression
   - Ridge Regression
   - Lasso Regression
   - Decision Tree Regressor
   - Random Forest Regressor
4. **Pattern Discovery (Unsupervised Learning):** Implementing **K-Means Clustering** with Elbow Method and Silhouette Analysis to categorize consumption into *Low*, *Moderate*, and *Peak* usage profiles across the 24 hours of the day.

---

## 📂 Project Structure

```
├── household_power_analysis.ipynb   # Main Jupyter Notebook with all analysis & models
├── requirements.txt                 # Project dependencies
├── .gitignore                       # Ignored files (dataset & virtual environment)
└── README.md                        # Project documentation
```

---

## 📊 Dataset

- **Source:** [UCI Machine Learning Repository - Individual Household Electric Power Consumption](https://archive.ics.uci.edu/dataset/235/individual+household+electric+power+consumption)
- **File:** `household_power_consumption.txt` *(Note: Due to GitHub's file size limits (>100MB), download the text file directly from UCI and place it in the project root directory).*

---

## ⚙️ Installation & Usage

1. **Clone the repository:**
   ```bash
   git clone https://github.com/dishitavaswani/Household-Energy-Consumption-Analysis-Prediction.git
   cd Household-Energy-Consumption-Analysis-Prediction
   ```

2. **Create and activate a virtual environment:**
   ```bash
   python -m venv .venv
   # Windows:
   .\.venv\Scripts\activate
   # macOS/Linux:
   source .venv/bin/activate
   ```

3. **Install dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

4. **Run Jupyter Notebook:**
   ```bash
   jupyter notebook household_power_analysis.ipynb
   ```
