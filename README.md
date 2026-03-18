# Amazon Sales Performance Dashboard
End-to-end data analytics project — 100,000+ raw Amazon sales records cleaned and transformed into an interactive Excel dashboard with Pivot Charts and Slicers.

---

## Project Structure

```
amazon-sales-dashboard/
│
├── data/
│   ├── Amazon.csv                     # Raw uncleaned dataset (100,000 rows)
│   └── Amazon_cleaned.csv             # Cleaned and validated dataset
│
├── dashboard/
│   └── Amazon_DASH.xlsx               # Interactive Excel dashboard
│
├── presentation/
│   └── Sales_Performance_Report.pptx  # Executive summary presentation
│
└── README.md
```

---

## About the Dataset

The raw dataset contains 100,000 Amazon order records with 20 columns:

| Column | Description |
|---|---|
| OrderID | Unique order identifier |
| OrderDate | Date of the order |
| CustomerName | Customer full name |
| ProductName | Name of the product |
| Category | Electronics, Books, Clothing, Home & Kitchen, etc. |
| Brand | Brand name |
| Quantity | Units ordered |
| UnitPrice | Price per unit |
| Discount | Discount percentage applied |
| Tax | Tax amount |
| ShippingCost | Shipping fee |
| TotalAmount | Final transaction value |
| PaymentMethod | Credit Card, UPI, COD, Amazon Pay, etc. |
| OrderStatus | Delivered / Cancelled / Returned |
| City / State / Country | Shipping location |
| SellerID | Seller identifier |

---

## Data Cleaning Steps

Raw file: `data/Amazon.csv` → Cleaned file: `data/Amazon_cleaned.csv`

- Removed duplicate rows and blank entries
- Standardized date formats in OrderDate column
- Fixed inconsistent category and order status labels
- Validated numeric columns — Discount, Tax, TotalAmount
- Removed unwanted index column from raw export

---

## Dashboard Overview

File: `dashboard/Amazon_DASH.xlsx`

The dashboard is built using Pivot Tables and contains 5 interactive charts. Slicers allow filtering by Category, State, and Payment Method.

| Chart | Type | What It Shows |
|---|---|---|
| Sales by Category | Bar Chart | Revenue breakdown across 6 product categories |
| Sales by State | Bar Chart | Top performing US states by total sales |
| Payment Method Share | Pie Chart | Distribution of payment methods used |
| Monthly Sales Trend | Line Chart | Revenue pattern across 12 months |
| Brand Performance | Clustered Bar | Revenue share vs discount rate by brand |

---

## Key Insights

- **Total Revenue** — $242,186 across all orders
- **Top Category** — Electronics at $52,042, followed by Toys & Games at $43,769
- **Top State** — California generated $42,500 in sales
- **Payment Preference** — Credit Card leads at 31.8%, followed by Amazon Pay at 19.6%
- **Peak Months** — November ($28,857) and May ($28,230) had the highest sales
- **Top Brand** — HomeEase held the highest revenue share at 14.1%

---

## Tools Used

- Microsoft Excel — Pivot Tables, Pivot Charts, Slicers, Dashboard Design

---

## How to Use

1. Download or clone this repository
2. Open `dashboard/Amazon_DASH.xlsx` in Microsoft Excel 2016 or later
3. Use the slicers on the dashboard to filter by Category, State, or Payment Method
4. Refer to `data/Amazon_cleaned.csv` for the underlying data
5. Open `presentation/Sales_Performance_Report.pptx` for the summary report


