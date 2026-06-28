# Part 4: Tableau Executive Dashboard

## Business Problem Summary

The objective of this project is to build an executive dashboard that helps the retail leadership team monitor overall business performance. The dashboard provides insights into sales trends, regional performance, profitability, customer segments, shipping performance, discount impact, and product returns to support data-driven decision making.

---

## Dataset Description

**Dataset Name:** dashboard_sales_data.xlsx

The dataset contains retail sales transactions with information such as:

- Order Date
- Ship Date
- Sales
- Profit
- Discount
- Region
- State
- Category
- Sub-Category
- Customer Segment
- Ship Mode
- Returned Orders

The dataset was used to create interactive Tableau visualizations and business insights.

---

## Tableau Workbook

**Workbook Name:** executive_dashboard.twbx

The workbook contains:

- Executive Dashboard
- Sales Trend View
- Regional Performance View
- Category Profitability View
- Customer Segment View
- Shipping Performance View
- Discount vs Profit Analysis
- Return Analysis View

---

## Calculated Fields Created

The following calculated fields were created in Tableau:

1. **Profit Margin**

```text
SUM([Profit]) / SUM([Sales])
```

2. **Cost**

```text
SUM([Sales]) - SUM([Profit])
```

3. **Average Order Value**

```text
SUM([Sales]) / COUNTD([Order ID])
```

4. **Return Rate**

```text
SUM([Return Flag]) / COUNTD([Order ID])
```

5. **Shipping Delay Bucket**

```text
IF [Delivery Days] <= 2 THEN "Fast Delivery"
ELSEIF [Delivery Days] <= 5 THEN "Medium Delivery"
ELSE "Slow Delivery"
END
```

---

## Dashboard Components

The executive dashboard includes:

- Monthly Sales Trend
- Regional Sales Performance
- Category Profitability
- Customer Segment Performance
- Shipping Performance
- Discount vs Profit Analysis
- Return Analysis

It also includes KPI cards for:

- Total Sales
- Total Profit
- Profit Margin
- Return Rate

---

## Filters and Interactions

Interactive filters included:

- Region
- Category
- Customer Segment
- Ship Mode
- Order Date

Dashboard Action:

- Selecting a region filters all dashboard visualizations.

---

## Key Business Insights

- Sales reached the highest level in **August 2025**.
- Sales were lowest in **May 2025**.
- South generated the highest sales.
- East generated the lowest sales.
- Technology category produced the highest profit.
- Furniture category generated the lowest profit.
- Home Office was the best-performing customer segment.
- Higher discounts reduced profitability.
- Same Day shipping delivered the fastest orders.
- Furniture recorded the highest return rate.

---

## Dashboard Story Summary

The dashboard highlights both business strengths and operational challenges.

Strong sales growth, profitable technology products, and the Home Office customer segment represent major business opportunities. However, high discounts, low-performing furniture products, longer Standard Class deliveries, and high return rates require management attention.

The dashboard enables executives to monitor KPIs, identify trends, and make informed business decisions.

---

## Assumptions and Limitations

### Assumptions

- Sales and Profit values are accurate.
- Delivery Days are calculated using Order Date and Ship Date.
- Return Flag correctly identifies returned orders.

### Limitations

- Historical data only.
- No predictive forecasting.
- No external market or competitor data.
- Results depend on the available dataset.

---

## Repository Structure

```

part4_tableau_dashboard/
├── data/
│ └── dashboard_sales_data.xlsx
├── tableau/
│ └── executive_dashboard.twbx
├── outputs/
│ ├── business_insights.md
│ ├── dashboard_story.md
│ └── chart_selection_justification.md
├── screenshots/
│ ├── full_dashboard.png
│ ├── sales_trend_view.png
│ ├── regional_performance_view.png
│ ├── category_profitability_view.png
│ └── filter_interaction_view.png
└── README.md

```

---

## Screenshots Included

- ✅ Full Executive Dashboard
- ✅ Monthly Sales Trend
- ✅ Regional Performance
- ✅ Category Profitability
- ✅ Filter Interaction

---

## Conclusion

This Tableau Executive Dashboard provides leadership with an interactive view of retail business performance. It enables quick identification of sales trends, profitable categories, customer behavior, operational issues, and strategic opportunities through KPIs, interactive filters, and business-focused visualizations.