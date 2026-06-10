#  IPL Data Analysis (2008–2020)

A complete exploratory data analysis (EDA) of Indian Premier League (IPL) match data using **Python**, **SQL (SQLite)**, and **data visualization** libraries.

---

##  Project Overview

This project analyzes 13 seasons of IPL data to uncover patterns in team performance, player statistics, toss impact, and scoring trends. It demonstrates end-to-end data engineering skills including data cleaning, SQL querying, and visual storytelling.

---

##  Dataset

- **Source**: [Kaggle – IPL Complete Dataset 2008–2020](https://www.kaggle.com/datasets/patrickb1912/ipl-complete-dataset-20082020)
- **Files Used**:
  - `matches.csv` — 816 IPL matches with result, toss, venue, and player details
  - `deliveries.csv` — 179,078 ball-by-ball delivery records

---

##  Tools & Technologies

| Tool | Purpose |
|------|---------|
| Python 3.x | Core programming language |
| Pandas | Data loading, cleaning, transformation |
| SQLite3 | SQL queries on structured data |
| Matplotlib | Data visualizations |
| Seaborn | Statistical charts and heatmaps |
| Jupyter Notebook | Interactive development environment |
| Git & GitHub | Version control |

---

## 📊 Key Analyses Performed

### 🔹 Data Cleaning (Pandas)
- Handled null values in winner, city, and player_dismissed columns
- Standardized team names across seasons (e.g. Delhi Daredevils → Delhi Capitals)
- Converted date strings to datetime and extracted season year

### 🔹 SQL Queries (SQLite)
1. Total matches won by each team across all seasons
2. Toss win to match win conversion rate
3. Top 10 all-time run scorers with average runs per match
4. Top 10 wicket takers (excluding run-outs)
5. Highest team totals in a single innings
6. Season-wise total runs and match count

### 🔹 Visualizations
1. **Bar chart** — Total wins by team
2. **Line chart** — Total runs scored per season (2008–2020)
3. **Pie chart** — Toss decision: bat vs field
4. **Horizontal bar chart** — Top 10 all-time run scorers
5. **Heatmap** — Team vs team win matrix (top 8 teams)

---

## 💡 Key Insights

- **Mumbai Indians** lead all-time wins with 120+ victories across seasons
- Teams winning the toss chose to **field ~57%** of the time in recent seasons
- Winning the toss results in match win only **~52%** of the time — nearly random
- **Virat Kohli** holds the record for most runs in IPL history
- Total runs scored per season show a consistent upward trend from 2008 to 2019
- The **win matrix** reveals MI and CSK have dominant records against most opponents

---

## 📁 Project Structure

```
ipl-data-analysis/
│
├── matches.csv                  # Raw matches data
├── deliveries.csv               # Raw deliveries data
├── matches_clean.csv            # Cleaned matches data
├── deliveries_clean.csv         # Cleaned deliveries data
├── ipl.db                       # SQLite database
│
├── step1_data_cleaning.py       # Data loading and cleaning
├── step2_sql_analysis.py        # SQL queries using SQLite3
├── step3_visualizations.py      # All 5 charts
├── IPL_Analysis.ipynb           # Complete Jupyter Notebook
│
├── chart1_wins_by_team.png
├── chart2_runs_per_season.png
├── chart3_toss_decision.png
├── chart4_top_batsmen.png
├── chart5_win_matrix.png
│
└── README.md
```

---

##  How to Run

```bash
# 1. Clone the repository
git clone https://github.com/YOUR_USERNAME/ipl-data-analysis.git
cd ipl-data-analysis

# 2. Install dependencies
pip install pandas matplotlib seaborn jupyter

# 3. Download dataset from Kaggle and place CSV files in the root folder

# 4. Run scripts in order
python step1_data_cleaning.py
python step2_sql_analysis.py
python step3_visualizations.py

# OR open the notebook
jupyter notebook IPL_Analysis.ipynb
```

---

##  Author

**Anshu Shahdeo**
B.Tech CSE, KIIT University
[LinkedIn](https://www.linkedin.com/in/anshu-shahdeo-7503a936a)

---

## 📄 License

This project is open source under the [MIT License](LICENSE).
