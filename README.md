# Retail_Analytics
End-to-end retail sales analytics pipeline for a multi-state bicycle chain across NY, CA &amp; TX. Features data cleaning in Excel, relational modeling in MySQL, Python EDA &amp; RFM customer segmentation, and a 4-page Power BI dashboard tracking ₹8.58M revenue, 1.6K orders, store maps, and inventory stock alerts.
# 🛒 Retail Sales Analytics — End-to-End Data Pipeline

[![Excel](https://img.shields.io/badge/Excel-217346?style=for-the-badge&logo=microsoft-excel&logoColor=white)](#)
[![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white)](#)
[![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)](#)
[![Power BI](https://img.shields.io/badge/Power_BI-F2C811?style=for-the-badge&logo=power-bi&logoColor=black)](#)

An end-to-end retail analytics solution processing raw transactional data from a multi-store bicycle chain across NY, CA, and TX into executive decision support tools.

---

## 📌 Executive Summary & Key KPIs

* **Total Revenue:** ~$8.58M
* **Total Orders:** 1,615 orders[cite: 4]
* **Active Customers:** 1,445 customers[cite: 4]
* **Average Order Value (AOV):** ~$5.31K[cite: 4]
* **Stores Covered:** 3 Stores (Santa Cruz, CA | Baldwin, NY | Rowlett, TX)[cite: 4]

---

## 🛠️ Multi-Tool Analytics Architecture

### Phase 1: Data Cleaning & Validation (Excel)
* Cleaned, deduplicated, and verified raw records across 9 linked dataset sheets[cite: 4].
* Standardized column types, handled missing ZIP codes/phones, and derived `total_price = (list_price × quantity) − discount`[cite: 4].
* Performed outlier detection using standard deviation thresholds (flagged high-value Trek bikes > $3,132.74)[cite: 4].

BRANDS:

<img width="1917" height="586" alt="brands_xl" src="https://github.com/user-attachments/assets/7e4b8254-9770-471d-ae7c-245b933408cf" />

CATEGORIES:

<img width="1802" height="227" alt="categories_xl" src="https://github.com/user-attachments/assets/4ec60492-93aa-4ad2-8e0d-f81e7a5c6c5d" />

CUSTOMERS:

<img width="1917" height="840" alt="customer_xl" src="https://github.com/user-attachments/assets/f66c4980-d989-48ab-aeaf-5c64903cdc9f" />

ORDER_ITEMS:

<img width="1916" height="848" alt="order_items" src="https://github.com/user-attachments/assets/04eca913-0a8d-4eb2-8dac-f5c7cec8766a" />

ORDERS:

<img width="1917" height="847" alt="orders_xl" src="https://github.com/user-attachments/assets/0632819d-a041-48cc-8347-3d15e837b143" />

PRODUCTS:

<img width="1917" height="825" alt="products_xl" src="https://github.com/user-attachments/assets/140acf3c-892d-43f0-8ece-5faa0902b1d9" />

STAFF:

<img width="1917" height="397" alt="staff_xl" src="https://github.com/user-attachments/assets/647ff9a8-11ed-43f4-b9e7-e5f52e2f6ec0" />

STOCKS:

<img width="1917" height="852" alt="stocks_xl" src="https://github.com/user-attachments/assets/bec6cd2a-0b28-41ef-9f9f-701659f4b727" />

STORES:

<img width="1917" height="180" alt="store_xl" src="https://github.com/user-attachments/assets/3dc5c3ba-ac6b-439f-b6e2-4c8d9f777dcd" />

### Phase 2: Relational Database Design (MySQL)
* Modeled an enterprise schema with foreign keys connecting customers, orders, order items, products, stores, and inventory stocks[cite: 4].
* Engineered multi-table `JOIN` aggregate queries for store and staff sales performance[cite: 4].
* Implemented inventory monitoring logic for low stock alerts (< 10 units)[cite: 4].

<img width="1917" height="1078" alt="sql" src="https://github.com/user-attachments/assets/e3faf121-6133-478c-9288-49446c1695a4" />

### Phase 3: Exploratory Analysis & ML Segmentation (Python)
* Automated database ingestion via `SQLAlchemy` and `Pandas`[cite: 4].
* Analyzed order volume distributions, store order shares (Store 2 led with 68% share), and product price boxplots[cite: 4].
* Calculated **RFM (Recency, Frequency, Monetary)** customer scores and exported segment classifications directly back to MySQL[cite: 4].

<img width="1285" height="551" alt="Screenshot 2026-10-05 190701" src="https://github.com/user-attachments/assets/0b540c2e-e3d0-4c61-8758-55bbe31bbaa8" />

<img width="1332" height="863" alt="Screenshot 2026-10-05 190752" src="https://github.com/user-attachments/assets/e6f6445b-45cc-43df-8a89-030b6174456c" />

<img width="1327" height="790" alt="Screenshot 2026-10-05 190911" src="https://github.com/user-attachments/assets/2a143189-af80-4d2b-b5af-6ec46c742be1" />

<img width="1227" height="547" alt="Screenshot 2026-10-05 190957" src="https://github.com/user-attachments/assets/0ffce4c3-6c1b-4c3d-a6bc-3eb4d2ce8cf2" />

<img width="1236" height="387" alt="Screenshot 2026-10-05 191032" src="https://github.com/user-attachments/assets/77a79864-7e3c-48d7-bedc-3e8b2136039c" />


### Phase 4: Executive Dashboard & BI (Power BI)
* Created a 2-page interactive dashboard with custom color themes, slicers, and bookmark navigators[cite: 4].
* **Page 1 (Executive Summary):** Displays core KPIs, monthly revenue trend line charts, store map location bubbles, and customer RFM segment breakdown[cite: 4].
* **Page 2 (Sales & Category Analysis):** Provides granular category revenue column charts and top 5 product bar charts[cite: 4].

<img width="1160" height="660" alt="retail_1st" src="https://github.com/user-attachments/assets/271a6910-29fd-455d-921e-069f3e2df94d" />

<img width="1153" height="657" alt="retail_2nd" src="https://github.com/user-attachments/assets/a786e1d8-853f-48ab-96c1-5ec4dfeb644c" />

<img width="1163" height="660" alt="retail_3rd" src="https://github.com/user-attachments/assets/19891801-0287-460b-8e55-ad5200ddb7f4" />

<img width="1178" height="678" alt="retail_4th" src="https://github.com/user-attachments/assets/51bf10ce-d6b2-4cd8-9d76-9cae587515fd" />

---

## 💡 Top Business Insights

1. **Category Leader:** Mountain Bikes generate the highest revenue (~$3.03M), more than double any other category[cite: 4].
2. **Store Concentration:** Store 2 (Baldwin Bikes) drives 68% of total order volume (1,093 / 1,615 orders)[cite: 4].
3. **Customer Base:** ~70% of the customer base (1,019 out of 1,445) is localized in New York[cite: 4].

---

## 📁 Repository Structure

```text
├── data/                 # Cleaned CSV files
├── excel/                # Phase 1: Excel spreadsheet & pivot tables
├── sql/                  # Phase 2: Relational schema setup & business queries
├── python/               # Phase 3: Jupyter notebook (EDA & RFM Segmentation)
├── power_bi/             # Phase 4: Power BI (.pbix) report & screenshots
└── README.md             # Project documentation
👤 Author
Presenter: PRAVEEN T
