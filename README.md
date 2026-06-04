# 💳 UPI Transaction Analytics Dashboard - Power BI

## 📌 Project Overview

This project is an end-to-end **UPI (Unified Payments Interface) Transaction Analytics Dashboard** built using **Microsoft Power BI**. It analyzes **20,000 real-world-style UPI transactions** to uncover patterns in payment behaviour, transaction success rates, city-wise spending, and demographic insights.

The dashboard is designed to help business analysts and fintech teams quickly visualize and explore digital payment trends across multiple dimensions.

---

## 📂 Dataset

| Property | Details |
|---|---|
| **File** | `UPI_Transactions.xlsx` |
| **Records** | 20,000 transactions |
| **Source Sheet** | UPI Transaction |
| **Time Period** | 2024 |

### 🗂️ Columns in Dataset

| Column | Description |
|---|---|
| `TransactionID` | Unique transaction identifier |
| `TransactionDate` | Date of transaction |
| `TransactionTime` | Time of transaction |
| `Amount` | Transaction amount |
| `BankNameSent` | Sender's bank (SBI, HDFC, ICICI, Axis) |
| `BankNameReceived` | Receiver's bank |
| `RemainingBalance` | Balance after transaction |
| `City` | City of transaction (Delhi, Mumbai, Bangalore, Hyderabad) |
| `Gender` | Customer gender |
| `CustomerAge` | Customer age |
| `TransactionType` | Payment / Transfer |
| `Status` | Success / Failed |
| `DeviceType` | Tablet / Laptop / Mobile |
| `PaymentMethod` | QR Code / Phone Number / etc. |
| `PaymentMode` | Instant / Scheduled |
| `MerchantName` | Merchant (Amazon, Zomato, etc.) |
| `Purpose` | Food / Travel / Shopping / Bill Payment / Others |
| `Currency` | Transaction currency |
| `CustomerAccountNumber` | Customer account (text format) |
| `MerchantAccountNumber` | Merchant account (text format) |

---

## 🛠️ Data Transformation (Power Query)

The following transformations were applied in **Power Query Editor**:

- ✅ Renamed `Sheet1` → `UPI Transaction`
- ✅ **Split `TransactionTime` column** to extract time-only values (removed date component)
- ✅ Renamed the resulting column back to `TransactionTime`
- ✅ Changed `CustomerAccountNumber` data type: **Numerical → Text**
- ✅ Changed `MerchantAccountNumber` data type: **Numerical → Text**
- ✅ Performed **Data Profiling** — Column Quality, Column Distribution, Column Profiling (based on entire dataset)
- ✅ Confirmed **zero null/missing values** in the dataset

---
## 📸 Screenshots

### Page 1 - Transaction and Balance
![Transaction and Balance](Screenshots/Transaction%20and%20Balance.png)

### Page 2 - Matrix Visuals
![Matrix Visuals](Screenshots/Matrix%20Visuals.png)

## 📈 Dashboard Features

### 🎛️ Slicers & Filters
- Multiple slicers with **Sync Slicer** enabled across pages (via View Tab)
- Slicers formatted and aligned for clean visual layout
- Canvas background customized for improved aesthetics

### 📉 Visualizations
- **Line Chart & Column Chart** with **Bookmark Toggle** - users can switch between chart types interactively
- **Conditional Formatting** on visuals - lighter color for lowest values, darker for highest
- **Age Group segmentation** for demographic analysis
- City-wise, bank-wise, purpose-wise, and status-wise breakdowns

### 🔖 Power BI Features Used
| Feature | Usage |
|---|---|
| Power Query Editor | Data transformation & profiling |
| DAX | Calculated columns |
| Bookmarks | Toggle between chart types |
| Sync Slicers | Consistent filtering across pages |
| Conditional Formatting | Color-coded value representation |
| Canvas Background | Custom report design |
| Selection Pane | Managing visual layers |

---

## 📁 Repository Structure

```
📦 upi-transaction-powerbi
 ┣ 📊 PowerBI_Project__UPI_Transaction_.pbix   ← Main Power BI Dashboard
 ┣ 📋 UPI_Transactions.xlsx                    ← Raw Dataset (20,000 rows)
 ┣ 📄 PowerBI_Project_3.docx                   ← Step-by-step project documentation
 ┗ 📖 README.md                                ← You are here
```

---

## 💡 Key Insights (from the Dashboard)

- **Transaction Types:** Payments and Transfers distributed across 4 major Indian cities
- **Top Banks:** SBI, HDFC, ICICI, Axis Bank
- **Top Purposes:** Food, Shopping, Travel, Bill Payment, Others
- **Device Trends:** Transactions tracked across Tablet, Laptop, and Mobile
- **Success vs. Failed:** Status breakdown to monitor transaction reliability
- **Age Demographics:** Segmented into A1 (≤25), A2 (26–40), A3 (>40)

---

## 🧰 Tools & Technologies

- **Microsoft Power BI Desktop**
- **Microsoft Excel** (data source)
- **DAX** (Data Analysis Expressions)
- **Power Query (M Language)**

---

## 👤 Author

**Amit Yadav**

Built as part of a Power BI learning project covering real-world retail analytics scenarios.

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-blue?logo=linkedin)](https://www.linkedin.com/in/amit-y-3408a2308)

---

## 📄 License

MIT License

Copyright (c) 2025 Amit Yadav

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.

---

> ⭐ If you found this project helpful, please consider giving it a star on GitHub!
