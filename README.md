# Customer-Behavior-Analysis
Understanding customer behavior is critical to driving long-term business success. For this project, I conducted a Customer Behavior Analysis using a dataset containing detailed information on customer demographics, lifetime value, churn probability, and purchase patterns. 
### Problem Statement

Despite having a large and seemingly valuable customer base, the company lacked visibility into key customer behavior metrics such as lifetime value, purchase activity, and churn risk. This limited the brand’s ability to identify which customers were most profitable, which were at risk of churning, and where to focus retention efforts. Without a structured analysis of customer behavior, the business risked revenue loss due to undetected churn trends and missed opportunities to nurture high-potential customers.

### Aim of Project

- **Identify customer segments based on spending and engagement**
    
    To classify customers into value-based groups (e.g., High, Medium, Low) using Lifetime Value and purchase patterns.
    
- **Understand churn risk across customer categories**
    
    To evaluate the churn probability of customers, especially high-value ones, and determine which segments are most at risk of leaving.
    
- **Discover key behavioral trends and patterns**
    
    To explore how factors such as region, product preference, and launch dates affect customer behavior and loyalty.
    
- **Generate actionable insights for retention strategies**
    
    To uncover data-driven opportunities that can help reduce churn, increase customer lifetime value, and improve marketing focus.
    

### **Data Cleaning & Preprocessing**

- **Cleaned and formatted the data**:

       Converted Launch_date and Peak_sales_date to Excel-recognized date formats.

        Removed duplicates and checked for missing values.

- **Created new analytical columns**:
    
    Categorized Lifetime Value into “High”, “Medium”, and “Low”.
    
    Grouped churn probability into “High Risk”, “Medium Risk”, and “Low Risk”.
    
    Classified customer activity levels using average purchases per period.
    
- **Churn prediction using Python**

       Used Python to predict if a customer is likely to stop buying or not, based on their behavior.

- **Analyzed customer distribution**:

       Calculated what percentage of customers were in each group.

- **Filtered and segmented key targets**:
    
    Used Excel filters to isolate customers who were both **High Value** and **High Churn Risk**
    
           
    

### Analysis

**Purchases by Region**

- North America and Europe had the highest number of purchases.
- Africa and South America recorded fewer purchases, indicating potential underperformance or lower customer reach in these regions

**Lifetime Value by Region**

- Customers in North America have the highest average lifetime value, followed closely by Europe.
- Asia and South America have the lowest lifetime value.

![image.png](attachment:3aff5bab-5a0e-4d76-bed3-523d4df2849e:image.png)

**Churn Over Lifetime**

- Low-value customers show significantly higher churn probability.
- High-value customers have lower churn,

![image.png](attachment:58f3de18-8fae-460e-96c1-ea5867c0d8a3:image.png)

**Frequently Purchased Categories**

- Clothing is the most purchased product category.
- Home and Electronics follow, while Books are the least purchased.

**Frequently Purchased Categories by Season**

- Most product categories, especially Clothing and Home, see consistent purchases across all seasons.
- Slight spike in Electronics during Winter (possibly linked to holiday sales).

**Season with the Most Purchases**

- Winter and Spring are the seasons with the highest number of purchases.
- Fall has the least.

![image.png](attachment:835e606c-525e-4e89-9d0e-428d08e8bcd7:image.png)

**Retention Strategy with the Most Purchases**

- Customers under Discount strategies made the highest number of purchases.
- Followed by Email Campaigns, while Loyalty Programs had the least purchases.
- Indicates discounts drive short-term sales, but long-term value still needs analysis.

**Churn in Region**

- Asia and Europe show the highest churn rates.
- South America has the lowest churn, despite having low purchases and value

![image.png](attachment:cef84f6d-5f5e-4dfc-bf7c-903979d17d9e:image.png)

**Churn probability prediction**

After cleaning and preparing the dataset, I used a Random Forest Classifier to predict whether a customer is likely to churn (stop buying) based on their purchase behavior and demographics.

The model achieved an accuracy of 48.35%, which means it correctly predicted customer churn in about half of the cases. While this shows that the model learned some patterns, its performance is not strong enough for business decisions yet.

Here’s a breakdown of what the model found:

- Out of 969 customers who actually churned, only 442 were correctly identified.
- It also mistakenly predicted churn for 506 customers who didn’t churn.
- The recall score for churn was 46%, which means the model captured less than half of the customers who were likely to churn.

![image.png](attachment:15aaf139-7ffd-474d-8d28-625cf12e5edf:image.png)

![image.png](attachment:c119ff14-af33-4a26-ad7e-6fd03f811e48:image.png)

North America customers had the highest lifetime value and purchase volume.

Low-value customers made up most of the churn risk, but 30% of high-value customers were still at risk, highlighting a retention gap.

Winter and Spring drove the most purchases, especially for Clothing and Electronics.

Discounts increased purchases but had higher churn, while Loyalty Programs retained fewer but more valuable customers.

Customers acquired in recent years (2021–2022) had lower churn and higher value, possibly due to improved onboarding or better offers.

### Recommendation

- I noticed that about 30 to 40% of high-value customers are showing signs of churn. These are the customers the brand should really focus on keeping. I’d recommend launching targeted retention efforts like personalized offers, exclusive loyalty benefits, or win-back messages that make them feel valued.
- Based on the lifetime value and purchase data, North America and Europe are clearly performing well. I think the brand should keep investing in those regions. However, places like Asia and South America aren’t performing as strongly, so it might be helpful to dig into why that’s happening — maybe through surveys or local campaigns.
- I found that discounts bring in more purchases, but those customers tend to leave quicker. On the other hand, loyalty programs seem to keep high-value customers engaged. So I think a good strategy would be to start with discounts to bring people in, then move them into loyalty programs to keep them longer.
- Purchases were highest in Winter and Spring, which means these are the best times to push major campaigns or product launches. Fall was the lowest-performing season, so I think we could use that period for testing new strategies or warming up customers for the peak season.
- From the product categories, Clothing and Electronics were the most frequently purchased. I’d recommend continuing to promote these strongly. For less popular categories like Books, we might try bundling them with other products or targeting specific customer segments that would be more interested.
- Low-value customers had the highest churn risk. I think improving their first experience with better onboarding, maybe a welcome offer or guidance through their first purchase, could help turn them into more valuable, long-term customers.
- I also noticed that newer customers, especially those acquired in recent years, tend to have higher value and lower churn. This means that recent acquisition efforts are working, and we should continue tracking customers by their join date to improve how we bring them in and keep them engaged.
- During the analysis, I looked closely at churn probability across different customer segments. One thing that stood out was that even though low-value customers had a higher churn risk overall, a significant portion of high-value customers—about 30 to 40%—were also at risk of leaving. This is a concern because these are the customers who contribute the most to revenue. The business should set up automated alerts or tags for high-value customers with a high churn score. Offer them early access to sales, loyalty bonuses, or personalized check-ins to keep them engaged.****
