# 💳 UPI Transaction Analytics Dashboard — Power BI

## 📌 Project Overview

This project is an end-to-end **UPI (Unified Payments Interface) Transaction Analytics Dashboard** built using **Microsoft Power BI**. It analyzes **20,000 real-world-style UPI transactions** to uncover patterns in payment behaviour, transaction success rates, city-wise spending, and demographic insights.

The dashboard is designed to help business analysts and fintech teams quickly visualize and explore digital payment trends across multiple dimensions.

---

## 📂 Dataset

| Property | Details |
|---|---|
| **File** | `UPI_Transactions.xlsx` |
| **Records** | 20,000 transactions |
| **Source Sheet** | Sheet1 (renamed to `UPI Transaction`) |
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

## 📈 Dashboard Features

### 🎛️ Slicers & Filters
- Multiple slicers with **Sync Slicer** enabled across pages (via View Tab)
- Slicers formatted and aligned for clean visual layout
- Canvas background customized for improved aesthetics

### 📉 Visualizations
- **Line Chart & Column Chart** with **Bookmark Toggle** — users can switch between chart types interactively
- **Conditional Formatting** on visuals — lighter color for lowest values, darker for highest
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

** Amit Yadav **
- 📧 amit.y21c@gmail.com
- 💼 [LinkedIn Profile](https://www.linkedin.com/in/amit-y-3408a2308/))
---

## 📜 License

This project is licensed under the [MIT License](LICENSE).

---

> ⭐ If you found this project helpful, please consider giving it a star on GitHub!
