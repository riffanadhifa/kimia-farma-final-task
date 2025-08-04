# Kimia Farma Final Task – Big Data Analyst Internship

This repository contains the SQL syntax and analysis process used to complete the Final Task project from the **Rakamin x Kimia Farma Big Data Analyst Virtual Internship**.

## 🧩 Project Overview

The goal of this project is to analyze Kimia Farma's business performance (sales, profit, and customer satisfaction) across various branches and provinces in Indonesia from **2020 to 2023** using BigQuery and Looker Studio.

## 📊 Dataset Used

- `kf_final_transaction.csv` – Transaction data  
- `kf_product.csv` – Product and pricing data  
- `kf_inventory.csv` – Inventory per branch  
- `kf_kantor_cabang.csv` – Branch info and customer rating

## ⚙️ SQL Process Summary

1. Upload 4 datasets into BigQuery  
2. Join tables using `LEFT JOIN`  
3. Create calculated fields:
   - `nett_sales = price - (price * discount_percentage / 100)`
   - `nett_profit = nett_sales * gross_profit_percentage`
   - `profit_category` using `CASE WHEN` logic based on price range
4. Save results as a new table: `analisa_kimia_farma`

## 📂 File

- `analisa_kimia_farma.sql` – Full SQL query for data cleaning, joining, and metric calculation.

## 📈 Dashboard

All results were visualized using **Google Looker Studio**.  
🔗 [Insert your Looker Studio dashboard link here]

---

🧠 Created by: Naswa Aulia  
🚀 Tools used: Google BigQuery, SQL, Looker Studio
