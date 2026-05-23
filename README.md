# 🚢 Titanic Survival Analysis

An Exploratory Data Analysis (EDA) project uncovering survival patterns in the Titanic passenger dataset — examining the impact of gender, passenger class, age, and embarkation port on survival outcomes.

---

## 📌 Project Overview

On April 15, 1912, the Titanic sank after hitting an iceberg — 1,502 out of 2,224 passengers and crew died. This project analyzes the passenger data to answer: **who was more likely to survive, and why?**

---

## 📊 Dataset

Loaded directly via Seaborn's built-in dataset — no external file needed.

```python
df = sns.load_dataset('titanic')
```

| Property | Value |
|---|---|
| Total Passengers | 891 |
| Survived | 342 |
| Not Survived | 549 |
| Features | 15 (age, sex, class, embarked, etc.) |

---

## 🔍 Analysis Breakdown

| Analysis | Key Finding |
|---|---|
| Age Distribution | Most passengers were adults aged 18–37 |
| Gender Split | 577 males vs 314 females on board |
| Class & Survival | First Class had the highest survival rate |
| Gender & Survival | Females survived at ~74% vs males at ~19% |
| Embarkation Port | Southampton was the most common boarding port |
| Age Group Survival | Children had the highest survival rate of all age groups |

---

## 🛠️ Tech Stack

- Python 3.x
- Pandas
- NumPy
- Seaborn
- Matplotlib

---

## 🚀 How to Run

1. **Clone the repository**
   ```bash
   git clone https://github.com/your-username/titanic-survival-analysis.git
   cd titanic-survival-analysis
   ```

2. **Install dependencies**
   ```bash
   pip install pandas numpy seaborn matplotlib jupyter
   ```

3. **Run the notebook** *(no external dataset needed — Seaborn loads it automatically)*
   ```bash
   jupyter notebook titanic_analysis.ipynb
   ```

---

## 📁 Project Structure

```
titanic-survival-analysis/
├── titanic_analysis.ipynb    # Main analysis notebook
└── README.md                 # You are here
```

---

## ⚠️ Limitations

- 177 missing age values — no imputation applied, may affect age-group results
- Analysis is exploratory only — no predictive model built
- Single dataset source — results reflect 1912 Titanic manifest only

---

## 🧠 What I Learned

- Groupby aggregations and survival rate calculations with Pandas
- Creating age bins with `pd.cut()` for group-level analysis
- Visualizing categorical distributions with Seaborn barplots and stacked bar charts
- Interpreting real historical data and forming data-backed conclusions

---

## 📚 Reference

- Dataset: [Kaggle Titanic Competition](https://www.kaggle.com/c/titanic)
- Loaded via `seaborn.load_dataset('titanic')`
