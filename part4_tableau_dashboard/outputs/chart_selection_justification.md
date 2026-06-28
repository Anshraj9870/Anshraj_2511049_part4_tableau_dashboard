# Chart Selection Justification

## 1. Monthly Sales Trend

### Business Question
How are sales changing over time?

### Chart Type
Line Chart

### Why This Chart?
A line chart is the best choice for showing trends over time because it clearly displays increases and decreases in sales across different months.

### Fields Used
- Columns: Order Date (Month)
- Rows: SUM(Sales)
- Color: Blue
- Filter: Region, Category, Customer Segment, Ship Mode, Order Date

### Design Principle Applied
- Simple time-series visualization
- Clear axis labels
- Minimal clutter
- Easy trend identification

### Mistake Avoided
Avoided using a pie chart or bar chart for time-series analysis.

---

## 2. Regional Sales Performance

### Business Question
Which region generates the highest sales?

### Chart Type
Horizontal Bar Chart

### Why This Chart?
A horizontal bar chart makes it easy to compare sales across multiple regions.

### Fields Used
- Rows: Region
- Columns: SUM(Sales)
- Color: Profit
- Label: Sales
- Filter: Region, Category, Customer Segment

### Design Principle Applied
- Descending sorting
- Consistent color usage
- Easy comparison

### Mistake Avoided
Avoided using a pie chart because comparing multiple regions is difficult in a pie chart.

---

## 3. Category Profitability

### Business Question
Which categories and sub-categories generate the highest and lowest profit?

### Chart Type
Horizontal Bar Chart

### Why This Chart?
A bar chart clearly compares profit values across different product categories.

### Fields Used
- Rows: Sub-Category
- Columns: SUM(Profit)
- Color: Category
- Label: Profit

### Design Principle Applied
- Sorted from highest to lowest profit
- Clear color distinction
- Easy comparison

### Mistake Avoided
Avoided using stacked charts that make profitability comparisons difficult.

---

## 4. Customer Segment Performance

### Business Question
Which customer segment contributes the most sales?

### Chart Type
Horizontal Bar Chart

### Why This Chart?
A bar chart provides a simple comparison between customer segments.

### Fields Used
- Rows: Customer Segment
- Columns: SUM(Sales)
- Label: SUM(Profit)

### Design Principle Applied
- Simple comparison
- Clear labels
- Business-friendly formatting

### Mistake Avoided
Avoided unnecessary 3D visualizations.

---

## 5. Shipping Performance

### Business Question
Which shipping mode delivers orders the fastest?

### Chart Type
Horizontal Bar Chart

### Why This Chart?
The chart clearly compares average delivery time across shipping modes.

### Fields Used
- Rows: Ship Mode
- Columns: AVG(Delivery Days)
- Color: Shipping Delay Bucket

### Design Principle Applied
- Easy comparison
- Consistent color coding
- Sorted values

### Mistake Avoided
Avoided using a line chart because shipping modes are categorical data.

---

## 6. Discount vs Profit Analysis

### Business Question
How does discount affect profit?

### Chart Type
Scatter Plot

### Why This Chart?
A scatter plot is ideal for identifying relationships between two continuous variables.

### Fields Used
- Columns: Discount
- Rows: Profit
- Detail: Order ID
- Color: Profit

### Design Principle Applied
- Shows correlation clearly
- Individual order-level analysis
- Minimal visual clutter

### Mistake Avoided
Avoided using a bar chart because it cannot effectively display relationships between two numerical variables.

---

## 7. Return Analysis

### Business Question
Which product category has the highest number of returned orders?

### Chart Type
Horizontal Bar Chart

### Why This Chart?
A bar chart makes return comparisons across categories simple and easy to understand.

### Fields Used
- Rows: Category
- Columns: SUM(Return Flag)
- Color: Customer Segment

### Design Principle Applied
- Clear comparison
- Simple layout
- Consistent formatting

### Mistake Avoided
Avoided using a pie chart because comparing return counts across categories is more accurate with bars.

---

# Overall Dashboard Design Principles

The dashboard follows standard data visualization best practices:

- Appropriate chart selection for each business question.
- Consistent colors throughout the dashboard.
- Clear titles and labels.
- Descending sorting for better readability.
- Interactive filters for easy exploration.
- KPI cards for quick executive summary.
- Minimal clutter and balanced dashboard layout.
- Business-friendly formatting focused on decision-making.