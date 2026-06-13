#  Adidas US Sales Performance Analysis (2020–2021)

**Author:** Zainab R. Ogunjobi
**Tools:** Microsoft Excel · Power BI
**Dataset:** Adidas US Sales Database
**Status:** ✅ Completed

---

##  Project Overview

This project analyses **2 years of Adidas US retail sales data** across 9,648 transactions covering multiple retailers, regions, product categories, and sales channels. The goal was to identify top-performing regions, retailers, and products — and uncover actionable insights to drive revenue growth and optimise sales strategy.

The analysis was completed using **Excel for data exploration and pivot analysis**, and **Power BI for interactive dashboard visualisation**.

---

##  Key Business Questions

1. How did Adidas US sales grow from 2020 to 2021?
2. Which retailers and regions generate the most revenue and profit?
3. Which product categories have the highest sales and operating margins?
4. How do different sales methods (In-store, Outlet, Online) compare in performance?
5. Which states and months are the strongest performers?
6. Is there a gender-based difference in product sales?

---

##  Repository Structure

```
adidas-sales-performance-analysis/
│
├── data/
│   └── Adidas_Sales_Data.xlsx           ← Raw sales database
│
├── analysis/
│   └── adidas_pivot_analysis.xlsx       ← Pivot tables, calculated fields & charts
│
├── dashboard/
│   └── adidas_dashboard.pbix            ← Power BI interactive dashboard
│   └── dashboard_preview.png            ← Screenshot of final dashboard
│
├── visuals/
│   ├── sales_by_region.png              ← Bar chart — regional performance
│   ├── sales_by_retailer.png            ← Bar chart — retailer comparison
│   ├── sales_by_product.png             ← Bar chart — product category breakdown
│   ├── monthly_trend.png                ← Line chart — monthly sales trend
│   └── sales_method_comparison.png      ← Channel performance comparison
│
└── README.md
```

---

##  Dataset Overview

| Detail | Info |
|--------|------|
| Source | Adidas US Sales Database (Practice Dataset) |
| Period | January 2020 — December 2021 |
| Total Transactions | 9,648 |
| Total Units Sold | 2,478,861 |

**Key Columns:**

| Column | Description |
|--------|-------------|
| Retailer | Name of the retail partner |
| Retailer ID | Unique retailer identifier |
| Invoice Date | Date of transaction |
| Region | US geographic region |
| State / City | Location details |
| Gender Type | Men's or Women's product line |
| Product Category | Street Footwear, Apparel, Athletic Footwear |
| Price per Unit | Unit selling price (USD) |
| Units Sold | Quantity sold per transaction |
| Total Sales | Gross revenue per transaction |
| Operating Profit | Profit after operating costs |
| Operating Margin | Profit as % of sales |
| Sales Method | In-store, Outlet, or Online |

---

##  Data Preparation Steps

Performed in **Excel** before analysis:

- ✅ Converted `Invoice Date` from Excel serial number to proper date format
- ✅ Extracted `Month` and `Year` columns for time-series analysis
- ✅ Verified `Operating Margin` as a decimal — converted to percentage for readability
- ✅ Checked for and confirmed zero duplicate records
- ✅ Validated no null values in key columns (Total Sales, Operating Profit, Region)
- ✅ Standardised text fields (Region, Product Category, Sales Method) for consistent grouping
- ✅ Created calculated column: `Profit per Unit = Operating Profit / Units Sold`

---

## 📊 Key Findings & Insights

###  Overall Business Performance

| KPI | Value |
|-----|-------|
| Total Revenue (2 Years) | **$899,902,125** |
| Total Operating Profit | **$332,134,761** |
| Overall Operating Margin | **36.9%** |
| Total Units Sold | **2,478,861** |
| Total Transactions | **9,648** |

> 🔍 **Insight:** Adidas achieved a strong 36.9% operating margin across the US market, demonstrating healthy pricing power and cost discipline across all sales channels.

---

### 📈 Revenue Growth by Year

| Year | Total Sales | Growth |
|------|-------------|--------|
| 2020 | $182,080,675 | Baseline |
| 2021 | $717,821,450 | **+294% YoY** |

> 🔍 **Insight:** Revenue surged by nearly 4x in 2021 following the disruption of 2020 (COVID-19 impact on retail). This dramatic recovery reflects pent-up consumer demand and the rapid expansion of online and outlet channels post-pandemic.

---

### 🗺️ Sales by Region

| Region | Total Sales |
|--------|-------------|
| West | $269,943,182 |
| Northeast | $186,324,067 |
| Southeast | $163,171,236 |
| South | $144,663,181 |
| Midwest | $135,800,459 |

> 🔍 **Insight:** The **West region leads with 30% of total US revenue**, driven by high-volume states like California. The Midwest underperforms relative to population size — a potential market development opportunity.

---

### 🏪 Sales by Retailer

| Rank | Retailer | Total Sales |
|------|----------|-------------|
| 1 | West Gear | $242,964,333 |
| 2 | Foot Locker | $220,094,720 |
| 3 | Sports Direct | $182,470,997 |
| 4 | Kohl's | $102,114,753 |
| 5 | Amazon | $77,698,912 |
| 6 | Walmart | $74,558,410 |

> 🔍 **Insight:** **West Gear and Foot Locker together account for 51% of total sales** — a significant dependency on two retail partners. Strengthening the Amazon and direct-to-consumer online channel could reduce this concentration risk.

---

### 👟 Sales by Product Category

| Product Category | Total Sales | Operating Profit | Margin |
|-----------------|-------------|-----------------|--------|
| Street Footwear | $336,829,057 | $127,898,100 | 38.0% |
| Apparel | $302,767,492 | $113,414,000 | 37.5% |
| Athletic Footwear | $260,305,576 | $90,822,670 | 34.9% |

> 🔍 **Insight:** **Street Footwear is the star category** — highest revenue AND highest margin at 38%. Athletic Footwear has the lowest margin, suggesting pricing pressure or higher production costs in this segment.

---

### 👫 Sales by Gender

| Gender | Total Sales |
|--------|-------------|
| Men's | $486,228,556 (54%) |
| Women's | $413,673,569 (46%) |

> 🔍 **Insight:** Men's products edge ahead in revenue, but Women's represents a nearly equal and growing segment. Investing in Women's product expansion and marketing could close this gap and unlock significant revenue upside.

---

### 🛒 Sales by Channel

| Sales Method | Total Sales |
|-------------|-------------|
| In-store | $356,643,750 (40%) |
| Outlet | $295,585,493 (33%) |
| Online | $247,672,882 (27%) |

> 🔍 **Insight:** In-store remains dominant, but **Online at 27% represents a fast-growing and scalable channel** with lower overhead costs. Shifting investment toward e-commerce could significantly improve overall margins.

---

### 📅 Monthly Sales Trend

| Peak Months | Sales | Slow Months | Sales |
|-------------|-------|-------------|-------|
| July | $95,480,694 | March | $56,809,109 |
| August | $92,166,201 | February | $61,100,153 |
| December | $85,841,957 | October | $63,911,033 |

> 🔍 **Insight:** **Summer (July–August) and the holiday season (December) are peak periods**, driven by back-to-school shopping and festive demand. Q1 (Jan–March) is consistently slower — a strong window for clearance sales or new product launches to stimulate demand.

---

### 🌎 Top 5 States by Revenue

| State | Total Sales |
|-------|-------------|
| New York | $64,229,039 |
| California | $60,174,133 |
| Florida | $59,283,714 |
| Texas | $46,359,746 |
| South Carolina | $29,285,637 |

---

## 💡 Business Recommendations

1. **Double down on Street Footwear** — highest revenue and margin. Prioritise new product launches and seasonal campaigns in this category.

2. **Accelerate online channel growth** — Online is the most scalable channel with lower costs. A 5% shift from in-store to online could meaningfully improve overall margin.

3. **Invest in the Women's segment** — at 46% of sales and growing, Women's products represent the highest upside opportunity. Targeted campaigns and exclusive product lines could close the gender revenue gap.

4. **Develop Midwest market** — underperforms relative to US population share. Targeted retailer partnerships or marketing spend in key Midwest cities could unlock new revenue.

5. **Leverage peak season inventory planning** — July, August, and December are consistently peak. Supply chain and inventory should be optimised 6–8 weeks ahead of these windows.

6. **Reduce retailer concentration** — West Gear + Foot Locker = 51% of sales. Diversifying across Amazon and direct-to-consumer online reduces risk and increases margin.

---

## 🛠️ How to Explore This Project

**Excel Analysis:**
1. Open `adidas_pivot_analysis.xlsx`
2. Navigate to `Pivot Analysis` tab — sales by region, retailer, product, and channel
3. Navigate to `Charts` tab for visual summaries

**Power BI Dashboard:**
1. Download and install [Power BI Desktop](https://powerbi.microsoft.com/desktop/) (free)
2. Open `adidas_dashboard.pbix`
3. Use slicers to filter by Year, Region, Retailer, Product Category, and Sales Method

---

## 🚀 Skills Demonstrated

- ✅ Data cleaning and preparation in Excel
- ✅ Pivot table creation and multi-dimensional analysis
- ✅ Revenue and profitability analysis across segments
- ✅ Regional and geographic performance mapping
- ✅ Channel and retailer benchmarking
- ✅ Power BI interactive dashboard design
- ✅ Business insight generation and strategic recommendations

---

## 👩‍💻 About the Author

**Zainab R. Ogunjobi** is an Economics graduate and data analyst based in Lagos, Nigeria, with hands-on experience in financial reporting, data management, and business performance analysis.

🌐 [Portfolio](https://zainab-ogunjobi-va.netlify.app) · 💼 [LinkedIn](https://linkedin.com/in/ogunjobi-zainab) · 📧 [Email](mailto:Zainabogunjobir@gmail.com)

---

*Part of my Data Analytics Portfolio — feel free to fork or reach out with feedback!*
