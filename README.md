# 📊 Sales Dashboard — Excel Workbook

An interactive Excel-based sales dashboard that tracks product sales performance across regions, salespeople, and time periods for the year **2021**.

---
![Sales_Dashboard_page-0001](https://github.com/user-attachments/assets/e205bf88-dccb-40e3-9666-3fcb7ece8b0d)



## 🗂️ Workbook Structure

The workbook contains **5 sheets**, each serving a distinct purpose:

| Sheet | Description |
|-------|-------------|
| `Dashboard` | Main visual dashboard with charts and KPI summaries |
| `Product` | Reference/lookup data for products |
| `Salesman` | Reference/lookup data for salespeople |
| `Pivot_table` | Pre-built pivot tables used to power the dashboard |
| `Data` | Raw transactional sales data (source of truth) |

---

## 📋 Data Sheet — Schema

The `Data` sheet contains **366 rows** of daily sales transactions spanning **January 1, 2021 to January 1, 2022**.

| Column | Type | Description |
|--------|------|-------------|
| `S No` | Integer | Serial / row number |
| `Date` | Date | Transaction date |
| `Salesman` | Text | Name of the salesperson |
| `Region` | Text | Sales region (East, West, North, South) |
| `Item` | Text | Product sold |
| `Qty` | Integer | Quantity sold |
| `Price` | Integer | Unit price (INR) |
| `Amount` | Formula | Computed as `Qty × Price` |

---

## 📈 Key Metrics

### Overall

| Metric | Value |
|--------|-------|
| Total Records | 366 transactions |
| Total Revenue | ₹18,25,700 |
| Date Range | Jan 2021 – Jan 2022 |

---

### 💰 Revenue by Month

| Month | Revenue (₹) |
|-------|------------|
| January | 1,43,130 |
| February | 2,24,470 |
| March | 86,100 |
| April | 1,53,530 |
| May | 1,10,160 |
| June | 1,18,530 |
| July | 1,30,100 |
| August | 1,56,300 |
| September | 2,23,770 |
| October | 1,97,350 |
| November | 31,520 |
| December | 2,07,610 |

> **Peak month:** February & September &nbsp;|&nbsp; **Lowest month:** November

---

### 🗺️ Revenue by Region

| Region | Revenue (₹) | Share |
|--------|------------|-------|
| East | 7,36,080 | 41.3% |
| West | 5,07,330 | 28.5% |
| South | 3,35,480 | 18.8% |
| North | 2,03,680 | 11.4% |

---

### 🧑‍💼 Revenue by Salesman

| Salesman | Revenue (₹) |
|----------|------------|
| Siddhu | 5,51,960 |
| Rohit Das | 3,94,410 |
| Ajit Kumar | 3,86,030 |
| Amit | 1,84,690 |
| Ramesh | 1,39,880 |
| Chandu | 1,25,600 |

---

### 🖨️ Revenue by Product

| Product | Revenue (₹) | Share |
|---------|------------|-------|
| Printer | 9,34,500 | 52.4% |
| Scanner | 3,52,200 | 19.8% |
| Monitor | 3,39,000 | 19.0% |
| Mouse | 66,150 | 3.7% |
| Speaker | 65,400 | 3.7% |
| Keyboard | 25,320 | 1.4% |

> **Printer alone accounts for over half of total revenue.**

---

## 🔧 How It Works

1. **Raw data** is entered in the `Data` sheet. The `Amount` column is auto-calculated using the formula `=Qty × Price`.
2. **Pivot tables** in the `Pivot_table` sheet aggregate data by month, region, product, and salesman.
3. The **Dashboard** sheet visualises these pivot tables using Excel charts and slicers.
4. `Product` and `Salesman` sheets act as **reference tables** for dropdowns or lookups.

---

## 🚀 Getting Started

1. **Clone or download** this repository.
2. Open `Dashboard__Recovered_.xlsx` in **Microsoft Excel** (2016 or later recommended).
3. Navigate to the `Dashboard` sheet to view the interactive summary.
4. Use **slicers** (if enabled) to filter by region, salesman, or product.
5. To add new data, append rows to the `Data` sheet — pivot tables can be refreshed via `Data → Refresh All`.

---

## 🛠️ Tech Stack

- **Microsoft Excel** (.xlsx format)
- Pivot Tables & Charts
- Excel Slicers for interactivity

---

## 📄 License

This project is for educational/portfolio purposes. Feel free to use and adapt.
