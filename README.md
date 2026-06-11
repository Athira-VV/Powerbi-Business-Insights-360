# Powerbi-Business-Insights-360

End-to-end Power BI business analytics project covering Finance, Sales, Marketing, Supply Chain, and Executive insights.

# Business Insights 360 - Power BI Project

## Project Overview

Business Insights 360 is a guided Power BI project that I completed as part of my Power BI learning journey. The project focuses on transforming business data into meaningful insights to support data-driven decision-making across different departments such as Finance, Sales, Marketing, Supply Chain, and Executive Management.

The goal of this project is to analyze business performance, identify trends, monitor KPIs, and provide actionable insights through an interactive Power BI dashboard.

## Project Objectives

* Analyze overall business performance using interactive dashboards.
* Track key financial and sales metrics.
* Monitor marketing effectiveness and customer performance.
* Evaluate supply chain forecasting accuracy.
* Provide executive-level insights for strategic decision-making.
* Build a centralized reporting solution for multiple business functions.

---

## Tools & Technologies Used

* Power BI Desktop
* SQL
* Microsoft Excel
* DAX (Data Analysis Expressions)

---

## Business Concepts Covered

* Gross Price
* Net Sales
* Net Invoice Sales
* Gross Margin
* Net Profit
* Cost of Goods Sold (COGS)
* Pre-Invoice Deductions
* Post-Invoice Deductions
* Forecast Accuracy
* Year-To-Date (YTD)
* Year-To-Go (YTG)

---

## Business Background

AtliQ Hardware is a rapidly growing company that sells computers and computer accessories across multiple markets through different sales channels.

### Sales Channels

* Retailers
* Direct
* Distributors

As the company expanded into new markets, it faced challenges in making accurate business decisions using traditional reporting methods. To improve decision-making and gain better visibility into business performance, the company adopted a centralized analytics solution using Power BI.

---

## Project Planning

Before developing the dashboard, the following business questions were considered:

* What is the objective of the dashboard?
* How will success be measured?
* Who are the end users?
* What insights do stakeholders expect?
* What data is required for analysis?
* What business challenges need to be addressed?
* What KPIs should be monitored?

---

## Dataset Overview

The project uses both dimension and fact tables.

**Dimension Tables:** Contain static information such as customer, product, and market details.

**Fact Tables:** Contain transactional and forecast data used for business analysis and reporting.

### gdb041

#### dim_customer

* **27** distinct markets (e.g., India, USA, Spain)
* **75** distinct customers across all markets
* **2** platform types:

  * Brick & Mortar – Physical/Offline Stores
  * E-commerce – Online Stores (Amazon, Flipkart, etc.)
* **3** sales channels:

  * Retailer
  * Direct
  * Distributors

#### dim_market

* **27** distinct markets
* **7** sub-zones
* **4** regions:

  * APAC
  * EU
  * NA
  * LATAM

#### dim_product

##### Divisions

**P & A**

* Peripherals
* Accessories

**PC**

* Notebook
* Desktop

**N & S**

* Networking
* Storage

Additional Information:

* 14 different product categories such as Internal HDD, Keyboard, etc.
* Multiple variants available for the same product.

#### fact_forecast_monthly

This table is used to forecast customer demand in advance, helping the business to:

* Improve customer satisfaction
* Reduce warehouse storage costs
* Support demand planning activities

Additional details:

* The table is denormalized by the data engineering team for analytical purposes.
* Monthly data is stored using the first date of the month.
* Contains forecast quantity information for products and customers.

#### fact_sales_monthly

This table stores actual sales transaction data.

* Similar structure to the forecast table.
* Contains sold quantity instead of forecast quantity.
* Used for sales analysis and forecast accuracy calculations.

---

### gdb056

#### freight_cost

* Contains freight and other logistics-related costs.
* Available by market and fiscal year.

#### gross_price

* Contains gross selling price information for each product.

#### manufacturing_cost

* Contains manufacturing cost details for products by fiscal year.

#### pre_invoice_deductions

* Contains pre-invoice deduction percentages for customers by fiscal year.

#### post_invoice_deductions

* Contains post-invoice deductions and other related deduction details.

---

## Importing Data into Power BI

The project data was stored in a MySQL database and imported into Power BI using database connection credentials.

---

## Data Model

Data modeling plays a vital role and serves as the foundation of the report. All visuals and calculations are built on top of the data model.

Poor data modeling can negatively impact report performance and usability.

In this project, a Snowflake data modeling approach was used.

### Data Model Diagram

*(Add Data Model Screenshot Here)*

---

## Dashboard Designing

Based on the business requirements and dashboard mockups, visuals and measures were created to support stakeholder needs and business analysis.

### Home View

The Home View acts as the landing page and provides navigation to all report sections.

* Info
* Finance View
* Sales View
* Marketing View
* Supply Chain View
* Executive View

---

## Info Page

*(Add Screenshot Here)*

---

## Finance View

*(Add Screenshot Here)*

---

## Sales View

*(Add Screenshot Here)*

---

## Marketing View

*(Add Screenshot Here)*

---

## Supply Chain View

*(Add Screenshot Here)*

---

## Executive View

*(Add Screenshot Here)*

---

## Report File

You can find the complete Power BI report file here:

[Report](Add_Report_Link_Here)

---

## Project Outcome

This dashboard helps stakeholders make data-driven decisions by providing a centralized view of business performance across different functions.

The report enables users to monitor KPIs, identify trends, analyze performance, and answer important business questions using data.
