# **E-commerce Sales Analysis Dashboard**

A comprehensive **Power BI dashboard** built to analyze **e-commerce sales performance**, **customer behavior**, and **product trends** using a CSV dataset.

---

## **📘 Project Overview**

This project focuses on analyzing e-commerce sales data to transform **raw transactional data** into **actionable business insights**.  
The core component is a **Power BI report** (`ec_Data Modeling.pbix`) that connects to a CSV dataset (`ec_data.csv`) and visualizes **key performance indicators (KPIs)** and trends.

The dashboard empowers **business stakeholders**—such as sales managers, marketing teams, and executives—to make **data-driven decisions** through a clear view of:

- Overall **sales performance**  
- **Product** and **category popularity**  
- **Geographical sales distribution**  
- **Payment method** utilization and status  

---

## **📊 Dataset**

**File:** `ec_data.csv`  
**Description:** A transactional dataset containing detailed order information.

**Key Columns:**
- Order ID  
- Date  
- Customer ID  
- Product Name  
- Category  
- Quantity  
- Total Sale Amount  
- Payment Method  
- Payment Status  
- Country  
- Continent  

---

## **🧰 Tools & Technologies Used**

### **Microsoft Power BI Desktop**
**Use:** Primary tool for the entire project.  

**Functions:**
- **Data Ingestion:** Connecting and importing the `ec_data.csv` file.  
- **Data Modeling:** Creating relationships, hierarchies, and a robust data model.  
- **Data Visualization:** Designing interactive reports, charts, tables, and maps.  
- **DAX (Data Analysis Expressions):** Writing formulas to calculate metrics such as:
  - Total Sales  
  - Total Orders  
  - Average Order Value  
  - Year-over-Year Sales  
  - Total Pending Orders  

---

### **Power Query (M Language)**
**Use:** Integrated within Power BI for **ETL (Extract, Transform, Load)** operations.  

**Functions:**  
- Cleaning and transforming raw CSV data.  
- Changing data types, handling nulls, and splitting or merging columns before loading to the model.

---

### **DAX (Data Analysis Expressions)**
**Use:** Formula language inside Power BI for building measures and calculations.  

**Functions:**  
Used to define business logic for:
- **Total Sales**
- **Total Orders**
- **Average Order Value**
- **Time Intelligence** (e.g., `SAMEPERIODLASTYEAR`, `DATESYTD`)

---

## **📂 Project Structure**

```
/ec_data.csv                # Raw e-commerce sales dataset
/ec_Data Modeling.pbix      # Power BI project file with model, DAX, and visuals
```

---

## **⚙️ How to Use This Project**

### **1. Prerequisites**
Install **Microsoft Power BI Desktop** (free application for Windows).

### **2. Clone the Repository**
```bash
git clone [your-repository-url]
```

### **3. Open the Report**
Navigate to the project folder and open the `ec_Data Modeling.pbix` file.

### **4. Update the Data Source (If Necessary)**
If you encounter a missing file error:
1. Go to **Home → Transform data → Data source settings**  
2. Select the `ec_data.csv` source (it will show an error icon)  
3. Click **Change Source...**  
4. Browse and select the local `ec_data.csv` file  
5. Click **OK → Close → Refresh**

---

## **📈 Potential Dashboard Features**

The Power BI report likely includes:

- **KPI Cards:** Total Sales, Total Orders, Average Order Value  
- **Geographical Map:** Sales by Country or Continent  
- **Bar Charts:** Top 10 Products by Sales, Sales by Category  
- **Pie / Donut Charts:** Orders by Payment Status (Completed, Pending, Failed), Sales by Payment Method  
- **Line Chart:** Sales Trend over Time  
- **Slicers:** Filters for Year, Continent, Category, and Payment Status  

---

## **📎 Summary**

This project demonstrates end-to-end data analytics using **Power BI**, from **data ingestion and cleaning** to **modeling and visualization**, helping businesses uncover valuable insights from e-commerce transactions.
