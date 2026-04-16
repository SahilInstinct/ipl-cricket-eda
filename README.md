# 🏏 IPL Exploratory Data Analysis
 
![Python](https://img.shields.io/badge/Python-3.8+-blue?style=flat&logo=python)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange?style=flat&logo=jupyter)
![pandas](https://img.shields.io/badge/pandas-EDA-green?style=flat&logo=pandas)
![Status](https://img.shields.io/badge/Status-Complete-brightgreen?style=flat)
 
An end-to-end EDA project on the Indian Premier League (IPL) dataset using Python — covering match results, team performance, batting, bowling, toss impact, and season-wise trends.
 
---

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
 
**Source:** [Kaggle — IPL Complete Dataset (2008–2020)](https://www.kaggle.com/datasets/patrickb1912/ipl-complete-dataset-20082020)
 
| File | Description | Key Columns |
|---|---|---|
| `matches.csv` | One row per match | team1, team2, winner, toss_winner, venue, season |
| `deliveries.csv` | One row per delivery | batter, bowler, batsman_runs, is_wicket, dismissal_kind |
 
---
 
## 🔧 Data Cleaning
 
Before analysis, the following preprocessing steps were applied:
 
- Parsed `date` column to `datetime` and extracted `season` (year)
- Filled missing `winner` with `"No Result"` for abandoned/tied matches
- Filled missing `player_of_match` and `city` with `"Unknown"`
- Standardised franchise names that changed over the years:

| Old Name | Standardised Name |
|---|---|
| Delhi Daredevils | Delhi Capitals |
| Deccan Chargers | Sunrisers Hyderabad |
| Kings XI Punjab | Punjab Kings |
| Rising Pune Supergiant | Rising Pune Supergiants |
 
---
 
## 📈 Analysis Overview
 
### 1. 🗓️ Match-Level Analysis
- Matches played per IPL season
- Win type distribution — wins by runs vs. wins by wickets
### 2. 🏆 Team Performance
- Top 10 teams by total wins across all seasons
- Win rate (%) per team — filtered to teams with at least 20 matches, with a 50% reference line
### 3. 🏏 Batting Analysis
- Top 10 all-time run scorers
- Boundary analysis — fours vs. sixes for top 10 batters
- Average runs per ball by over — run-rate trends across all 20 overs
### 4. 🎳 Bowling Analysis
- Top 10 wicket takers (run-outs excluded)
- Most common dismissal types across all IPL matches
### 5. 🪙 Toss Analysis
- Toss decision split — bat vs. field preference
- Does winning the toss actually help win the match?
### 6. 📅 Season-wise Trends
- Heatmap of wins per team per season — visualise dominance across years
---
 
## 💡 Key Insights
 
- Most matches are **won by wickets** rather than by runs — teams batting second hold a structural edge
- **Mumbai Indians** lead in total wins across all IPL seasons
- **Virat Kohli** is the all-time leading run scorer in IPL history
- Winning the toss shows **no strong correlation** with winning the match — roughly a coin flip
- **Run rates peak** in the powerplay (overs 1–6) and death overs (17–20), dipping in the middle overs
---
 
## 🚀 How to Use
 
### 1. Clone the repository
```bash
git clone https://github.com/SahilInstinct/ipl-cricket-eda.git
cd ipl-cricket-eda
```
 
### 2. Install dependencies
```bash
pip install pandas numpy matplotlib seaborn jupyter
```
 
### 3. Download the dataset
Download `matches.csv` and `deliveries.csv` from [Kaggle](https://www.kaggle.com/datasets/patrickb1912/ipl-complete-dataset-20082020) and place them in the `data/` folder.
 
### 4. Launch the notebook
```bash
jupyter notebook notebook/ipl_analysis.ipynb
```
 
Or open directly in **VS Code** using the Jupyter extension.
 
---
 
## 🧑‍💻 Author
 
**Sahil** — [GitHub](https://github.com/SahilInstinct)

### 4. Launch the notebook
```
jupyter notebook notebook/ipl_analysis.ipynb
```

Or open directly in **VS Code** using the Jupyter extension.

---
