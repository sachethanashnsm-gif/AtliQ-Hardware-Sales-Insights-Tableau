# AtliQ Hardware Sales Insights - Tableau Data Analysis

## 📌 Project Overview
AtliQ is a rapidly growing computer hardware and peripheral manufacturer with a head office in Delhi, India, and multiple regional offices across different states. They supply hardware to major clients including Surge Stores, Nomad Stores, Excel Stores, and Electrical Stores. 

Recently, the company has been experiencing a decline in sales. The Sales Director struggled to get a clear, actionable picture of the business due to the sheer volume of fragmented Excel files provided by regional managers. To solve this problem and enable data-driven decision-making, this project consolidates the data and transforms it into an interactive **Tableau Dashboard**.

## 🎯 Objective
To build a centralized visual dashboard that provides the Sales Director with immediate, simple, and clear insights into the company's sales performance across various regions, products, and clients, ultimately replacing cumbersome spreadsheet reporting.

## 📊 Dashboard Features & Key Metrics
The Tableau dashboard provides a comprehensive view of the company's performance, featuring:
* **Overall Business Health**: Tracking Total Revenue and Total Sales Quantity[cite: 3].
* **Time-Series Analysis**: Revenue breakdown by years (2017–2020) and individual months to identify seasonal trends[cite: 3].
* **Geographical Performance**: Revenue breakdown by major markets/cities across India[cite: 3].
* **Client Analysis**: Identification of the Top 5 customers by revenue[cite: 3].
* **Product Analysis**: Identification of the Top 5 best-selling products by revenue[cite: 3].

## 💡 Key Insights Uncovered
Based on the dashboard data, the following high-level insights were extracted:
* **Overall Metrics**: The company generated a Total Revenue of **986.64M** and a Total Sales Quantity of **2.43M** over the tracked period[cite: 3].
* **Top Markets**: **Delhi NCR** is the dominant market generating 520.79M in revenue, followed by **Mumbai** (150.18M) and **Ahmedabad** (132.53M)[cite: 3].
* **Top 5 Customers**[cite: 3]: 
  1. Electricalsara Stores (413.91M)
  2. Electricalslytical (49.64M)
  3. Excel Stores (49.18M)
  4. Premium Stores (45.33M)
  5. Nixon (43.92M)
* **Top 5 Products**[cite: 3]: 
  1. Prod040 (23.58M)
  2. Prod159 (17.66M)
  3. Prod065 (16.26M)
  4. Prod018 (15.60M)
  5. Prod053 (15.14M)

## 🛠️ Tools & Technologies Used
* **Data Visualization**: Tableau[cite: 3, 4]
* **Database / Data Source**: MySQL (Sales Database containing tables for Transactions, Customers, Date, Markets, and Products)[cite: 4]
* **Data Modeling**: Star schema setup connecting transaction facts with dimension tables[cite: 4].

## 📂 Data Structure
The analysis is built on a relational data model with the following core tables[cite: 4]:
* `transactions`: Contains sales quantities, amounts, order dates, and currency details. 
* `customers`: Contains customer codes, names, and types.
* `markets`: Contains regional data, market codes, and zones.
* `products`: Contains product codes and types.
* `date`: Contains calendar details (year, month, cy_date) for time intelligence. 

*(Note: Data cleaning processes included currency normalization, converting USD transactions into INR to maintain consistent revenue tracking[cite: 4]).*
