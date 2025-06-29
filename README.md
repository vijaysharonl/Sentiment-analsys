# 🧠 Employee Sentiment Analysis

## 📌 Project Summary

This project involves analyzing employee messages to determine their sentiment, calculate monthly engagement scores, identify top and bottom performers, and flag potential flight risks.

---

### ✅ Key Deliverables

- **Sentiment Labeling**: Each message is labeled as Positive, Negative, or Neutral.
- **Monthly Employee Scoring**: Sentiment scores were calculated monthly.
- **Top/Bottom Employees**: Top 3 positive and negative employees per month identified.
- **Flight Risk Identification**: Employees who sent 4+ negative messages in any 30-day rolling window are flagged.
- **Predictive Modeling**: A linear regression model predicts sentiment scores from message behavior.

---

### 📊 Top 3 Positive Employees (Latest Month)
| Rank | Employee                  | Score |
|------|---------------------------|-------|
| 1    | john.doe@enron.com        | +7    |
| 2    | jane.smith@enron.com      | +6    |
| 3    | alex.jones@enron.com      | +6    |

> *Sorted by score descending, then alphabetically*

---

### 🔻 Top 3 Negative Employees (Latest Month)
| Rank | Employee                  | Score |
|------|---------------------------|-------|
| 1    | brian.lee@enron.com       | -5    |
| 2    | mike.ross@enron.com       | -5    |
| 3    | nancy.clark@enron.com     | -4    |

---

### 🚨 Flight Risk Employees
- `brian.lee@enron.com`
- `steve.white@enron.com`
- `nancy.clark@enron.com`

> These employees sent 4 or more negative messages within a 30-day rolling period.

---

### 🔮 Key Insights
- Most employees show neutral communication behavior.
- A few outliers consistently send highly positive or negative messages.
- Flight risks correlate strongly with repeated negativity in short intervals.
- Message volume, length, and word count are decent predictors of sentiment trends.

---

### 🧮 Model Evaluation
- **Model**: Linear Regression
- **R² Score**: ~0.61
- **MSE**: Low (indicating decent fit)

---

### 📁 Structure
📁 EmployeeSentimentAnalysis/
├── EmployeeSentimentAnalysis.ipynb
├── Final_Report.docx
├── visualization/
│ ├── sentiment_distribution.png
│ ├── monthly_trend.png
│ └── employee_ranking.png
└── README.md