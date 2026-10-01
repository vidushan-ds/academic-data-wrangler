# 📊 Academic Data Wrangler

A collection of data cleaning and exploratory data analysis (EDA) projects built with **Python** and **pandas**, focused on turning messy, real-world datasets into clean data and actionable insights.

This repository is a growing portfolio of hands-on data wrangling work — each project follows the same workflow: **explore → clean → engineer → analyze → visualize → summarize**.

---

## 📁 Projects

| Project | Description | Notebook |
|---|---|---|
| 🛒 [Sales Data Analysis](#-1-sales-data-analysis) | Cleans and analyzes retail sales transactions to uncover revenue, profit, and customer trends | `sales-data-analysis/sales_analysis.ipynb` |
| 🎓 [Student Marks Analyzer](#-2-student-marks-analyzer) | Cleans messy student score data and analyzes academic performance | `student-marks-analyzer/student_performance_analysis.ipynb` |
| 🏏 [IPL Match Analysis](#-3-ipl-match-analysis) | Cleans 12 seasons of IPL match data and analyzes team performance, toss impact, and home advantage | `ipl-match-analysis/cricket_analyz.ipynb` |

---

## 🛒 1. Sales Data Analysis

Cleans a retail sales dataset and analyzes it to answer key business questions around revenue, profitability, and customer behavior.

### What it covers
- **Data cleaning:** duplicate removal, date-type conversion, validation of numeric fields, profit consistency checks
- **Feature engineering:** profit margin calculation, day-of-week extraction
- **Business analysis:**
  - Revenue and quantity sold by product and category
  - Profitability analysis (total profit vs. average profit margin)
  - Time-based trends (yearly, monthly, daily revenue)
  - Customer analysis by age group, gender, and country
- **Visualizations:** revenue/profit by category, monthly revenue trend, top countries by revenue, top products by profit margin

### Key insights
- Bikes generate ~72% of total revenue from just ~3% of units sold, while Accessories drive the highest sales volume (78%) but the lowest revenue share (18%)
- Accessories retain the highest profit margin (~59%), outperforming Bikes (~33%) and Clothing (~34%)
- The best-selling product isn't always the most profitable one
- Revenue grew steadily from 2011–2015, then dropped ~12% in 2016
- December and June are peak sales months; July and August are the slowest
- Adults aged 35–64 make up the largest customer segment

### Tools
`pandas` · `matplotlib`

---

## 🎓 2. Student Marks Analyzer

Cleans a student academic dataset containing missing values, duplicates, and invalid text entries, then analyzes performance across subjects and students.

### What it covers
- **Data cleaning:** duplicate removal, replacing invalid placeholders (`ABSENT`, `ERROR`, `NULL`, `N/A`), numeric type conversion, missing value handling
- **Analysis:**
  - Average marks per student and per subject
  - Grade assignment (A–F) based on average score
  - Above/below average performance per subject
  - Best subject per student
  - Top 10 performing students
  - At-risk and failing student identification
- **Visualizations:** subject performance comparison, best-subject distribution, grade distribution (pie chart), top 10 students by average score

### Key insights
- English recorded the highest average marks among all subjects
- Students generally performed better in Science than in Mathematics
- Mathematics had the lowest average score, suggesting it's the most challenging subject
- Emily achieved the highest overall average in the dataset

### Tools
`pandas` · `matplotlib`

---

## 🏏 3. IPL Match Analysis

Cleans 12 seasons (2008–2019) of IPL match data and analyzes what drives winning — team strength, toss decisions, home advantage, and standout players.

### What it covers
- **Data cleaning:** dropping unreliable columns, handling missing city/umpire values, date-type conversion, standardizing renamed/inconsistent team names (e.g. Delhi Daredevils → Delhi Capitals)
- **Feature engineering:** toss-to-match-win flag, home city mapping per franchise, neutral-venue exclusion
- **Analysis:**
  - Most wins and win percentage by team
  - Toss impact on match outcome, and bat-first vs field-first win rates
  - Most Player of the Match awards, overall and by season
  - Venue analysis — most-hosted grounds and top team per venue
  - Season-by-season winning team trends
  - Home vs away win percentage by franchise
- **Visualizations:** top winning teams, win percentage by team, toss outcome pie chart, win % by toss decision, top POTM award winners, top team per season, home vs away win % comparison

### Key insights
- Mumbai Indians have the most wins (109) and lead most by volume, while Chennai Super Kings have the best win rate (60.98%) — the two most successful franchises win in different ways
- Toss winners only won 51.98% of matches, but teams that chose to field first won 55.94% of the time vs 45.73% for teams that batted first — fielding first is the stronger strategic choice
- Home advantage is real: teams win about 10 points more often at home (56.1%) than away (45.6%), with Chennai, Hyderabad, and Rajasthan benefiting the most
- Chris Gayle (21) and AB de Villiers (20) lead all players in Player of the Match awards
- No team topped the win table in two consecutive seasons — the league lead changed hands every year

### Tools
`pandas` · `matplotlib` · `numpy`

--

## 🗂️ Repository Structure

```
academic-data-wrangler/
│
├── sales-data-analysis/
│   ├── data/
│   │   └── sales_data.csv
│   └── sales_analysis.ipynb
│
├── student-marks-analyzer/
│   ├── data/
│   │   ├── data.csv
│   │   └── cleaned_data.csv
│   └── student_performance_analysis.ipynb
│
├── ipl-match-analysis/
│   ├── data/
│   │   └── matches.csv
│   └── cricket_analyz.ipynb
└── README.md
```

---

## ⚙️ Getting Started

### Prerequisites
- Python 3.9+
- Jupyter Notebook or JupyterLab

### Installation
```bash
git clone https://github.com/vidushan-ds/academic-data-wrangler.git
cd academic-data-wrangler
pip install pandas matplotlib jupyter
```

### Run a notebook
```bash
jupyter notebook sales-data-analysis/sales_analysis.ipynb
```

---

## 🧰 Tech Stack

- **Python** – core language
- **pandas** – data cleaning, transformation, and aggregation
- **matplotlib** – data visualization
- **numpy** – numerical operations

---

## 🌱 About This Repository

This repository documents my ongoing journey learning data analysis and pandas — practicing real-world data cleaning techniques (handling missing values, duplicates, invalid entries, and type conversions) and translating cleaned data into meaningful business and academic insights.

More projects will be added here as I continue building on these skills.

---

## 👤 Author

**Vidushan Pathirana**
Data Science Undergraduate