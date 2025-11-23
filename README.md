# 🛒 Banggood Product Scraping & Data Engineering Pipeline

## 📌 Project Overview
This project is part of the **Data Engineering Hackathon – Batch 3**, where I built a complete data engineering workflow from **web scraping → cleaning → EDA → SQL ingestion → insights → reporting**.

The dataset used in this project:  
`banggood_products_with_category_clean.csv`

---

## 🚀 Workflow Architecture

```
Web Scraping → Data Cleaning → Feature Engineering → 
Exploratory Data Analysis → SQL Server Storage → Insights → Report
```

---

## 🧩 Features Implemented

### 🔍 1. Web Scraping
- Scraped multiple Banggood categories using `Requests` + `BeautifulSoup`.
- Extracted product attributes:
  - Title  
  - Price  
  - Rating  
  - Review Count  
  - Image  
  - Link  
  - Category  
  - Availability  

---

### 🧼 2. Data Cleaning & Standardization
- Removed null/duplicate records  
- Unified price format  
- Removed currency symbols  
- Standardized missing values  
- Lowercased inconsistent product titles  

---

### 🛠️ 3. Feature Engineering
Added new useful features:

- `price_range` → *Low, Medium, High*
- `availability_flag` → *In Stock / Out of Stock*
- Extracted clean category names
- Clean review & rating columns

---

### 📊 4. Exploratory Data Analysis (EDA)
Performed at least **5 analyses**:
- Price distribution by category  
- Rating vs price correlation  
- Most-reviewed products  
- Best value score (rating ÷ price)  
- Availability analysis  
- Top product categories  

Visualizations created using **Matplotlib**.

---

### 🗄️ 5. SQL Server Data Loading
- Created database schema  
- Inserted cleaned dataset using `pyodbc`  
- Verified row counts  
- Performed SQL Aggregations such as:
  - Average price per category  
  - Rating distribution  
  - Count of available products  
  - Most expensive & cheapest items  

---

## 📁 Project Structure

```
├── scraping_code.py
├── cleaning_code.py
├── eda_analysis.ipynb
├── sql_insertion_script.py
├── final_report.pdf
└── banggood_products_with_category_clean.csv
```

---

## 📈 Key Insights
- Electronics category had the **highest avg price**.
- Sports/Outdoors had the **best price-to-rating ratio**.
- Most products fell into the **Low–Medium price range**.
- Nearly 20–30% of products were **out of stock**.
- Higher review count products generally had **better ratings**.

---

## 🧠 Learnings
- Full data engineering pipeline design  
- Handling messy scraped data  
- Building automated ETL-like workflows  
- SQL schema design  
- Turning raw scrape into insights  

---

## 🛠️ Tech Stack
- **Python** – Pandas, BeautifulSoup, Matplotlib  
- **SQL Server**  
- **pyodbc**  
- **GitHub**  

---

## 📬 Contact
If you want to collaborate or discuss data engineering, feel free to connect!

