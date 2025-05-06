# ETL-Driven Retail Analytics: SQL Data Pipeline

## ❓ Problem Statement
Built an **ETL pipeline** to extract, transform, and load retail store data into a structured database. Using **SQL queries** analyzed consumer behavior, sales trends, and operational performance to derive meaningful insights that help in decision-making for a retail business.

## 📊 Data Points Used
The dataset includes information on:
- **Customers:** Customer details such as ID, Name, Gender, City, State.
- **Stores:** Store ID, Location details (City, Area, State).
- **Products:** Product ID, Category, Price.
- **Orders:**  Order ID, Customer ID, Store ID, Order Date, Total Amount.
- **Order Mapping:** Links Orders to Products, including Order ID, Product ID, and Quantity.

## ⚙️ Technology Stack
- **ETL Pipeline:** Extract, transform(Using Excel), and load data 
- **SQL:** Data transformation and analysis
- **Excel:** For initial data formatting before loading into SQL
- **Database Management:** Structured storage of retail data

## 🏗️ Methodology
- Format Data: Clean and structure raw data using Excel.
- Load into SQL: Import formatted data into a SQL database.
- Data Transformation: Create relationships between tables using keys (e.g., Customers → Orders → Order Mapping → Products).
- SQL Querying & Analysis: Perform aggregations, joins, and conditional computations.

### 📈 SQL Querying & Data Analysis
#### **Key SQL Operations Used:**
- **Aggregation (`SUM`, `COUNT`, `AVG`)** for sales and revenue analysis
- **Joins (`INNER JOIN`, `LEFT JOIN`)** to connect customers, transactions, and stores
- **Conditional Columns (`CASE WHEN`)** to classify transactions
- **Filtering (`WHERE`, `HAVING`)** for targeted insights
- **Grouping & Sorting (`Group By` , `ORDER BY`)** to group & rank performance metrics

## 🔍 Key Insights Generated

# 📊 Project Outcome - Insights & Business Impact

## ✅ Customer Trends:

- **Male customers** made **358 transactions** vs. **192 by female**, indicating a stronger **male customer base**.
- **Loyalty pattern**: 101 customers purchased from more than one store, ideal for **loyalty program targeting**.
- **Karnataka** had the **highest customer base** (97 customers), making it the **prime focus** for customer-centric campaigns.

## ✅ Store & Regional Sales:

- **Bengaluru** had the **highest number of orders (275)** and **Indiranagar** emerged as the **top area by sales** with **₹1.12 Lakhs**, followed by **Andheri in Mumbai**.
- **Jayanagar**, **Marathahalli**, and **Koramangala** were also **key contributors to revenue**.

## ✅ Product Performance:

### 🔝 Top-Selling Products (by Quantity):
- **Nilgiris Premium Fried Gram - Split**: 89 units  
- **Chana Dal**: 71 units  
- **Marie Gold Biscuits**: 64 units

### 💰 Top Revenue-Generating Products:
- **Avocado**: ₹25,650  
- **Asparagus**: ₹17,625  
- **Kolam Rice**: ₹14,260  
  > These showed **high ROI** despite **lower volumes**.

- **Personal care items** like **Nivea** and **Garnier face washes** ranked in both **volume and revenue**, indicating **strong consumer preference**.

---

## 🎯 Business Impact:

- 💡 **Enabled data-driven inventory planning** by highlighting **fast-moving** and **high-margin** products.
- 🎯 **Helped identify high-performing stores and areas**, guiding **expansion and investment strategy**.
- 🧠 **Facilitated loyalty program design** using **customer clustering**.
- 📈 **Supported targeted marketing** by analyzing **gender and regional preferences**, improving **engagement** and **conversion rates**.

## 🚀 Getting Started
1. Clone this repository
2. Load the dataset into a **SQL database**
3. Run the **ETL pipeline** to clean and transform data
4. Execute SQL queries to generate insights

---

## 🤝 Contributing 
💡 Open for feedback & collaborations!  If you have any improvements, feel free to open a pull request! 🚀

## **👨‍💻 Author & 📌 Contact**
### Dushyanth KM 🔗 www.linkedin.com/in/
dushyanth-km-666660260


