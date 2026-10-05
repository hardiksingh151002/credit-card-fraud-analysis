# Credit Card Fraud & Customer Spending Analysis

A Python data analysis project where I explore credit card transaction data to understand fraud patterns, customer spending, and the impact of an offer campaign.

## What I did
- Cleaned the data (removed duplicates, handled missing values)
- Explored fraud rate by category, channel, hour of day and international vs domestic
- Analysed customer spending (top 20% customers, monthly trend, city tier)
- Built a Logistic Regression model to predict fraud
- Ran a t-test to check if an offer campaign increased spending

## Key findings
- International transactions are about 7x more likely to be fraud (5.06% vs 0.68%)
- Travel and Electronics are the riskiest categories; Online is the riskiest channel
- Top 20% of customers contribute about 40% of total spend
- The model catches about 69% of fraud (ROC-AUC 0.81) but has many false alarms
- The offer campaign gave about 4.4% more spend (p = 0.0456, borderline significant)

## Tools
Python, Pandas, NumPy, Matplotlib, Scikit-learn, SciPy, Jupyter Notebook

## Files
- `fraud_analysis.ipynb` - main notebook with all the code and explanations
- `data/` - transactions.csv, customers.csv, campaign.csv (synthetic data)

## How to run
```
pip install -r requirements.txt
jupyter notebook
```
Then open `fraud_analysis.ipynb` and run all cells.

## Note
The dataset is synthetic (generated for practice), so results are not from real bank data.
