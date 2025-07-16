# 📊 Global NPS Breakdown by Question & Answer

This notebook performs advanced **data manipulation and NPS analysis**, computing **Promoters, Passives, and Detractors** for **each answer** to **survey question**, segmented by **company** — and in one case, by **user group**.

It aggregates and **weights results**, providing per-answer insights and a **global NPS summary** across the dataset.

---

## 🎯 Objective

To calculate and present:
- **NPS scores per answer**
- Weighted contributions from multiple companies (and optionally user groups)
- A **global view** of satisfaction trends across the dataset

---

## ✅ Main Features

### 🔍 1. Per-Answer Breakdown
- For **question**, it counts how many **Promoters (9–10)**, **Passives (7–8)**, and **Detractors (0–6)** selected each **specific answer option**
- This is done **per company**, with optional segmentation by **user group**

### ⚖️ 2. Weighted Aggregation
- Adds **weights** to each company's contribution, based on sample size or predefined logic
- Produces **fair global estimates** that reflect relative response volumes

### 🌐 3. Global Data Aggregation
- Combines results into a single view showing:
  - Total counts of Promoters, Passives, and Detractors by answer
  - **Global NPS per answer**
  - **Overall NPS across the entire dataset**

---

## 📊 Output Summary

- Tables showing:
  - Per-question, per-answer distribution of NPS types
  - Global NPS scores by answer
  - Overall NPS across all companies

---

## 🧠 Methodology

1. **Input**: Cleaned survey data (Excel or CSV)
2. **Segmentation**: Split by company (and user group if defined)
3. **Classification**: For each respondent, classify NPS type based on 0–10 rating
4. **Counting**: For every answer in every question, count NPS segments
5. **Weighting**: Multiply each company’s contribution by its sample size or predefined weight
6. **Aggregation**: Sum across companies to get global totals
7. **NPS Calculation**:
