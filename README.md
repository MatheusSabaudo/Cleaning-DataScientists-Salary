# 📊 Data Science Salaries Analysis

## 📋 Project Description

Analysis of a dataset containing **3,755 salaries** in the field of Data Science, covering the years **2020-2023**.
The goal is to answer 6 key questions about the data job market, with a focus on the impact of the COVID-19 pandemic.

## 🎯 Research Questions

1. **Is there a correlation between experience level and salary?**
2. **Are there salary differences between companies of different sizes?**
3. **How are data professionals geographically distributed?**
4. **What has been the growth of data professionals over the last 4 years?**
5. **Is there a correlation between the pandemic onset and the increase in professionals?**
6. **Which are the highest-paid roles in the sector?**

## 🛠️ Technologies Used

* **Python 3.13**
* **Pandas** - Data manipulation and analysis
* **NumPy** - Numerical computations
* **Matplotlib** - Basic visualizations
* **Seaborn** - Advanced statistical visualizations
* **SciPy** - Statistical tests (ANOVA, t-test)

## 📁 Project Structure

```
Data-Cleaning.ipynb          # Main notebook with full analysis
data/
└── ds_salaries.csv          # Original dataset
README.md                    # Project documentation
```

## 🔍 Analysis Steps

### 1. Data Cleaning & Preprocessing

* Converted experience level codes (SE → Senior-Level, MI → Mid-Level, EN → Entry-Level, EX → Executive-Level)
* Converted employment types (FT → Full-Time, CT → Contract, FL → Freelance, PT → Part-Time)
* Converted company sizes (L → Large, M → Medium, S → Small)
* Set ordinal order for categorical variables

### 2. Statistical Analysis

* **ANOVA** to compare group means
* **T-tests** for pairwise comparisons
* **Descriptive statistics** (mean, median, standard deviation)
* **CAGR calculation** (Compound Annual Growth Rate)

### 3. Visualizations

* Boxplots for salary distributions
* Bar charts for categorical comparisons
* Time series for trend analysis
* Heatmaps for geographic correlations

## 📊 Key Findings

### 📈 Sector Growth

* **2020**: 76 positions
* **2023**: 1,785 positions
* **Total growth**: +2,249%
* **CAGR**: +186.4%

### 💰 Salaries by Experience

| Level           | Average Salary | Premium vs Entry-Level |
| --------------- | -------------- | ---------------------- |
| Entry-Level     | $78,546        | -                      |
| Mid-Level       | $104,526       | +33%                   |
| Senior-Level    | $153,051       | +95%                   |
| Executive-Level | $194,931       | +148%                  |

### 🏢 Salaries by Company Size

| Size   | Average Salary | Premium vs Small |
| ------ | -------------- | ---------------- |
| Small  | $78,227        | -                |
| Medium | $143,131       | +83%             |
| Large  | $118,301       | +51%             |

### 🌍 Geographic Distribution

* **USA**: 81% of positions (3,040)
* **UK**: 4.6% (172)
* **Canada**: 2.3% (87)
* **Spain**: 2.1% (77)

### 🦠 Pandemic Impact

* **Post-pandemic growth**: +4,741%
* **Pre-pandemic salary**: $92,303
* **During pandemic salary**: $138,506
* **Salary increase**: +50.1%

### 🏆 Highest-Paid Roles

| Role                               | Average Salary |
| ---------------------------------- | -------------- |
| Principal Data Scientist           | $198,171       |
| Director of Data Science           | $195,141       |
| Machine Learning Software Engineer | $192,420       |
| Data Science Manager               | $191,279       |
| Applied Scientist                  | $190,264       |

## 📈 Statistical Tests

### ANOVA - Experience vs Salary

* **F-statistic**: 245.67
* **p-value**: < 0.001
* **Conclusion**: Statistically significant correlation

### ANOVA - Company Size vs Salary

* **F-statistic**: 89.23
* **p-value**: < 0.001
* **Conclusion**: Significant differences between company sizes

## 💡 Key Takeaways

1. **Experience matters**: Senior-Level earn twice as much as Entry-Level
2. **Medium companies pay more**: Surprisingly, medium-sized companies pay more than large ones
3. **USA dominates the market**: 81% of positions are in the United States
4. **Pandemic boom**: Explosive growth (+623% in 2022) post-pandemic
5. **Specialization is rewarded**: Machine learning and data science leadership roles are the highest-paid

## 🚀 How to Run

```bash
# Clone the repository
git clone https://github.com/MatheusSabaudo/Cleaning-DataScientists-Salary.git

# Install dependencies
pip install pandas numpy matplotlib seaborn scipy

# Open the notebook
jupyter notebook Data-Cleaning.ipynb
```

## 📝 Notes

* Dataset includes only positions with salaries converted to USD
* Statistical tests performed with α = 0.05
* Only roles with ≥ 5 occurrences were considered for reliability

## 📚 Sources

* Dataset: [Data Science Salaries on Kaggle](https://www.kaggle.com/datasets/ruchi798/data-science-job-salaries)
* Years covered: 2020-2023

## ✨ Author

[Matheus Sabaudo Rodrigues] - Full data analysis with focus on market trends and pandemic impact
