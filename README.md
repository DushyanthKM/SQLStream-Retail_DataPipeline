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

- **Gender Distribution**:  
  - Male customers: **358 transactions**  
  - Female customers: **192 transactions**  
  ➤ Indicates a stronger male customer base.

- **Loyalty Pattern**:  
  - **101 customers** purchased from **more than one store**  
  ➤ Ideal segment for loyalty program targeting.

- **Regional Focus**:  
  - **Karnataka** had the highest customer base with **97 customers**  
  ➤ Prime focus region for customer-centric campaigns.

---

### 🏬 Store & Regional Sales

- **Top Performing Region**:  
  - **Bengaluru**: **275 orders**  
  - **Indiranagar**: Top area by sales – **₹1.12 Lakhs**  
  - Followed by **Andheri** in Mumbai.

- **Key Revenue Contributors**:
  - Jayanagar  
  - Marathahalli  
  - Koramangala

---

### 📦 Product Performance

- **Top-Selling Products (by Quantity)**:
  - Nilgiris Premium Fried Gram - Split: **89 units**
  - Chana Dal: **71 units**
  - Marie Gold Biscuits: **64 units**

- **Top Revenue-Generating Products**:
  - Avocado: **₹25,650**
  - Asparagus: **₹17,625**
  - Kolam Rice: **₹14,260**
  ➤ High ROI despite lower volume sales

- **Consumer Preferences**:
  - Personal care items like **Nivea** and **Garnier face washes** ranked high in both **volume** and **revenue**  
  ➤ Strong and consistent consumer demand

---

## 🎯 Business Impact

- 💡 **Inventory Optimization**:  
  Identified fast-moving and high-margin products to enable data-driven inventory planning.

- 📍 **Strategic Expansion**:  
  Pinpointed high-performing stores and regions to guide investment and expansion decisions.

- 🧠 **Loyalty Program Design**:  
  Cluster analysis of customer behavior supported personalized loyalty strategies.

- 📈 **Targeted Marketing**:  
  Insights into gender and region preferences enabled better-targeted marketing, improving customer engagement and conversion rates.

---

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


