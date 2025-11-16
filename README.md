# Customer_Behavior_Analysis
This is a guided data analytic project. It demonstrated demo customer behavior analysis using python, sql, powerBI, and Excel etc. 


🛍️ Customer Shopping Behavior Analysis
This project analyzes customer shopping behavior using transactional data to uncover valuable insights into spending patterns, product preferences, and subscription engagement. The findings are intended to guide strategic business decisions, optimize product positioning, and refine marketing efforts.

🚀 Project Goals
The primary objectives of this analysis were to:

Identify and understand customer spending patterns and key product preferences.

Uncover different customer segments (e.g., Loyal, Returning, New).

Analyze the impact of subscription status on customer behavior and revenue.

Provide actionable business recommendations based on data-driven insights .

📊 Dataset Summary
The analysis is based on a dataset of 3,900 customer purchases.

Feature Group	Key Features
Customer Demographics	
Age, Gender, Location, Subscription Status 

Purchase Details	
Item Purchased, Category, Purchase Amount (USD), Season, Size, Color 

Shopping Behavior	
Discount Applied, Promo Code Used, Previous Purchases, Frequency of Purchases, Review Rating, Shipping Type 


Note on Missing Data: The Review Rating column contained 37 missing values.

🛠️ Methodology and Tools
1. Exploratory Data Analysis (EDA) and Preparation (Python)

Data Cleaning: Handled 37 missing values in the Review Rating column by imputing them using the median rating of each product category.


Data Standardization: Renamed columns to snake case for improved readability.

Feature Engineering:

Created age_group by binning customer ages.

Created purchase_frequency_days from purchase data.


Data Consistency: The redundant promo_code_used column was dropped.


Database Integration: The cleaned DataFrame was loaded into PostgreSQL for structured SQL analysis.

2. Data Analysis (SQL in PostgreSQL)
Structured SQL queries were executed to answer key business questions, including:


Revenue Comparison: Calculated total revenue by Gender and Age Group.


Discount Analysis: Identified customers who used discounts but still spent above the average purchase amount. Also, identified the 5 products most dependent on discounts.


Product Performance: Found the Top 5 Products by Average Rating and the Top 3 Products per Category by total orders.


Subscription Impact: Compared average spend and total revenue between subscribers and non-subscribers. Checked if customers with >5 purchases are more likely to subscribe.


Segmentation: Classified customers into Loyal (3,116), Returning (701), and New (83) segments based on purchase history.


Shipping Preference: Compared the average purchase amounts across different Shipping Types (e.g., Standard vs. Express).

3. Data Visualization (Power BI)
An interactive Customer Behavior Dashboard was built in Power BI to present the key insights visually.

💡 Key Findings

Gender Revenue Split: Male customers generated significantly more total revenue ($157,890) than Female customers ($75,191).


Subscription Status: The majority of customers (73%) do not have a subscription. Non-subscribers generate higher total revenue ($170,436) and a slightly higher average spend ($59.87) than subscribers.


Shipping Type: Express shipping has a slightly higher average purchase amount ($60.48) compared to Standard shipping ($58.46).


Age Group Revenue: The Young Adult age group contributes the highest total revenue ($62,143).


Top-Rated Products: Gloves, Sandals, and Boots were among the top 3 products by average review rating.


Discount Dependency: Products like the Hat (50.00%) and Sneakers (49.66%) had the highest percentage of discounted purchases.

📝 Business Recommendations

Boost Subscriptions: Promote exclusive benefits for subscribers to increase the 27% subscription rate.


Customer Loyalty Programs: Implement a system to reward repeat buyers and encourage movement from the 'Returning' segment (701 customers) into the 'Loyal' segment (3,116 customers).


Targeted Marketing: Focus marketing efforts on the Young Adult age group and users who select Express Shipping, as they represent high-revenue segments.


Product Positioning: Highlight top-rated and best-selling products (e.g., Gloves, Jewelry, Blouse) in promotional campaigns.
