Learning project. Built while learning [Power BI / SQL / Python] with AI assistance for guidance and debugging. The business questions, dataset selection, and review of results were mine. Some advanced parts were AI-guided.

# IT Service Desk — SLA Compliance & Ticket Analytics

An end-to-end Excel analytics project analyzing 97,498 IT support tickets (2016–2020) to uncover SLA compliance gaps, agent performance patterns, and process failures at a growing IT service desk.

## 📊 Project Overview

This repository contains a working Excel analysis workbook built with Microsoft Excel tools including:
- Nested `IF`
- `COUNTIFS` / `AVERAGEIFS`
- `VLOOKUP`
- Pivot Tables and Slicers
- Array formulas such as `MEDIAN(IF(...))`
- `QUARTILE` / IQR outlier detection
- `CORREL`
- Conditional formatting

## 🎯 The Problem

The company had 5 years of raw ticket logs but no visibility into:
- Whether SLA targets were actually being met
- Whether tickets were being triaged/prioritized correctly
- Whether agent workload or performance drove service quality

## 🔍 My Approach

- Data cleaning: handled messy real data, including typos in category labels and ~30% of tickets missing priority.
- Built SLA logic from scratch: no SLA target column existed, so I calculated realistic targets using each priority tier's median resolution time plus a reasonable buffer.
- Statistical validation: used IQR to detect outlier tickets and Pearson correlation to test assumptions before drawing conclusions.
- Interactive dashboard: built Pivot Tables with slicers for Year, Agent, and Priority to support live exploration.

## 📈 Key Findings

- **Triage Gap:** 29.76% of tickets never received a priority — consistent across every category and indicating a systemic intake failure.
- **Breach Rate:** 40.29% overall SLA breach rate, ranging from 1% for Login Access to 66% for Hardware.
- **No Improvement Over Time:** Ticket volume doubled from 2016 to 2020, but breach rate and triage gap remained flat.
- **Agent Performance ≠ Workload:** Correlation between ticket volume and breach rate was only 0.14, showing the true driver was consistency rather than overload.
- **Speed ≠ Satisfaction:** Correlation between resolution time and satisfaction was -0.02, suggesting faster resolution did not necessarily mean higher satisfaction.

## 🧠 What I Learned

This project pushed me beyond basic formula application into analytical thinking: testing assumptions with statistics, distinguishing correlation from causation, and translating raw numbers into business recommendations.

## 📁 Files in this Repository

- `IT ANALYSIS WORKING SHEET.xlsx` — the main working file with raw data, formulas, pivot tables, and dashboard.
- `README.md` — this project overview.

## 📝 Notes

- A `.gitignore` has been added to exclude Excel temporary files like `~$IT ANALYSIS WORKING SHEET.xlsx`.
- If you want, I can also create a `IT_Service_Desk_Findings.md` summary file or a `IT_Service_Desk_Project_Roadmap.md` file for the analytical process.

## 📌 How to Use

1. Download or clone the repository.
2. Open `IT ANALYSIS WORKING SHEET.xlsx` in Microsoft Excel.
3. Use the Pivot Table slicers and dashboard to explore SLA compliance, triage gaps, and agent performance.

## 🔗 Connect

This project is part of a data analyst portfolio. Connect on LinkedIn to discuss the analysis and business recommendations further:

- https://www.linkedin.com/in/afreenofficial
