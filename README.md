# Task---8
# 📊 Superstore Sales Dashboard – Power BI Project

## 📝 Project Title
Simple Sales Performance Dashboard using Superstore Dataset

---

## 🎯 Objective
To create an **interactive dashboard** that visualizes sales performance by **product category**, **region**, and **month**, enabling business users to make data-driven decisions.

---

## 🛠 Tools Used
- **Power BI Desktop** – for data visualization and interactive dashboard creation  
- (Optional) **Python (Pandas)** – for preprocessing/cleaning the dataset  
- **Dataset** – Superstore_Sales.csv  
  *(Columns Used: Order Date, Sales, Region, Category, Profit)*

---

## 📁 Dataset Overview
| Column Name   | Description                      |
|---------------|----------------------------------|
| Order Date    | Date of the order placed         |
| Region        | Geographic sales region          |
| Category      | Product category (e.g., Furniture, Technology) |
| Sales         | Sales amount in USD              |
| Profit        | Profit amount in USD             |

---

## 📈 Dashboard Components

### 1. **Line Chart: Sales Over Time**
- **X-Axis**: Month-Year (from Order Date)
- **Y-Axis**: Sales
- **Purpose**: To analyze monthly sales trends

### 2. **Clustered Bar Chart: Sales by Region**
- **Axis**: Region
- **Values**: Sales
- **Purpose**: To compare sales performance across regions

### 3. **Donut Chart: Sales by Category**
- **Legend**: Category
- **Values**: Sales
- **Purpose**: To visualize category-wise sales distribution

### 4. **Slicer: Region Filter**
- Enables filtering the visuals by a specific region

---

## 🧹 Data Cleaning Steps
1. Converted `Order Date` to `Month-Year` format using DAX:
   ```DAX
   MonthYear = FORMAT('Sample - Superstore'[Order Date], "YYYY-MMM")
