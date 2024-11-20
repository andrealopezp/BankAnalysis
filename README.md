# Project Background
eMoney, a digital bank founded in 2015, specializes in simplifying financial management through products designed for it. Thanks to the success of its first product, eMoney savings account, the platform expanded through a partnership with eBanking S.A., which introduced complexity to its product offerings. As the company faces pressure to achieve profitability with limited funding, eMoney is at a critical point in leveraging its existing customer base for growth. I am working as a Data Scientist in the Marketing Team to extract insights, deliver recommendations, segment customers and develop a predictive model to improve performance across sales, product, and marketing teams.



**Insights and Recommendations** are provided on the following key areas:
* **Products Popularity and Customer Preferences**: An analysis of products trends as well as most in demand products among customers.
* **Customer Loyalty Across Top Products**: An assessment of the loyalty on customer retention and sales.
* **New Customer Acquisition by Product:** An evaluation of number of new customers who have purchased a product for the first time.
* **Product Churn by Month:** An analysis of the number of customers who end their relationship with a company on a monthly basis.
* **Trends in Product Revenue Over Time:** An assessment of products, understanding their impact on sales and returns.

**Queries**:
* **Data Merging**: The Python queries used to merge the datasets are **not publicly available**.
* **Data Cleaning and Analysis**: The Python queries used to consolidate and analyze data can be found [here.](https://github.com/andrealopezp/....ipynb)
* **Interactive Reporting Dashboard**: An interactive Tableau dashboard used to explore and report data can be found [here.](https://public.tableau.com/app/profile/andrealopezp/viz/eMoney/DashboardIntro)
* **Customer Segmentation**: The Python queries used to segment customers can be found [here.](https://github.com/andrealopezp/....ipynb)
* **Predictive Model**: The Python queries used to build a predictive model are **not publicly available**.
* **Targeted Marketing Strategy**: The Python queries used to propose a targeted marketing strategy are **not publicly available**.


If you are interested in accessing the **complete project**, including all detailed sections, please feel free to **reach out directly**. I am happy to provide full access upon request.\
**Contact**: [LinkedIn](https://www.linkedin.com/in/andrealopezp)

# Data Structure & Initial Checks

eMoney's database structure as seen below consists of five tables:  customer_commercial_activity, customer_products, customer_sociodemographics, sales, and product_description, with a total row count of 2,997,300 records.

![eMoney Dataset ERD](/Images/Dataset_ERD.png)

1. **Customer Commercial Activity**: Information about customer acquisition channels, their engagement with the app, and their behavior over time. By analyzing the combination of entry channel, entry date, segment and app activity, we can extract customer acquisition insights, classify customers into different groups, understand customer engagement and retention, and identify seasonal patterns/trends.
2. **Customer Products**: Information about customer purchasing habits, which provide an understanding of customer behavior and preferences. This information allows to refine commercial strategies and customize customer offers.
3. **Customer Sociodemographics**: Information about customer demographics (age, gender, income) and geographic location. By analyzing these details, we can profile our ideal customers.
4. **Sales**: Each unique sales ID represents a sales transaction, including customer ID, sales date, and net margin. With these details, we can extract commercial insights such as customer profitability, sales trends and sales performance which allows us to refine customer segmentation, improve pricing, and enhance profitability.
5. **Product Description**: Information about individual products, including product ID, product name, and product category. We can evaluate which products are most popular and profitable to optimize sales efforts and enhance overall profitability.



# Executive Summary

### Overview of Findings
After peaking in October 2018, eMoney's sales have continued to decline, with significant drops in 2019. The analysis reveals that Madrid is the top city in revenue generation (over 30% in 2019). Additionally, popular products—such as eMoney and payroll accounts, debit cards, and pension plans— are key drivers of long-term customer retention, maintaining loyalty rates between 80% and 100%, with active engagement fueling repeat purchases. New customer acquisition is strongest for top-rated products in July, September and October 2018, while being weaker in June 2018 and recent months. Certain products, like eMoney accounts and debit cards, face higher churn rates compared to others. Trends show steady revenue growth, driven by seasonal peaks and consistent customer preferences, suggesting opportunities for targeted marketing and product-focused strategies.

Below is the overview page from the Tableau dashboard and more examples are included throughout the report. It can be found [here.](https://public.tableau.com/app/profile/andrealopezp/viz/eMoney/DashboardIntro)

![Dashboard](/Images/Dashboard.png)



# Insights Deep Dive
An analysis has been carried out on eMoney available data between January 2018 and May 2019 and useful observations have been extracted for making strategic decisions. Below we list the ideas:

- **1. Products Popularity and Customer Preferences**
![Dashboard](/Images/1.png)
  - On average eMoney account has proven to be the flagship product among customers, with 55.71% of the total, followed by debit cards (11.59%), pension plans (5.03%) and payroll (4.97%) during 2019. In contrast, products such as short-term deposits, loans, and eMoney+ account did not register any market penetration.
  - The high implementation percentage of eMoney accounts suggests its popularity and predictive value of customer behavior, while the low implementation of other products such as securities or funds indicates their possible underutilization or focus on specific niches.

- **2. Customer Loyalty Across Top Products**
![Dashboard](/Images/2.png)
![Dashboard](/Images/2.2.png)
  - Retention for the top five products has remained stable, with rates between 80% and 100% from October 2018 to April 2019. However, in May 2019, there was a decline in retention. Especially for debit cards, both eMoney and payroll accounts, suggesting possible changes in policies or market conditions. In addition, retention for eMoney Crypto accounts (34.01%) and debit cards (47.69%) were slightly below average, which may indicate a greater willingness of customers to cancel or change this product. In contrast, pension plans (from 82.56% in April decreases to 70.69% in May) and payrolls (from 95.78% decreases to 65.78% in May) maintain a more stable retention.

- **3. New Customer Acquisition by Product**
![Dashboard](/Images/3.png)
    - There were significant peaks in July 2018, September 2018 and October 2018, likely driven by marketing campaigns, while months such as June 2018 and from December 2018 to April 2019 had very low acquisitions, possibly due to seasonality or lack of promotion.
    - Among the top-rated products, eMoney accounts has led sales throughout the entire period, followed by debit cards and payroll accounts. However, eMoney accounts that were a must-have product for new customers, seem to not be so today. The product has shown a very pronounced drop in recent months, highlighting a drop in popularity that could be influenced by consumer trends, government regulations, company perception and reputation or market competitors.
    - Pension plans and payrolls have a lower share, indicating that they might be less attractive to new customers or targeted at specific segments.

- **4. Product Churn by Month**
![Dashboard](/Images/4.png)
    - Product churn changed month to month, with notable peaks in December 2018 and January 2019, suggesting possible changes in retention policies. eMoney accounts and debit cards recorded the highest churn rates (over 1K customers), while products such as pension plans and payrolls showed more stable rates, suggesting higher loyalty.
    - In 2019, a decrease in churn was observed compared to the second half of 2018, possibly as a result of adjustments in retention policies.

- **5. Trends in Product Revenue Over Time**
![Dashboard](/Images/5.png)
  - eMoney accounts have been the main revenue generator in several periods, especially between 2015 and 2017, showing significant spikes compared to other products, which remained stable in revenue. Towards the end of 2018 and beginning of 2019, there was an overall decrease in revenue, which could indicate changes in demand or business strategies.



# Recommendations
- **1. Products Popularity and Customer Preferences**
    - **Products Review**: Lack of penetration of certain products in the last year highlights the need for a strategic review to improve their offer and competitiveness.
    - **Flagship Product**: Focus resources on promoting eMoney accounts.
    - **Cross-selling and Upselling Strategy**: Leverage eMoney accounts customer base to offer complementary products.

- **2. Customer Loyalty Across Products**
    - **Loyalty Drop Analysis & Customer Feedback**: Examine the reasons contributing to the decrease in loyalty. Conducting surveys to customers who abandoned products to understand their reasons and understand their product expectations.
    - **Competition and Market Analysis**: Investigate whether competitors introduced new offers or modifications that may have influenced customers' decision to cancel products. If necessary, readjust conditions of the products.
    - **Value Proposition Review**: Enhance the value proposition of products to increase retention and reduce churn.

- **3. Acquisition of New Products by Current Customers**
  - Marketing Campaign Analysis.
  - **Seasonality Analysis**: Analyze whether seasonality is impacting the acquisition of new products. If confirmed, it would be advisable to offer promotions in low months.

- **4. Product Churn by Month**
  - **Causes of Churn**: Investigate the factors that drive churn spikes. Conducting surveys to customers who abandoned products to understand their reasons and what motivated their decision.
  - **Customer Segmentation**: Segment customers into groups based on their behavior and needs. It will enable customization of offers for each group.
  - **Churn Monitoring**: Implement a continuous monitoring system to identify churn in real time to anticipate changes and be effective.

- **5. Trends in Product Revenue Over Time**
  - **Demand Analysis**: An in-depth analysis to understand reasons that have influenced these results (e.g. specific campaigns, changes in offerings or variations in consumer behavior). Being aware of such details could help replicate success in the future.
  - **Trend Monitoring**: Implement a continuous monitoring system to identify trends in real time to anticipate changes in demand.



# Assumptions and Caveats
Throughout the analysis, multiple assumptions were made to manage challenges with the data. These assumptions and caveats are noted below:
* **Products and their corresponding details:** Most entries were empty or incomplete, we assume that these variables are relatively new and data will be gradually updated. Due to incomplete product data, the analysis might be skewed or less accurate. Moreover, if product attributes are missing, personalized recommendations or campaigns based on customer history may be less effective.
    * It would be necessary to consult and/or verify with the Data Collection Team to better understand the situation and, if necessary, agree on a solution that avoids missing data in the future.
* **Sales Entry Channels Review:** The dataset considers different sales channels. It would be advisable to review the full list and evaluate if they are adequately representing the market or if it should be adjusted.
* **External Influences:** It is essential to keep in mind that factors such as consumer trends, government regulations, company perception and reputation, geographic location, economic changes or competitive actions could have a direct impact on customers decisions. Therefore, on revenue. Obtaining updated data on a regular basis is key to ensuring that the correct product and price assessment and its adjustment to reality is as accurate as possible over time.



# Tech Stack
- **Programming Language**: Python
- **Data Analysis**: Pandas, NumPy, Scikit-Learn
- **Data Visualization**: Matplotlib, Seaborn, Tableau
- **Tools**: Jupyter Notebooks
- **Machine Learning - Supervised Learning**: XGBoost
- **Model Evaluation**: Accuracy, Precision, Recall, F1-score, Confusion Matrix



# Data Source
In this analysis, data was obtained from an educational institution and cannot be shared due to confidentiality agreements. Therefore, the data used in this project is not publicly available.

Prior to beginning the analysis, several checks were performed for quality control and familiarization with the datasets. The Python queries used are **not publicly available**.
