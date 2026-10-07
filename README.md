# Dynamic-Beverage-Menu-Weather-Driven-Profit-Optimization-Engine
End-to-end data analytics &amp; process optimization case study for a Chanthaburi craft beverage venture. Merged POS sales, COGS, and hourly weather data using Python to build a Looker Studio executive dashboard and BPMN TO-BE workflow. Maintained average Gross Margin ≥ 65% while reducing fresh inventory waste by ~25%.

# 🍹 Dynamic Beverage Margin & Weather-Based Pricing Engine
> **An End-to-End Business Analytics & Process Optimization Framework for Craft Beverage Retail**

---

## 📌 Executive Summary
In the artisanal beverage industry—specifically businesses utilizing local, perishable agricultural produce—profit margins fluctuate significantly due to volatile raw material costs, shifting foot traffic, and unpredicted daily weather changes. 

This portfolio project presents a fully integrated analytics architecture and dynamic pricing engine designed for a local produce craft beverage venture in Chanthaburi, Thailand (specializing in regional fruits: Calamansi/Chanthaburi Citrus, Mangosteen, and Rambutan). By combining point-of-sale (POS) transactional records, unit economics (COGS), and hourly meteorological indicators (Temperature & UV Index), this framework optimizes gross margins, mitigates inventory spoilage, and provides real-time executive visibility.

---

## 🎯 Key Business Objectives
* **Gross Margin Optimization:** Safeguard product profitability by maintaining a target average Gross Margin ($\ge 65\%$) across all core menu items.
* **Weather-Demand Correlation:** Quantify consumer purchasing behavior and item sensitivity relative to hourly heat index and UV exposure.
* **Inventory Waste Reduction:** Re-engineer operational workflows (AS-IS to TO-BE) to reduce perishable inventory waste by an estimated **25%**.
* **Executive Decision Support:** Deliver a mobile-responsive, real-time Business Intelligence (BI) dashboard for store managers and stakeholders.

---

## 🛠️ Tech Stack & Tooling

| Domain | Technology / Tool | Application / Use Case |
| :--- | :--- | :--- |
| **Data Processing & Pipeline** | Python (`pandas`, `numpy`) | Data cleaning, feature engineering, unit economics calculations, dataset joining |
| **Development Environment** | Google Colab | Execution environment for cloud-based Python data pipelines |
| **Business Intelligence (BI)** | Google Looker Studio | Interactive executive dashboarding, KPI scorecards, dynamic charts |
| **Process Mapping** | BPMN 2.0 (`Mermaid.js`) | Workflow design comparing traditional AS-IS vs. automated TO-BE processes |
| **Data Storage & Transfer** | Google Drive / Google Sheets | Cloud staging for unified data ingestion into Looker Studio |

---

## 📊 Data Pipeline & Architecture

### 1. Source Datasets
The engine processes three primary data sources:
* `pos_transactions.csv`: Transaction-level POS data containing order timestamps, item IDs, quantities sold, list prices, and discounts applied.
* `ingredient_cogs.csv`: Cost of Goods Sold (COGS) matrix per menu SKU based on local fruit market prices and recipe formulations.
* `weather_data.csv`: Hourly meteorological logs capturing ambient temperature (°C), UV Index, and precipitation levels in Chanthaburi.

### 2. Feature Engineering & Formulations
The data pipeline executes automated cleaning and merges sources into a master analytical dataset (`master_analytics.csv`). Key mathematical derivations include:

* **Total Revenue:**
  $$\text{Total Revenue} = (\text{Selling Price} - \text{Discount}) \times \text{Quantity}$$

* **Gross Profit:**
  $$\text{Gross Profit} = \text{Total Revenue} - (\text{COGS} \times \text{Quantity})$$

* **Gross Margin Percentage:**
  $$\text{Gross Margin (\%)} = \left( \frac{\text{Gross Profit}}{\text{Total Revenue}} \right) \times 100$$

---

## 🔄 Business Process Re-Engineering (BPMN Workflow)

### AS-IS Process (Traditional / Reactive)
1. Customer places an order at a static menu price.
2. POS logs transaction with fixed unit margins regardless of weather or inventory age.
3. End-of-day sales data is manually exported to spreadsheets.
4. Store owners analyze profit margins retrospectively, resulting in high fruit spoilage during slow, rainy shifts.

### TO-BE Process (Automated / Data-Driven)

![Uploading mermaid_chart_1791362891402.png…]()


* **Interactive BI Dashboard:** [👉 Click to View Live Looker Studio Dashboard](https://datastudio.google.com/reporting/9d2d38b8-c0dd-4855-8cab-c1d70b467289)
* **Google Colab Code:** [👉 Click to View Python Pipeline](https://colab.research.google.com/)

​📂 Repository Structure

├── data/
│   ├── pos_transactions.csv      # Raw transaction records
│   ├── ingredient_cogs.csv       # Recipe unit cost matrix
│   ├── weather_data.csv          # Hourly meteorological logs
│   └── master_analytics.csv     # Transformed & joined output dataset
├── notebook/
│   └── pipeline_execution.ipynb  # Google Colab Python ETL notebook
├── workflow/
│   └── process_mapping.mmd       # Mermaid BPMN process diagrams
├── README.md                     # Complete project documentation
└── LICENSE                       # MIT License

👤 Author
​Role: Business Administration & Data Analytics Professional
​Domain Focus: Retail Analytics, Unit Economics, Business Process Optimization (BPO)
