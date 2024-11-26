# Credit Card Customer Segmentation

### Objective

The goal of this assignment is to segment a credit card customer base into different groups for marketing and customer management purposes.

### Dataset

Use the following dataset available on Kaggle:
1. Title – Customer Credit Card Data
2. Author  - n.a., Fatemeh Habibimoghaddam (Owner)
3. Source – https://www.kaggle.com/datasets/fhabibimoghaddam/customer-credit-card-data   
(alternatively, can be found in `DSIF-course-material/python-material/data/1-raw/dsif8-assignment`)
3. License – Attribution 4.0 International (CC BY 4.0)

### Tasks
-   **Load and Explore the Data:** Start by loading the data and performing basic exploratory data analysis (EDA).
-   **Data Preprocessing:** Handle missing values, standardize the data, and prepare it for clustering.
-   **Clustering:** Apply clustering techniques like K-Means or Hierarchical Clustering to segment the customers. Optionally, use PCA to reduce dimensionality before clustering.
-   **Segmentation and interpretation:** Create meaningful and valid customer segments (at least 2, pick the number that works best for you based on your analysis) that can be leveraged for targeted marketing, customer management, and strategic decision-making.


## Overall Strategic Recommendations:
- Debt Management Programs for Cluster 0:
                          
- Focus on creating financial products that cater to individuals with high balances and reliance on cash advances. Introducing low-interest loans or consolidation products could improve customer satisfaction and retention.
Rewards-Based Spending Incentives for Cluster 1:

- Given their conservative financial behavior, create incentives such as reward points, cashback, or travel benefits that encourage increased spending without increasing financial risk.
Re-Engagement Campaigns for Cluster 2:

- Consider personalized marketing campaigns aimed at re-engaging this group through seasonal promotions, exclusive discounts, and installment purchase offers to drive higher engagement and loyalty.
Premium Services and Retention Strategies for Cluster 3:

- These are high-value customers with responsible credit habits. Retention strategies should focus on personalized offers, premium credit products, and loyalty programs that enhance their credit card experience and drive further purchases.

## Customer Segmentation Analysis and Insights for Targeted Marketing and Strategic Decision-Making

This analysis is based on the customer segmentation results derived from the KMeans clustering algorithm. The dataset was reduced using PCA, and clustering was performed based on key financial behaviors of customers, such as balance, purchases, payments, and credit limit. Four distinct customer clusters were identified, and their behaviors across several key features were visualized through boxplots, scatterplots, and a heatmap of cluster profiles.

### Cluster Overview

#### 1. **Cluster 0 (High Balance, Cash-Advance Users)**
   
- Balance: This cluster has very high balances (mean z-score = 1.72), significantly higher than the other clusters.
- Cash Advances: They rely heavily on cash advances (z-score = 1.89), which indicates financial stress or a need for liquidity.
- Credit Limit: They have a high credit limit (z-score = 1.07), but their usage patterns suggest they are maxing out their available credit.
- Minimum Payments: Higher than average minimum payments (z-score = 0.79), suggesting they might only be paying the minimum amount due on their credit cards.
- Purchases: Slightly below average purchases (z-score = -0.19), meaning they don’t use their credit cards heavily for purchases, instead relying on cash advances.

**Actionable Insights for Cluster 0:**

- Targeted Offers: Provide this segment with debt consolidation or low-interest personal loan offers to help manage their high balances and reduce reliance on high-interest cash advances.
- Financial Education: Offer credit management counseling or programs that encourage reducing balance levels and paying more than the minimum.
- Credit Limit Management: Consider reviewing their credit limit usage to ensure they're not consistently maxing out their cards. Proactive credit limit adjustment notifications may help these customers manage their credit more responsibly.

#### 2. **Cluster 1 (Low Balance, Financially Conservative)**
   
- Balance: This group has below-average balances (z-score = -0.69).
- Purchases: Slightly below-average purchase activity (z-score = -0.24).
- Cash Advances: They use very little to no cash advances (z-score = -0.34).
- Credit Limit: Their credit limits are also below average (z-score = -0.23).
- Payments: They consistently pay off their balances (high percentage of full payments z-score = 0.82), indicating they manage their credit responsibly.

**Actionable Insights for Cluster 1:**
- Loyalty and Rewards: Focus on rewards-based incentives to encourage this group to spend more, such as cashback offers or travel rewards for increased credit usage.
- Upsell Higher Credit Products: Offer this segment higher credit limits or premium credit cards that provide better rewards, given their responsible usage.
- Engagement Programs: Design campaigns to encourage more frequent spending, such as seasonal promotions or limited-time discounts to boost their relatively low purchase behavior.

#### 3. **Cluster 2 (Moderate Users, Low Activity)**
   
- Balance: Balances close to the average (z-score = -0.13), indicating a balanced credit usage.
- Purchases: Slightly below-average purchase behavior (z-score = -0.22).
- Cash Advances: Minimal use of cash advances (z-score = -0.19).
- Payments: Below-average payment activity (z-score = -0.25), meaning they may not be as engaged with their credit card usage.
- Credit Limit: This segment has below-average credit limits (z-score = -0.34).

**Actionable Insights for Cluster 2:**
- Engagement Campaigns: Focus on re-engagement strategies by offering exclusive deals or discounts to encourage more frequent spending.
- Installment Plans: Introduce installment payment options to help drive higher-value purchases, especially for those who might be hesitant to spend larger amounts at once.
- Educational Offers: Offer credit education programs to help them understand the benefits of responsible credit usage, and encourage higher credit engagement.

#### 4. **Cluster 3 (High Purchasers, Responsible Credit Users)**
   
- Purchases: This group is characterized by very high purchases (z-score = 1.66), making them a key revenue driver.
- Credit Limit: Their credit limit is above average (z-score = 0.97), giving them more financial flexibility.
- Payments: High payments (z-score = 0.92) indicate they are making substantial payments toward their balance, but they likely don't pay in full.
- Installment Purchases: They frequently use installment purchases (z-score = 1.44), indicating a strategic use of credit for large purchases.
- Percentage Full Payment: They make a higher-than-average portion of full payments (z-score = 0.57), showing responsible credit use.

**Actionable Insights for Cluster 3:**
- Premium Rewards: Offer premium loyalty programs or exclusive VIP perks such as priority customer service or early access to sales to retain this high-value group.
- Installment Plan Marketing: Promote installment payment programs or low-interest installment offers to encourage more spending on larger purchases.
- Higher Credit Products: Upsell them to higher credit limit products or premium credit cards, as they are likely to take advantage of enhanced credit features.
