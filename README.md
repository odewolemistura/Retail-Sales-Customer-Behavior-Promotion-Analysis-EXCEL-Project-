# Introduction  

This **Retail Sales, Customer Behavior & Promotion Analysis** report is designed to help retail businesses make data-driven decisions on revenue growth and promotional strategies.  

The study explores:  
- Transaction patterns  
- Customer categories  
- Payment methods  
- Store types  
- Seasonal sales  
- Promotion impacts  

Its purpose is to uncover insights into purchasing behavior, evaluate store and promotion performance, and provide actionable guidance for optimizing sales and enhancing customer engagement.  

# Problem Statement  

Retail businesses today operate in a highly competitive market where customer preferences shift quickly, promotions must be well-targeted, and store performance varies across locations and seasons. While large volumes of transaction data are available, the absence of a structured analysis limits the ability to clearly see how customer behavior, promotional activities, and seasonal patterns drive overall revenue.  

The business faces several challenges:  
- Identifying which customer groups generate the highest value.  
- Comparing the impact of discounts and promotions on sales.  
- Understanding how purchasing behavior varies by payment method and spend level.  
- Assessing differences in performance across cities, store types, and seasons.  

This project addresses these challenges by transforming raw retail transaction records into meaningful insights. Through the use of **Excel** and **Power Query**, the analysis highlights revenue trends, customer spending patterns, and the effectiveness of promotions, equipping retail managers with the information needed to strengthen decision-making, improve promotional planning, and maximize sales opportunities.  

# Key Posing Business Questions  

To maximize strategic value, this analysis was framed from the perspective of retail decision-makers such as the **Sales Director**, **Marketing Manager**, and **Store Operations Lead**. The following questions guided the KPIs, measures, and dashboard design:  

- Which customer categories contribute the most to overall revenue, and how do their purchasing behaviors differ?  
- What is the average number of items purchased per transaction across customer segments?  
- Which spend ranges occur most frequently, and what do they reveal about customer spending power?  
- How are payment methods distributed, and do certain methods indicate different customer preferences?  
- Do discounts meaningfully increase revenue compared to non-discounted sales?  
- Which promotion types (e.g., BOGO, product discounts) are most effective in driving higher transaction values?  
- Which store types and city locations generate the highest revenue contributions?  
- How do monthly sales trends evolve across the year, and what seasonal differences are most significant?  
- How do overall KPIs — total transactions, total revenue, and average cost — reflect retail performance at scale?  

# Dataset Overview  

The dataset contains **1 million retail transactions** collected from various store types and cities. It captures detailed information about customer purchases, payment methods, discounts, and promotions, making it suitable for analyzing sales performance, customer behavior, and marketing effectiveness.  

- **Transaction_ID** – Unique identifier for each purchase.  
- **Customer_Name** – Name of the purchasing customer.  
- **Product** – List of items bought in the transaction.  
- **Total_Items** – Quantity of items purchased.  
- **Total_Cost** – Monetary value of the transaction.  
- **Date** – Timestamp of the transaction (used to derive year, month, and season).  
- **Payment_Method** – Mode of payment (cash, credit card, debit card, mobile).  
- **City** – Geographic location of the store.  
- **Store_Type** – Store classification (e.g., supermarket, convenience store, department store).  
- **Discount_Applied** – Indicator showing if a discount was applied.  
- **Customer_Category** – Classification of customers (e.g., student, retiree, professional).  
- **Season** – Season of the purchase (spring, summer, fall, winter).  
- **Promotion** – Type of promotion applied (e.g., BOGO, product discounts, or none).  

# Data Preparation  

To ensure accuracy and usability, the dataset underwent a series of **cleaning and transformation steps** before analysis. The process was carried out in **Power Query** and **Excel**, focusing on removing inconsistencies, deriving new fields, and preparing the data for visualization.  

### Key Steps Taken:  
- Removed duplicates to eliminate repeated transactions.  
- Extracted date components (**date, year, and month name**) from the original timestamp for time-based analysis.  
- Created a **spend range column** by grouping transaction values into intervals for customer segmentation.  
- Standardized fields such as **customer categories, store types, and payment methods** to ensure consistency.  
- Calculated key measures (KPIs) including **total revenue, average cost per transaction, average items per transaction, and transaction counts**.  
- Loaded the cleaned dataset into **Excel** for pivot table and pivot chart modeling.  

# Measures (DAX)  

**Description:**  
Contains calculated measures created using **DAX in Power Pivot** to define key retail KPIs and evaluate sales performance. These measures form the backbone of the dashboard, providing insights into revenue generation, transaction activity, customer purchasing behavior, and average spend.  

**Fields:**  
- Total Cost  
- Total Transaction  
- Average Cost  
- Average Items per Customer Category  

**Purpose:**  
Delivers core summary metrics that enable data-driven analysis of retail operations. These measures help stakeholders monitor **revenue growth**, compare **customer buying patterns**, track **transaction volume**, and assess **spending trends**, supporting better decisions around **promotions, store performance, and customer engagement**.  

# Data Analysis & Visualization  

The dashboard is structured into two main pages, each focusing on specific retail objectives and delivering practical insights for sales managers, marketing teams, and business decision-makers.  

## Page 1: Retail Sales, Customer Behavior & Promotion Analysis  

**Business Goal:**  
Analyze customer transactions, spending, and payment habits to understand key sales drivers.  
 PICTURE

 # Key Metrics (Top of Page): Total Transactions, Total Revenue, Average Items per Customer Category  

Provide a high-level snapshot of overall sales activity, customer purchasing behavior, and revenue contribution. They help quickly assess business performance and customer engagement across different shopper groups.  

- **Total Cost (Revenue):** Represents the overall value of all completed transactions. It highlights the total income generated and serves as the primary measure of sales performance.  
- **Average Items per Customer Category:** Shows how many items customers typically purchase within each demographic segment. This metric helps uncover spending habits and shopping preferences across different customer groups.  
- **Total Transactions:** Counts the number of completed purchases. It provides insight into transaction volume and customer activity over time.  

Together, these KPIs offer a snapshot of customer behavior and sales activity, helping stakeholders identify the key drivers of revenue and transaction frequency.  

---

## Visuals  

- **Sales by Customer Category (Bar Chart):** Breaks down sales by shopper segments (e.g., Student, Homemaker, Professional), making it easy to compare category-level contributions to total revenue.  
- **Customer Spend Range (Column Chart):** Groups purchases into predefined spending brackets, highlighting how frequently customers spend within specific ranges. This helps assess transaction size distribution.  
- **Sales Trend Over Time (Line Chart):** Tracks revenue across months, allowing stakeholders to detect seasonal demand patterns, peak sales periods, and potential off-season slowdowns.  
- **Average Items per Transaction (Bar Chart):** Displays the average quantity of items purchased across different customer categories, showing which groups typically buy more per visit.  
- **Payment Method Distribution (Pie Chart):** Shows the share of transactions across cash, debit card, credit card, and mobile payment, giving insights into customer payment behavior and preferred channels.  

---

## Slicer: Year  

The dashboard includes a **Year** slicer that allows users to filter and interact with sales data dynamically across different time periods.  

- **Year** enables users to examine annual sales trends, compare performance across multiple years, and identify shifts in customer behavior or promotion effectiveness over time.  

This interactive filter ensures that KPIs, charts, and visuals adapt instantly, giving decision-makers a flexible view of sales performance. By narrowing the focus to specific years, users can detect seasonality, evaluate yearly growth, and align strategies with evolving retail trends.  

---

# Page Two: Promotion & Store Performance Analysis  

**Business Goal:**  
Evaluate how discounts, promotions, store types, and locations impact sales performance.  

PICTURE

# Key Metrics (Top of Page): Total Transactions, Total Revenue, Average Cost per Transaction  

These KPIs summarize store and promotion outcomes, giving a quick snapshot of overall sales activity, revenue generation, and how much customers typically spend per purchase. They form the foundation for evaluating how promotions, locations, and store formats influence performance.  

- **Total Cost (Revenue):** Indicates the total sales generated across all stores, promotions, and discounts. It shows the financial impact of retail operations.  
- **Average Cost:** Measures the mean transaction value, offering insight into how much customers typically spend per purchase. It’s useful for tracking promotion effectiveness and store performance.  
- **Total Transactions:** Tracks the number of purchases across all stores and time periods, reflecting overall activity levels and customer engagement.  

Together, these KPIs help decision-makers assess how discounts, promotions, and store formats affect sales performance and customer spending behavior.  

---

## Visuals  

- **Discount Impact on Revenue (Pie Chart):** Shows the revenue split between discounted and non-discounted purchases, helping to measure the financial contribution of discounts to overall sales.  
- **Promotion Effectiveness (Column Chart):** Compares the average transaction value across different promotion types (e.g., BOGO, Discounted Items, No Promotion), revealing which promotional strategy drives higher customer spending.  
- **Sales by City (Map Visualization):** Displays revenue distribution across cities, providing a geographic view of store performance and highlighting key urban markets.  
- **Store Type Revenue (Bar Chart):** Breaks down sales by store format (e.g., Supermarket, Pharmacy, Convenience Store), making it clear which store types generate the most revenue.  
- **Seasonal Sales Analysis (Column Chart):** Analyzes revenue by season, offering insights into how customer demand fluctuates across spring, summer, fall, and winter.  

---

## Slicer: Year  

The dashboard includes a **Year** slicer that allows users to filter and interact with sales data dynamically across different time periods.  

- **Year** enables users to examine annual sales trends, compare performance across multiple years, and identify shifts in customer behavior or promotion effectiveness over time.  

This interactive filter ensures that KPIs, charts, and visuals adapt instantly, giving decision-makers a flexible view of sales performance. By narrowing the focus to specific years, users can detect seasonality, evaluate yearly growth, and align strategies with evolving retail trends.  

---

# Key Analysis Findings  

The analysis of the retail dataset produced several insights into customer behavior, sales performance, and promotional effectiveness:  

### 1. Revenue Performance and Seasonal Trends  
- Total revenue reached **$52.46M** across **1.0M transactions**, with a steady average transaction cost of **$52.46**.  
- Monthly sales revealed peaks in **March ($5.1M)** and **January ($5.08M)**, while **September ($3.92M)** and **June ($3.94M)** recorded the lowest sales. This highlights seasonality in customer demand.  

### 2. Customer Categories and Spending Habits  
- Spending was evenly distributed across customer categories, each contributing around **$6.5M** to revenue.  
- Average items per transaction remained stable across categories, at roughly **5.5 items**, showing little variation in basket size.  

### 3. Transaction Patterns and Spend Range  
- Most transactions fell between the **21–80 spend range**, each range accounting for about **210K transactions**, indicating consistent customer spending behavior.  

### 4. Payment Preferences  
- Payment methods were evenly split across **cash, debit card, credit card, and mobile payment**, each with around **250K transactions**, suggesting customers have diverse but balanced payment preferences.  

### 5. Discounts and Promotions  
- Sales were nearly equal between **discounted ($26.25M)** and **non-discounted ($26.21M)** transactions, showing discounts did not drastically alter overall revenue.  
- Average transaction values were very close across promotions: **BOGO ($52.42)**, **Discount on Selected Items ($52.38)**, and **None ($52.57)** — indicating limited variation in customer spending regardless of promotion type.  

### 6. Geographic and Store Performance  
- Revenue was evenly spread across major cities, each generating around **$5.2M**, with no single city dominating sales.  
- Store types contributed similar revenue levels (~**$8.7M each**), with **Pharmacies ($8.77M)** and **Supermarkets ($8.76M)** slightly ahead.  

### 7. Seasonal Revenue Insights  
- Sales were consistent across seasons, with **Fall ($13.14M)** recording the highest revenue and **Winter ($13.08M)** the lowest.  
- However, the difference between seasons was minimal, suggesting year-round steady demand.  

**Overall Insight:** Customer purchasing behavior, store performance, and seasonal sales remained remarkably balanced across categories, cities, store types, and promotions. While discounts and promotions had minimal impact on average transaction values, revenue was primarily driven by transaction volume rather than promotional strategies or customer segmentation. This suggests opportunities lie in expanding transaction counts (e.g., through loyalty programs or cross-selling) rather than relying heavily on discounts.  

---

# Recommendations  

Based on the analysis of sales, customer behavior, promotions, and store performance, the following recommendations can help strengthen retail strategy and revenue growth:  

1. **Leverage Transaction Volume Growth Over Discounts:** Since discounts and promotions showed minimal impact on increasing average spend, focus should shift toward driving more transactions. Loyalty programs, bundle offers, and personalized product recommendations can encourage repeat purchases without relying on heavy discounts.  

2. **Target Seasonal Peaks for Optimized Promotions:** Sales were highest in **January** and **March**, suggesting natural demand spikes. Retailers can align major promotions and marketing campaigns around these periods to maximize impact while keeping discounts moderate in off-peak months.  

3. **Enhance Cross-Selling and Upselling Strategies:** With basket sizes averaging around **5.5 items** across all customer groups, retailers can introduce product bundles, “frequently bought together” deals, or tiered discounts to increase average items per transaction.  

4. **Diversify Payment Experience:** Since all payment methods were used almost equally, retailers should continue supporting multiple options while exploring emerging payment solutions (e.g., BNPL or digital wallets) to further enhance convenience and customer retention.  

5. **City-Specific and Store-Type Marketing:** Revenues were balanced across cities and store types, but subtle differences exist (e.g., Pharmacies and Supermarkets slightly higher). Tailored promotions based on local demographics or store format can help unlock incremental sales.  

6. **Strengthen Customer Segmentation and Personalization:** Although revenue distribution across customer categories was balanced, retailers should consider personalized marketing by age group and lifestyle segment to deepen engagement and create long-term loyalty.  

7. **Maintain Year-Round Engagement:** Seasonal revenue was relatively stable, showing steady demand throughout the year. Instead of heavy seasonal campaigns, retailers can focus on consistent engagement strategies such as rewards programs, customer appreciation events, and targeted promotions spread evenly across the year.  

**Overall Strategy:** By reducing overreliance on discounts and focusing on increasing transaction frequency, personalization, and steady engagement, the business can achieve sustainable revenue growth while keeping customer satisfaction high.  

---

# Limitations  

This analysis is based on a single dataset sourced from **Kaggle**, which may not fully capture real-world retail complexities. Customer names and product details were generalized, limiting deeper insights into individual purchasing patterns or product-level profitability. Additionally, the balanced distribution of sales across cities, store types, and customer categories suggests the dataset may have been simulated, which can restrict the applicability of findings to actual retail operations.  
