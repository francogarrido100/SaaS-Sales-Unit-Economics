# SaaS Unit Economics Analysis 📊

## Overview
End-to-end analysis of a SaaS company's unit economics using 4 years of transactional data (2020–2023). 
The goal was to identify profitability drivers, pricing inefficiencies, and customer value across segments and products.

**Tools:** Python · Pandas · Looker Studio · Excel

---

## 📊 Interactive Business Intelligence Dashboard

The results of this analysis were connected to **Google Looker Studio** to build a high-level executive dashboard for strategic decision-making.

* **Live Dashboard Link:** https://datastudio.google.com/s/iV86ADL2rvM

---

## Business Questions Answered
- Which products generate the most revenue vs. the most profit?
- How do discounts impact margin across the portfolio?
- Which customer segments have the highest LTV?
- Is the business growing profitably?

---

## Key Findings

### 📈 Revenue Growth Without Margin Improvement
Revenue grew **52% from 2020 to 2023** ($484K → $733K), but profit margin stagnated at ~13%.
The business is scaling, but not becoming more profitable.

### 🔴 Two Products Are Destroying Value
- **Marketing Suite**: negative margin (-3%). Being sold at a loss.
- **ContactMatcher**: #1 product by revenue ($410K) but only 3% margin. High volume, almost no profit.

### 💎 Hidden Gems
**Alchemy** (37% margin) and **SaaS Connector Pack - Gold** (42% margin) are the most profitable products
despite lower revenue. Scaling these could significantly improve overall profitability.

### ⚠️ Discount Policy Is Broken
| Discount Level | Profit Margin |
|----------------|--------------|
| No discount    | +29.5%       |
| 11–20%         | +11.6%       |
| 21–30%         | -10.1%       |
| 31–40%         | -19.4%       |
| 50%+           | -119.2%      |

Any discount above 20% destroys margin. At 50%+, the company loses $1.19 for every $1 sold.

### 👥 SMB Segment Outperforms Enterprise
Counterintuitively, SMB customers have the highest average LTV ($12,097) vs Enterprise ($5,653).
SMB clients buy more frequently and sustain the business.

---

## Project Structure
```text
├── SaaS-Sales.csv                 # Raw transactional dataset
├── unit_economics_analysis.ipynb  # Jupyter Notebook with Python/Pandas analysis
├── unit_economics_results.xlsx    # Processed data tables used for BI input
└── README.md                      # Project documentation and insights

Data Used: https://www.kaggle.com/datasets/nnthanh101/aws-saas-sales
