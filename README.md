# 🛒 Customer Shopping Behavior Analysis

![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)
![SQL Server](https://img.shields.io/badge/Database-SQL%20Server-orange.svg)
![PowerBI](https://img.shields.io/badge/Power%20BI-Dashboard-yellow.svg)

---

## 📊 Project Overview
The **Customer Shopping Behavior Analysis** project focuses on understanding customer purchasing patterns using real-world transactional data from **3,900 purchases** across multiple product categories.  

The goal is to extract meaningful insights about:
- Spending behavior  
- Customer segmentation  
- Product performance  
- Subscription and discount usage  

These insights help guide **strategic business decisions** and improve **marketing, sales, and customer retention**.

---

## 📁 Dataset Summary
| Feature Type | Examples / Description |
|---------------|------------------------|
| **Demographics** | Age, Gender, Location, Subscription Status |
| **Purchase Details** | Item Purchased, Category, Purchase Amount, Season, Size, Color |
| **Behavioral Data** | Discount Applied, Promo Code Used, Previous Purchases, Frequency of Purchases, Review Rating, Shipping Type |
| **Rows** | 3,900 |
| **Columns** | 18 |
| **Missing Data** | 37 null values in Review Rating (handled with median imputation) |

---

## 🧹 Data Preprocessing (Python)
Performed in **Python** using libraries such as `pandas`, `numpy`, and `matplotlib` for cleaning and exploration.

### 🔧 Steps:
1. **Data Loading** – Imported dataset using `pandas.read_csv()`  
2. **Exploratory Analysis** – Used `.info()` and `.describe()` for data overview  
3. **Handling Missing Values** – Imputed missing ratings with median per product category  
4. **Feature Engineering**
   - Created `age_group` by binning age values  
   - Derived `purchase_frequency_days` from transaction timestamps  
5. **Column Standardization** – Converted column names to `snake_case` for consistency  
6. **Redundancy Check** – Dropped `promo_code_used` due to overlap with `discount_applied`  
7. **Database Integration** – Loaded the cleaned data into **SQL Server (SSMS)** for advanced analysis  

---

## 🧠 SQL Analysis (Using SSMS)
All structured analysis and insights were generated using **Microsoft SQL Server Management Studio (SSMS)**.

### Key Analytical Queries:
| # | Analysis | Description |
|---|-----------|-------------|
| 1 | **Revenue by Gender** | Compared total revenue from male vs. female customers |
| 2 | **High-Spending Discount Users** | Identified customers who used discounts yet spent above the average |
| 3 | **Top 5 Products by Rating** | Extracted products with highest average review ratings |
| 4 | **Shipping Type Comparison** | Compared purchase behavior between Standard and Express shipping |
| 5 | **Subscribers vs. Non-Subscribers** | Analyzed spending patterns based on subscription status |
| 6 | **Discount-Dependent Products** | Found products most reliant on discounts |
| 7 | **Customer Segmentation** | Classified users into New, Returning, and Loyal categories |
| 8 | **Top 3 Products per Category** | Identified best-sellers within each product category |
| 9 | **Repeat Buyers & Subscriptions** | Analyzed link between repeat purchases and subscriptions |
| 10 | **Revenue by Age Group** | Calculated revenue contribution from each age group |

---

## 📈 Power BI Dashboard
A fully interactive **Power BI Dashboard** was designed to visualize the SQL insights.

### 🔹 Dashboard Features:
- Revenue by **Gender** and **Subscription**
- **Top Products** by Rating and Purchase Count
- Customer **Segmentation Overview**
- **Discount vs. Average Spend** analysis
- **Shipping Type** performance comparison
- Interactive filters for **Category, Age Group, and Season**

> The dashboard enhances storytelling through visuals, providing a clear picture of customer trends and actionable insights.

---

## 💡 Key Business Insights
1. **Encourage Subscriptions** – Offer special benefits to attract new subscribers.  
2. **Reward Loyalty** – Implement a points-based system for repeat customers.  
3. **Optimize Discounts** – Control discount-heavy categories to improve profit margins.  
4. **Highlight Bestsellers** – Promote top-rated and frequently purchased products.  
5. **Target Marketing Campaigns** – Focus on high-spending demographics and express shipping users.

---

## 🛠️ Tech Stack
| Category | Tools & Technologies |
|-----------|----------------------|
| Programming | Python (Pandas, NumPy, Matplotlib) |
| Database | SQL Server (SSMS) |
| Visualization | Power BI |
| Environment | Jupyter Notebook |
| File Formats | CSV, PBIX, SQL |

---

## 📬 Results & Achievements
✅ Cleaned and analyzed 3,900 transactions across 18 features  
✅ Derived 10+ key business insights from SQL-based exploration  
✅ Built a dynamic Power BI dashboard for management reporting  
✅ Provided data-backed recommendations to improve customer engagement

---

## 👩‍💻 Author
**Kanika Choudhary**  
🎓 B.Tech CSE | JECRC University  
📍 Jaipur, India  
💼 Role: Data Analyst & Power BI Developer  
