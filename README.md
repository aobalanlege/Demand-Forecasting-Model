# Demand-Forecasting-Model

![Shopping trolley in front of a laptop](./iStock-1249219777.jpg)

It's simple to buy any product with a click and have it delivered to your door. Online shopping has been rapidly evolving over the last few years, making our lives easier. But behind the scenes, e-commerce companies face a complex challenge that needs to be addressed. 

Uncertainty plays a big role in how the supply chains plan and organize their operations to ensure that the products are delivered on time. These uncertainties can lead to challenges such as stockouts, delayed deliveries, and increased operational costs.

You work for the Sales & Operations Planning (S&OP) team at a multinational e-commerce company. They need your help to assist in planning for the upcoming end-of-the-year sales. They want to use your insights to plan for promotional opportunities and manage their inventory. This effort is to ensure they have the right products in stock when needed and ensure their customers are satisfied with the prompt delivery to their doorstep.


## The Data

You are provided with a sales dataset to use. A summary and preview are provided below.

# Online Retail.csv

| Column     | Description              |
|------------|--------------------------|
| `'InvoiceNo'` | A 6-digit number uniquely assigned to each transaction |
| `'StockCode'` | A 5-digit number uniquely assigned to each distinct product |
| `'Description'` | The product name |
| `'Quantity'` | The quantity of each product (item) per transaction |
| `'UnitPrice'` | Product price per unit |
| `'CustomerID'` | A 5-digit number uniquely assigned to each customer |
| `'Country'` | The name of the country where each customer resides |
| `'InvoiceDate'` | The day and time when each transaction was generated `"MM/DD/YYYY"` |
| `'Year'` | The year when each transaction was generated |
| `'Month'` | The month when each transaction was generated |
| `'Week'` | The week when each transaction was generated (`1`-`52`) |
| `'Day'` | The day of the month when each transaction was generated (`1`-`31`) |
| `'DayOfWeek'` | The day of the weeke when each transaction was generated <br>(`0` = Monday, `6` = Sunday) |

### Step 1: Understand the Problem and Define Objectives

**Objective**:  
Predict the quantity of products sold (demand) for future periods to support inventory and sales planning.

**Target Variable**:  
- Quantity (units sold per transaction).

**Features**:  
- **Time-based features**: Year, Month, Week, Day, DayOfWeek, InvoiceDate  
- **Product information**: StockCode, Description, UnitPrice  
- **Customer information**: CustomerID, Country  
