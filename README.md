# customer_behaviour_analysis
Data Analytics Project – Customer Behaviour Analysis

1. Overview
This project demonstrates a complete data analytics workflow — from raw data to insights and visualization. The analysis covers data loading, cleaning, exploration, SQL querying, and dashboard creation using Python, PostgreSQL, Power BI, and Gamma AI.
The goal is to uncover key trends and generate actionable insights through interactive visual reports and an executive presentation deck.

2. Dataset
Format: CSV file
Records: 3,900 rows × 18 columns

3. Description: The dataset contains information on:
Customer Demographics (Age, Gender, Location, Subscription Status)
- Purchase Details (Item Purchased, Category, Purchase Amount (USD), Size, Colour,
Season, Payment Method)
- Shopping Behaviour (Discount Applied, Promo Code Used, Previous Purchases,
Frequency of Purchases, Review Rating, Shipping Type)

4. Tools and Technologies
Python: Data loading, cleaning, and exploratory data analysis (EDA)
Pandas, NumPy, Matplotlib, Seaborn: Data manipulation and visualization
PostgreSQL: SQL querying and database management
Power BI: Dashboard development and visualization
Gamma AI: Automated presentation design and report creation

5. Steps and Workflow
Data Loading: Imported the dataset into Python using Pandas.
Exploratory Data Analysis (EDA): Examined a sample of the uncleaned dataset using df.head(). Utilised df.info() and df.describe() to conduct an initial exploration of the data structure and associated summary statistics.

Data Cleaning
Handled missing values: Identified 37 null values in the Review Rating column and imputed the median review rating for each category.
Column Standardisation: Formatted each column name as snakecase. The column purchase_amount_(usd) was renamed to purchase_amount_usd.
Feature Engineering:
- Created a new column, age_group by binning customer ages.
- Created a new column, purchase_frequency_days to represent the Frequency of Purchases column numerically in days (i.e. Every 3 months as 90 days).
Data Consistency Check: Verified that discount_applied and promo_code_used columns were identical. Hence promo_code_used was removed as a redundant column.

SQL Integration: Connected cleaned data in Python to a PostgreSQL database and loaded the dataset for SQL analysis.

Executed analytical queries

Dashboard Creation (Power BI): 
Built interactive visuals highlighting KPIs and trends
Linked filters and drill-down options for deeper analysis

Report and Presentation:
Summarized findings into a concise report
Created a professional presentation using Gamma AI

Dashboard
The Power BI dashboard includes:
Key Summary Statistics
Category-wise breakdowns
Interactive filters for dynamic exploration
<img width="1462" height="797" alt="Customer Shopping Behaviour Dashboard Screenshot" src="https://github.com/user-attachments/assets/7702c669-7111-44ff-aaa4-0b40652a1cdd" />

Business Recommendations Based on Data Analysis:
Boost Subscriptions - Promote exclusive benefits for subscribers to incentivise new subscriptions.
Customer Loyalty Programs - Reward repeat customers to incentivise them to subscribe.
Review Discount Policy - Balance increased revenues from discounts with margin control.
Product Positioning - Highlight top-rated, and best-selling products in marketing campaigns.
Targeted Marketing - Focus efforts on high-revenue age groups and express-shipping users.

How to Run
Clone this repository:
bash
git clone https://github.com/Sristi-Das/customer_behaviour_analysis.git

Navigate to the project folder:
bash
cd customer_behaviour_analysis

Install dependencies:
bash
pip install psycopg2-binary sqlalchemy

Run the Python notebook for EDA and data cleaning.
Import the cleaned dataset into PostgreSQL and execute SQL scripts.

Open the Power BI dashboard file (.pbix) to view visualizations.

Review the Gamma AI presentation for the final summary.

Author
Srist Das
