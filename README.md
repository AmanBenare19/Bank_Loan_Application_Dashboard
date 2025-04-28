# Bank Loan Application Dashboard

## 📚 Project Overview

This project analyzes a synthetic bank loan application dataset using SQL Server for data extraction and aggregation, and Power BI for developing an interactive business intelligence dashboard.  
The goal was to track key financial KPIs, monitor loan performance, and generate actionable insights for business decision-making in loan management and risk analysis.

---

## 🗄️ Dataset Description

The project uses a synthetic dataset (`financial_loan.csv`) representing customer loan applications, including details such as loan amount, funded amount, customer demographics, loan purpose, interest rates, DTI (Debt-to-Income) ratios, and loan statuses (Fully Paid, Current, Charged Off).

All data is fictional and used solely for educational and professional demonstration purposes.

---

## 🛠️ Tools and Technologies Used

- **SQL Server**: Data extraction, aggregation, and KPI calculations
- **Power BI**: Dashboard creation, interactive reporting, visualization
- **Microsoft Excel**: Data validation and cross-verification
- **GitHub**: Version control and project documentation

---

## 📊 Power BI Dashboard Overview

The final report is structured into three main dashboards:

---

### 🔵 1. Summary Dashboard

- Displays core KPIs:
  - **Total Loan Applications**
  - **Total Funded Amount**
  - **Total Amount Received**
  - **Average Interest Rate**
  - **Average DTI (Debt-to-Income)**
- Good Loan vs Bad Loan breakdown (donut chart with % visualization).
- Loan Status Summary:
  - Loan counts, funded amounts, received amounts categorized by status (Current, Charged Off, Fully Paid).
- MTD (Month-to-Date) and MoM (Month-over-Month) comparisons for trend analysis.

![Summary Dashboard](images/summary_dashboard.png)

---

### 🔵 2. Overview Dashboard

- Trend of **Total Loan Applications by Month** (line chart).
- State-wise loan application distribution (USA map).
- Loan breakdowns by:
  - **Loan Term** (36 vs 60 months)
  - **Employee Length** (experience group)
  - **Loan Purpose** (Credit Card, Debt Consolidation, Home Improvement, etc.)
  - **Home Ownership Status** (Rent, Mortgage, Own)
- Dynamic filters and slicers for real-time data exploration.

![Overview Dashboard](images/overview_dashboard.png)

---

### 🔵 3. Details Dashboard

- Tabular display of individual loan records:
  - Loan ID, Purpose, Home Ownership, Grade, Sub-Grade, Issue Date, Funded Amount, Interest Rate, Installment, Amount Received.
- Top panel KPIs for:
  - Total Loan Applications
  - Total Funded Amount
  - Total Amount Received
  - Average Interest Rate
  - Average DTI
- Slicers for filtering by State, Grade, and Good vs Bad Loan.

![Details Dashboard](images/details_dashboard.png)

---

## 🗄️ SQL Data Preparation and KPIs

The raw dataset was pre-processed using SQL Server to generate KPIs, using queries such as:

- `COUNT(id)` for total applications
- `SUM(loan_amount)`, `SUM(total_payment)` for funding and payments
- `AVG(int_rate)`, `AVG(dti)` for interest rate and DTI averages
- Loan performance segmentation (Good Loan = Fully Paid or Current, Bad Loan = Charged Off)
- MTD and PMTD analysis using issue dates

Aggregated data was imported into Power BI for further modeling and visualization.

---

## 📈 Key Metrics and Business Insights Delivered

- Good Loan vs Bad Loan analysis for credit risk monitoring.
- Funding and payment trends by month, state, term, purpose, and home ownership.
- Identification of high-risk categories and regional patterns.
- Performance comparison across different loan types and borrower demographics.
- Real-time slicing and dicing capabilities for business users.

---

## 📂 How to Navigate the Repository

- `AmanBenare_FinalProject.pbix`: Power BI dashboard file (all three dashboards inside).
- `Loan_Application_SQL_Queries.docx`: SQL queries for KPI generation and data extraction.
- `financial_loan.csv`: Raw dataset containing original bank loan applications.
- `/images`: Dashboard screenshots (Summary, Overview, Details).

---

## 📚 Key Learnings

- Practical experience in real-world KPI tracking using SQL Server.
- Advanced Power BI dashboard development with multi-level filtering and dynamic storytelling.
- End-to-end business intelligence workflow: from raw data → SQL aggregation → visual insights.
- Skills in communicating financial trends and customer behavior through BI reports.

---

## 🚀 Thank You for Exploring!

Feel free to view the dashboards, SQL queries, and raw data to understand the complete analytics lifecycle.  
Connect with me on [LinkedIn](https://www.linkedin.com/in/aman-benare-7801701bb/).

