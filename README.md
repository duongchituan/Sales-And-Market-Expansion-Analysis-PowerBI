# 📊 Sales & Market Expansion Analysis (PowerBI)

---
![ChatGPT Image 13_27_57 23 thg 6, 2025](https://github.com/user-attachments/assets/2bb232ae-9c85-4725-8079-4247c7cd9f37)


Author: Duong Chi Tuan  
Date: May 2025  
Tools Used: Power BI  

---

## 📑 Table of Contents  
1. [📌 Background & Overview](#-background--overview)  
2. [📂 Dataset Description & Data Structure](#-dataset-description--data-structure)  
3. [🧠 Design Thinking Process](#-design-thinking-process)  
4. [📊 Key Insights & Visualizations & Recommendations](#-key-insights--visualizations)  

---

## 📌 Background & Overview  

### Objective:
### 📖 What is this project about? 
 
This project provides a Power BI dashboard to support strategic decision-making. The objective is:  

- Understand company-wide sales performance

- Identify top products & regions for market expansion

- Support senior management in selecting strategic products 

### 👤 Who is this project for?  

✔️ Senior managers & business decision-makers  

✔️ Data analysts supporting executive insights  

###  ❓Business Questions:  
✔️ Which products generate the most revenue and profit?  

✔️ What are the top-performing regions or markets?  

---

## 📂 Dataset Description & Data Structure  

### 📌 Data Source  
- Source: Kaggle  
- Size:
  - The Orders table contains 51,290 records
  - The People table contains 13 records
  - The Returns table contains 1,172 records  
- Format: .csv  

### 📊 Data Structure & Relationships  

#### 1️⃣ Tables Used:  
The dataset consists of three tables:  
<details>
<summary><strong>📊 Table 1: Orders - Contains detailed transaction and customer information</strong></summary>

| Column Name     | Data Type | Description                                         |
|-----------------|-----------|-----------------------------------------------------|
| Order ID        | VARCHAR   | Unique identifier for each order.                  |
| Order Date      | DATE      | Date when the order was placed.                   |
| Ship Date       | DATE      | Date when the order was shipped.                  |
| Ship Mode       | VARCHAR   | Shipping method used for delivery.                |
| Customer ID     | VARCHAR   | Unique identifier for each customer.              |
| Customer Name   | VARCHAR   | Full name of the customer.                        |
| Segment         | VARCHAR   | Customer segment (e.g., Consumer, Corporate).     |
| City            | VARCHAR   | City where the order was placed.                  |
| State           | VARCHAR   | State where the order was placed.                 |
| Country         | VARCHAR   | Country where the order was placed.               |
| Postal Code     | VARCHAR   | Postal code of the shipping address.              |
| Market          | VARCHAR   | Market region (e.g., APAC, EMEA).                 |
| Region          | VARCHAR   | Geographical region of the order.                 |
| Product ID      | VARCHAR   | Unique identifier for each product.               |
| Category        | VARCHAR   | Product category (e.g., Furniture, Office Supplies). |
| Sub-Category    | VARCHAR   | Sub-category of the product.                      |
| Product Name    | VARCHAR   | Name of the product ordered.                      |
| Sales           | DECIMAL   | Revenue generated from the order.                 |
| Quantity        | INT       | Number of items ordered.                          |
| Profit          | DECIMAL   | Profit earned from the order.                     |

</details>
<details>
<summary><strong>📦 Table 2: Returns – Stores data on returned orders</strong></summary>

| Column Name | Data Type | Description                                           |
|-------------|-----------|-------------------------------------------------------|
| Returned    | VARCHAR   | Indicates whether the order was returned (e.g., 'Yes' or 'No'). |
| Order ID    | VARCHAR   | Unique identifier for each order.                    |

</details>

<details>
<summary><strong>🧑‍💼 Table 3: People – Holds information about sales representatives</strong></summary>

| Column Name | Data Type | Description                                           |
|-------------|-----------|-------------------------------------------------------|
| Person      | VARCHAR   | Name of the salesperson.                             |
| Region      | VARCHAR   | Geographic region where the salesperson operates.    |

</details>

#### 2️⃣ Data Relationships:  

![image](https://github.com/user-attachments/assets/e16fece0-207e-48c9-81f4-ce7f92fc9958)


## 🧠 Design Thinking Process  

Explain the step-by-step approach taken to solve the problem.  

1️⃣ Empathize  

![image](https://github.com/user-attachments/assets/9a174114-56d7-4db5-908c-f8bc29458b63)

![image](https://github.com/user-attachments/assets/a1c30bda-9210-452c-ae6a-a097c89332d8)


2️⃣ Define point of view  

![image](https://github.com/user-attachments/assets/f8095e2f-de5a-4c4e-9544-2c587495725b)

3️⃣ Ideate  

![image](https://github.com/user-attachments/assets/3c861a6a-e804-44dc-85d5-6bc33c65d1b1)

![image](https://github.com/user-attachments/assets/5f7e537a-a3a5-405c-abf2-ec70395024c1)

---

## 📊 Key Insights & Visualizations  

### 🔍 Dashboard Preview  

#### 1️⃣ Overview 

![image](https://github.com/user-attachments/assets/ad0862a1-f30d-459d-8344-fa3a65757af8)  

From 2011 to 2014, the company maintained a strong growth trajectory in both revenue and profit. In 2014 alone, revenue grew significantly (+24% vs. 2013). However, profit margin showed a slight decline across all three key markets (APAC, EU, and US), indicating some underlying issues with profitability efficiency.  

![1](https://github.com/user-attachments/assets/be44600c-98c9-47d7-9c5d-aa8d50263cfc)


📌 Analysis:  

 📈 Revenue increased, but profit didn't keep up
Profit margin peaked in 2013 (11.97%), not in 2014 when revenue was highest. This suggests that as revenue grew, costs also rose—implying the company may be trading margin for scale.

🚚 Increase in high-cost shipping methods
In 2014, there was a notable rise in orders using expensive shipping methods such as First Class and Same Day. This shift significantly raised logistics costs, which outpaced gross profit growth and eroded overall profitability.

🛍️ Higher share of low-margin product categories
In particular, Office Supplies—a category with relatively low profit margins—experienced a surge in order volume. This shifted the product mix toward less profitable items, reducing the company's overall margin efficiency.  

![2](https://github.com/user-attachments/assets/826e0533-f500-446f-8e68-1987362e13d3)

🔁 Slight increase in return rate in APAC and US
Compared to 2013, the return rate rose in key markets like APAC (4.99% → 5.04%) and US (5.90% → 6.12%) in 2014. While the change is small, when combined with expensive shipping and a weak product mix, it added to costs and reduced net revenue.  

![3](https://github.com/user-attachments/assets/9509d04d-c6b4-4c28-bca9-6d7f80448e78)

⚠️ Three factors combined to reduce profit margin
The margin drop in 2014 was not caused by a single issue, but by a combination of:

(1) increased use of high-cost shipping,
(2) a rise in low-margin product share,
(3) higher return rates.
→ These factors together exerted cost pressure and squeezed profitability.

🌍 EU – High revenue but also the highest return rate (6.18%)
Although EU is one of the top contributors in both revenue and profit, it also has the highest return rate among all regions. This signals potential issues with product quality, after-sales service, or customer experience—and could hurt long-term margins if not addressed.

🪑 Furniture – Underperforming product category
Among the three main categories (Technology, Office Supplies, Furniture), Furniture generated the lowest profit. It may exist for catalog diversity, but in reality, it's dragging down the company's overall performance.  

💡 Recommendation:  

- Review shipping policies, especially for orders using First Class and Same Day. Consider applying minimum order thresholds or extra fees to manage logistics costs.

- Restructure the product mix to reduce dependency on low-margin items (like Office Supplies) and promote cross-selling with higher-performing products.

- Investigate product quality and customer experience in the EU region, where the return rate is highest. Prioritize after-sales improvements or redesign return policies to limit loss.

- Reassess or scale down the Furniture category if it continues to underperform in upcoming periods.

- Track profit per order more closely, not just overall revenue or profit, to quickly detect operational inefficiencies.

#### 2️⃣ Dashboard 2 Preview  

![image](https://github.com/user-attachments/assets/57c30008-b5d0-49ba-ae73-cf41a7478857)

📌 Analysis:   

🇨🇦 Canada – Small market with exceptionally high margin
Despite contributing only $0.05M in revenue and $0.01M in profit, Canada recorded the highest profit margin (27.59%) in the entire dataset.
⚠️ However, due to the small sample size, just a few large transactions could create an inflated margin.
→ Further validation at the SKU/product level is needed to confirm its potential.

🌍 Africa – A small but surprisingly efficient market
With $0.59M in revenue and $0.07M in profit, Africa reached a profit margin of 11.48%, aligning with the company average.
→ This suggests potential for niche market expansion with controlled cost and focused targeting.  

🖨️ Copiers – Key profit driver in Canada
Copiers contributed 38% of total profit in Canada, making it a standout product for scaling efforts in this market.

📱 Phones – High revenue, modest efficiency
While it generated the highest revenue ($1.37M) across all SKUs, its profit margin is only 13.07%.
→ A reassessment is needed to investigate operational or pricing inefficiencies.

📄 Paper & Labels – Low-volume, high-margin SKUs
Although small in revenue, these SKUs deliver 25%+ profit margins, suggesting strong potential if scaled carefully.

💡 Recommendation:  

- Scale up operations in Canada, focusing on high-margin categories such as Copiers, Office Supplies, and Technology.
→ A lean, margin-driven strategy could prove highly effective here.

- Explore niche expansion in Africa with selective investment in high-margin SKUs. Prioritize low-risk, cost-effective channels to test the waters.

- Re-evaluate the overall SKU mix to reduce dependency on high-revenue but low-margin products like Phones, and shift toward smaller, high-efficiency items such as Paper and Labels.


---


