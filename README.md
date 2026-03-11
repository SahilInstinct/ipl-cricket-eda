#  IPL Exploratory Data Analysis
![Python](https://img.shields.io/badge/Python-3.8+-blue?style=flat&logo=python)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange?style=flat&logo=jupyter)
![pandas](https://img.shields.io/badge/pandas-EDA-green?style=flat&logo=pandas)
![Status](https://img.shields.io/badge/Status-In%20Progress-yellow?style=flat)

An end-to-end EDA project on the Indian Premier League (IPL) dataset using Python.

## 📁 Project Structure
```
ipl_eda_project/
├── data/
│   ├── matches.csv       # Match-level data
│   └── deliveries.csv    # Ball-by-ball data
├── notebook/
│   └── ipl_analysis.ipynb
│
└── README.md
```

## 🛠️ Tech Stack

- **Python 3.8+**
- **pandas** — data loading, cleaning, aggregation
- **numpy** — numerical operations
- **matplotlib** — base plotting
- **seaborn** — statistical visualisations (darkgrid theme)
- **Jupyter Notebook** — interactive analysis environment

---


## 📊 Dataset

**Source:** [Kaggle — IPL Dataset](https://www.kaggle.com/datasets/patrickb1912/ipl-complete-dataset-20082020)

| File | Description | Key Columns |
|---|---|---|
| `matches.csv` | One row per match | team1, team2, winner, toss_winner, venue, season |
| `deliveries.csv` | One row per delivery | batter, bowler, batsman_runs, is_wicket, dismissal_kind |

---

## How to use:

### 1. Clone the repository
```bash
git clone https://github.com/SahilInstinct/ipl-eda-project.git
cd ipl-eda-project
```

### 2. Install dependencies
```
pip install pandas numpy matplotlib seaborn jupyter
```

### 3. Download the dataset
Download `matches.csv` and `deliveries.csv` from [Kaggle](https://www.kaggle.com/datasets/patrickb1912/ipl-complete-dataset-20082020) and place them in the `data/` folder.

### 4. Launch the notebook
```
jupyter notebook notebook/ipl_analysis.ipynb
```

Or open directly in **VS Code** using the Jupyter extension.

---