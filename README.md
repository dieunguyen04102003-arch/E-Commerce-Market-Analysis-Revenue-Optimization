# E-Commerce Market Analysis & Revenue Optimization

## I. Project Overview
This project demonstrates an end-to-end data analytics and marketing research workflow, transforming raw transactional records into actionable business strategies. The objective is to evaluate market trends, analyze competitor-driven promotional strategies, and uncover consumer behavior insights to optimize product lifecycles and maximize platform profit margins.

### 📊 Dashboard Preview
> <img width="1315" height="720" alt="image" src="https://github.com/user-attachments/assets/c7558b83-4589-4e9e-9796-809dba5716cc" />

Key research activities include:
* **Market Overview & Audience Segmentation:** Profiling consumers to identify high-value segments.
* **Promotional Strategy Evaluation:** Analyzing discount exploitation and its impact on margins.
* **Product Portfolio Expansion:** Identifying category growth trends to guide future product launching.
* **BI Dashboard Reporting:** Translating data into strategic recommendations for stakeholders.

---

## II. Dataset Summary
**Dataset Name:** `customer_behavior.xlsx`  
**Description:** The dataset contains 1,238 transaction records from an e-commerce platform, capturing essential consumer touchpoints:
- **Customer Demographics:** Gender, Subscription Status.
- **Purchase Behavior:** Purchase Amount (USD), Category, Discount Usage.
- **Shipping Preferences:** Shipping Type (Standard, Express, Free Shipping, Store Pickup).
- **Customer Feedback:** Review Ratings (1-5 scale) acting as a proxy for product satisfaction.

---

## III. Tools & Technologies
* **Data Validation & Review:** Microsoft Excel (Advanced Formulas, Pivot Tables, Data Validation, Charts).
* **Database Querying:** SQL (Aggregations, Joins, Group By) for extracting business metrics.
* **Data Processing & EDA:** Python (Pandas, NumPy) for deep consumer profiling.
* **Business Intelligence:** Power BI (Interactive Dashboard, DAX basics) for executive reporting.
* **Market Research Tools:** Google Trends, Competitor Matrix Frameworks.

---

## IV. Project Workflow

### 1. Data Loading & Validation
* Imported raw data and verified data types and structures.
* Utilized Excel and Python to cross-check total record counts and standard ranges.

### 2. Data Cleaning & Wrangling
* Handled missing values and standardized inconsistent formats.
* Validated outlier transactions to ensure data integrity before running market queries.

### 3. Market Insights & Key Findings

#### 🎯 Insight 1: Promotional Strategy & Margin Optimization (The Discount Paradox)
* **Finding:** Subscribers make up only 27% of the user base but consume 62% of all discounts without driving a higher Average Order Value (AOV) ($59 vs $58).

| SQL Query | Power BI Dashboard |
|:---:|:---:|
| ![Discount SQL](https://github.com/user-attachments/assets/52a9a8bc-563d-4f38-9f83-c25b67d951ef) | ![Discount Dashboard](https://github.com/user-attachments/assets/6248a55a-12f4-43ec-a210-75ff4256d225) |

* **Market Action:** Current promotions are heavily eroding margins on existing loyalists without growing basket size. Recommend transitioning from direct discounts to a **Points-Based Loyalty Program** to safeguard net profit margins.

#### 📈 Insight 2: Target Audience Segmentation & Product Line Expansion
* **Finding:** Male consumers dominate the Accessories category, generating 71% of total revenue (~$50K) in that sector.

| Metric | Male + Accessories | Female + Accessories |
| :--- | :--- | :--- |
| Customers | 848 (69%) | 390 (31%) |
| Total Revenue | ~$50K (71%) | ~$20K (29%) |
| Avg Revenue / Order | $59.41 | $60.76 |
| Total Sales | 800 (67%) | 400 (33%) |

**Power BI Visualizations:**

**Male + Accessories:**
![Male Accessories](https://github.com/user-attachments/assets/37a8ed50-f24c-4e56-8035-3385d45b0768)

**Female + Accessories:**
![Female Accessories](https://github.com/user-attachments/assets/cdf7f496-cffc-4aa0-84f8-2f6d892e6470)

* **Market Action:** Identify a significant product-market fit. Recommend expanding the men's accessory line (wallets, belts) for upcoming product rollouts and cross-selling them with clothing lines.

### 4. Product Funnel & Health Monitoring Concept

#### 📊 Product Funnel Optimization (User Journey)
To align this data with standard Product Analytics Frameworks, we map out the e-commerce purchase journey to identify drop-off points:
* **Funnel Stages:** `View Product` ➔ `Add to Cart` ➔ `Purchase (Non-Subscribed)` ➔ `Upgrade to Subscription`
* **The Friction:** 73% of users drop off before subscription conversion, despite maintaining a high purchase intent (AOV $58). The friction lies in the subscription value proposition, not the pricing.

#### 🚨 Proposed Automated Data Alerts (Product Health Monitoring)
| Alert Trigger | Threshold | Business Reason |
| :--- | :--- | :--- |
| **Subscriber Discount Abuse** | Over **65%** | Alerts Product Team when promos burn too much margin without increasing transaction volume. |
| **Category Rating Drop** | Below **3.5 / 5.0** | Signals potential quality friction or supply chain issues in specific product categories. |

---

## V. Conclusion & Future Outlook

### 🎯 Strategic Conclusion
This analysis successfully bridges raw metrics with consumer psychology. By addressing the **Discount Paradox** and capturing the **Male-Dominated Accessories Trend**, the platform can execute data-driven launching strategies, optimize inventory risk, and improve conversion metrics.

### 🔮 Future Research Directions
1. **Predictive Churn Modeling:** Building machine learning models via Python to identify at-risk subscribers early.
2. **RFM Customer Segmentation:** Developing advanced Recency, Frequency, Monetary (RFM) clusters for targeted database marketing.
