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
### 🔹 Customer Insights
- **Number of Transactions by Gender:** Helps understand purchasing behavior
- **Loyalty Analysis:** Identifying customers purchasing from multiple stores
- **State-wise Customer Distribution:** Determines demand by geography
- **Transactions by Men & Women:** Analyzes gender-based shopping patterns

### 🔹 Sales Revenew & Performance Analysis
- **City with the Highest Number of Orders:** Helps optimize store expansion
- **Area with the Highest Sales:** Determines high-revenue locations
- **Top-selling Products & Categories:** Guides inventory planning
- **Customer segmentation:** Segments customers into loyalty tiers based on purchase frequency

## 📊 Business Impact & Benefits
- **✅Improved Inventory Management:** Stores can optimize stock levels based on demand patterns.
- **✅Personalized Marketing:** Gender-based and location-based insights help in targeted promotions.
- **✅Operational Efficiency:** Identifying high-performing stores and streamlining underperforming ones.
- **✅Revenue Growth:** Data-driven decision-making leads to better pricing and sales strategies.
- **✅Better Customer Retention:** Loyalty segmentation helps tailor reward programs for high-value customers.


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


