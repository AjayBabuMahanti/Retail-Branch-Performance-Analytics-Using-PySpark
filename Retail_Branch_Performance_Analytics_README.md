# **Retail Branch Performance Analytics at Scale Using PySpark**

## **📌 Project Overview**
Retail businesses with multiple branches across regions generate massive volumes of sales transactions every day. These transactions hold valuable insights into:
- Branch performance
- Product-level demand
- Sales team efficiency
- Regional revenue trends
- And much more.

However, traditional Excel or SQL-based approaches struggle to scale with growing data. There’s a strong need for a scalable, fast, and automated analytics pipeline that can deliver business KPIs across thousands of daily records.
----

## **🛠 Problem Statement**
The challenge is to process and analyze large-scale retail data efficiently while generating actionable KPIs. Without a scalable analytics solution, decision-making for sales planning, staffing, inventory forecasting, and revenue growth tracking becomes slow and less effective.
----

## **🎯 Objective**
To design and implement an end-to-end retail analytics solution using **PySpark** that:
- Handles large datasets efficiently
- Extracts and transforms transactional sales data
- Computes actionable KPIs at branch, region, product, and time levels
- Outputs analysis-ready summaries and dashboards

The final solution should assist decision-makers in sales planning, staffing, inventory forecasting, and revenue growth tracking.
----

## **🧰 Tools & Technologies Used**
| **Category**      | **Tools / Frameworks** |
|-------------------|------------------------|
| Big Data Engine   | Apache Spark (PySpark) |
| Notebook Env      | Google Colab / Jupyter |
| Data Viz          | Pandas, Matplotlib, Seaborn |
| Output Export     | CSVs for Power BI / Tableau |
| Language          | Python |
----

## **📊 Dataset Description**
A synthetic yet realistic dataset simulating transactional retail data.

**Columns:**
- `Branch_ID`: Store location code
- `Date`: Transaction date
- `Product_Code`: Internal SKU (product ID)
- `Units_Sold`: Quantity sold
- `Revenue`: Transaction revenue in ₹
- `Region`: North, South, East, West
- `Sales_Rep`: Salesperson handling the transaction

**Size:** 100,000+ records (scalable for PySpark)
----

## **📌 Key Performance Indicators (KPIs)**

**Intermediate KPIs:**
- Total Revenue per Region
- Revenue per Branch
- Monthly Revenue Trends
- Average Revenue per Transaction
- Units Sold per Product
- Revenue per Sales Rep
- Daily Transaction Volume

**Advanced KPIs:**
- Top 5 Branches (by revenue using window functions)
- Peak Sales Day per Region
- Average Basket Size
- Regional Revenue Share %
- Monthly Growth Rate
- Revenue Variance across Regions
----

## **⚙ Approach & Pipeline**
1. **ETL with PySpark:**
   - Read and parse raw CSV data
   - Clean missing/null fields
   - Convert data types and format dates

2. **Feature Engineering:**
   - Extract year/month for time-based KPIs
   - Calculate basket size, growth rates, etc.

3. **KPI Computation:**
   - Used Spark SQL and DataFrame APIs
   - Grouped, filtered, ranked (Window functions)
   - Aggregated at different levels (region, branch, product)

4. **Visualization & Export:**
   - Converted PySpark results to Pandas
   - Generated clean plots (monthly revenue, top branches, etc.)
   - Saved summary CSVs for BI tools like Tableau or Power BI
----

## **📊 Sample Visuals Created**
- Line Chart: Monthly Revenue Trend
- Bar Chart: Top 10 Branches by Revenue
- Pie Chart: Revenue Share by Region
- Horizontal Bar Chart: Top Sales Reps
- Boxplot: Distribution of Units Sold
----

## **📦 Deliverables**
- `retail_branch_data.csv` (dataset)
- `retail_analytics_kpi_pyspark.ipynb` (core notebook)
- Visual plots (as images)
- CSV summaries for dashboards
- PDF problem statement & README
----

## **📈 Impact / Result**
This project reflects a real-world, internship-grade analytics scenario, demonstrating the ability to:
- Handle big data using distributed computing
- Build complex KPIs using PySpark
- Prepare executive-level insights
- Contribute to scalable business analytics systems
