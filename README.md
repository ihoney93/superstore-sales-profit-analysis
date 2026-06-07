# Superstore Sales & Profit Analysis

## Overview
I took on this project as a business analytics exercise — imagine a 
manager handing me a spreadsheet and asking "where are we making money 
and where are we losing it?" That's exactly what I set out to answer.

The dataset covers 9,994 transactions from a US retail superstore across 
regions, product categories, and customer segments. Source: Kaggle.

---

## The Business Questions I Answered
1. Where is our money coming from? Which regions and states are strongest?
2. Which product categories are actually profitable?
3. Are discounts hurting our margins?
4. Which customer segment should we focus on?
5. How does shipping method affect profitability?

---

## Tools Used
- Python — pandas, matplotlib, seaborn
- Jupyter Notebook
- Google Looker Studio — interactive dashboard

---

## What I Found

**Region:** West and East are carrying the business. Central is the 
problem — it generates $501K in sales but only $39K in profit (7.9% 
margin vs West's 14.9%). Texas specifically shows up as our 3rd highest 
sales state but with negative profit. Something is wrong there.

**Category:** Technology is our strongest category in both sales and 
profit. Furniture is the one that needs a serious conversation — second 
highest sales but barely any profit. When I drilled into sub-categories, 
Tables jumped out immediately: strong sales, but losing $17,725. 

**Discounts:** My boss was right to be suspicious. Products at 0% 
discount generate the most profit by far. Anything above 30% discount 
is losing money. The 70-80% discount range is particularly bad — almost 
no customers and heavy losses every time.

**Customer Segments:** Consumer brings in the most total profit but 
Home Office has the best profit margin at 14.03%. They buy less but 
every sale is more efficient.

**Shipping:** Most customers choose Standard Class but First Class 
shipping has the highest profit margin at 13.93%. Same pattern as 
segments — volume doesn't always mean efficiency.

---

## My Recommendations
1. Investigate Central region and Texas discounting immediately
2. Review Tables and Bookcases pricing — both are loss-making products
3. Cap discounts at 20% maximum — eliminate anything above 30%
4. Invest in growing the Home Office segment for better margins
5. Obtain order date data for seasonal trend analysis — this dataset 
   didn't include dates which limited the time-based analysis

---

## Dashboard
I built a Looker Studio dashboard to visualize the key findings:
- Sales & Profit by Region
- Profit and Sales by Category
- Discount vs Profit scatter plot
- Profit Share by Segment

See `Superstore_Sales_&_Profit_Analysis_Dashboard.pdf` in this repository.

---

## How to Run
1. Clone this repository
2. Open `Superstore.ipynb` in Jupyter Notebook
3. Place `Superstore.xlsx` in the same folder
4. Run all cells in order

---

## Notes
This was a purely business analytics project — no machine learning, 
just data exploration, visualization, and business storytelling. 
The goal was to answer real questions a manager would actually ask 
and deliver recommendations they could act on.
