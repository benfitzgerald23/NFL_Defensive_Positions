# 🏈 Positional Predictive Modelling for Defensive Players in NFL Player Evaluation

This repository contains the full code, data, and analysis for a master's thesis project focused on evaluating NFL defensive players using data-driven models. The project compares traditional scouting methods with machine learning predictions to assess long-term professional success, focusing on Defensive Linemen (DL), Linebackers (LB), and Defensive Backs (DB).

## 📘 Project Overview

Traditional NFL scouting often emphasises athletic testing and draft pedigree, but may overlook consistent collegiate performance. This project builds machine learning models using college statistics and Combine data from 2008–2024 to predict professional success, measured by **Weighted Career Approximate Value per Year (WCarAV/year)**.

## 📁 Project Structure
.
├── data/                         # Contains all data files
│   ├── def_college_stats_2008.xlsx
│   ├── def_college_stats_2009.xlsx
│   ├── ...                       # Yearly college stats through 2024
│   ├── combined_college_data.xlsx
│   ├── combine_data.xlsx
│   ├── draft_data.xlsx

├── scrape/                       # Python scripts to scrape raw data
│   ├── scrape_college_data.py
│   ├── scrape_combine_data.py
│   ├── scrape_draft_data.py

├── 1.1 Combine Defensive Files.ipynb   # Combines and aligns data sources
├── 1.2 Data Preprocessing.ipynb        # Cleans and prepares datasets
├── 1.3 Correlations.ipynb              # Correlation analysis (draft vs success)
├── 1.4.1 Modelling DL.ipynb            # Modelling pipeline for Defensive Linemen
├── 1.4.2 Modelling LB.ipynb            # Modelling pipeline for Linebackers
├── 1.4.3 Modelling DB.ipynb            # Modelling pipeline for Defensive Backs

├── README.md                    # Project overview and documentation



## ⚙️ Technologies Used

- Python 3.10
- pandas, numpy, scikit-learn, xgboost
- imbalanced-learn (SMOTE)
- matplotlib, seaborn
- BeautifulSoup4 (web scraping)
- Jupyter Notebooks
- LaTeX (thesis write-up)

## 📊 Evaluation Metric

- **WCarAV/year**: A weighted version of Career Approximate Value (CarAV) from Pro Football Reference, normalised by number of seasons played. This allows comparisons between players of different draft classes and career lengths.

## 🧠 Modelling Summary

- Trained models using Random Forest and XGBoost to predict high-impact players at each defensive position.
- Compared top 10 players selected by the model with top 10 drafted players.
- Evaluated performance using t-tests on WCarAV/year to test impact prediction accuracy.

## 📈 Correlation Analysis

- Generated correlation matrices (Pearson, Spearman, Kendall) for each position group.
- Analysed metrics influencing draft pick and NFL success (WCarAV/year).
- Visual results available in `1.3 Correlations.ipynb` and Appendix of the thesis.



