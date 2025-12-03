Excel-Walmart-Dynamic-Dashboard
The Dynamic Retail Dashboard is an interactive and data-driven tool built in Excel to visualize and analyze retail data. It connects to datasets hosted on GitHub, uses Power Query for data transformation, and presents insights through dynamic charts and KPIs. The dashboard solves key business questions, enabling informed decision-making.

Orders Table The Orders table contains detailed information about customer orders, including product, shipping, and financial metrics.
🔸 Sample Data:

Order ID Returned Order Date Ship Date Ship Mode Customer Name Segment Country Market Sales Profit Discount CA-2012-124891 No 31-07-2020 31-07-2020 Same Day Rick Hansen Consumer United States US 2309.65 762.18 0 IN-2013-77878 Yes 05-02-2021 07-02-2021 Second Class Justin Ritter Corporate Australia APAC 3709.40 -288.77 0.1 IN-2013-71249 No 17-10-2021 18-10-2021 First Class Craig Reiter Consumer Australia APAC 5175.17 919.97 0.1

Returns Table The Returns table tracks orders that were returned, along with the associated markets.
🔸 Sample Data:

Returned Order ID Market Yes MX-2013-168137 LATAM Yes US-2011-165316 LATAM Yes ES-2013-1525878 EU Yes CA-2013-118311 United States

People Table The People table contains information about sales representatives and their assigned regions.
🔸 Sample Data:

Person Region Anna Andreadi Central Chuck Magee South Kelly Williams East Matt Collister West Deborah Brumfield Africa

🧩 Problem Statements Solved with Steps & Insights

Key Performance Indicators (KPIs) 🎯 Objective: Display key metrics such as Total Sales, Profit, Quantity, Orders, and Profit Margin.
🛠 Steps:

Import Orders table via Power Query.

Create calculated columns:

Profit Margin = Profit / Sales

Total Orders = Count of Order ID

Use Excel formulas to calculate:

=SUM(Sales) → Total Sales

=SUM(Profit) → Total Profit

=SUM(Quantity) → Total Quantity

Display in a KPI card format with symbols/icons.

image
📈 Visual: KPI card section 💡 Insight: Gives a snapshot of business performance in real-time.

Sales and Profit Trend Analysis 🎯 Objective: Identify sales and profit trends over time.
🛠 Steps:

Group Order Date by Year-Month using Pivot Table.

Add Sales and Profit as values.

Use a Line Chart to display trends.

Add slicers for filters (e.g. Market, Region).

📈 Visual: Line chart with slicers 💡 Insight: Strong peak in Q4; vital for seasonal planning.

image
Category-Wise Profit Analysis 🎯 Objective: Compare profit across product categories.
🛠 Steps:

Create Pivot Table with Category in rows and Profit as values.

Sort descending to identify top contributors.

Build a Bar Chart for visual display.

Use slicers for category/region drill-down.

📈 Visual: Bar chart (Profit by Category) 💡 Insight: Technology leads; Furniture may need strategy review.

image
Segment-Wise Sales Share (%) 🎯 Objective: Show sales distribution by customer segments.
🛠 Steps:

Create Pivot Table: Segment → Rows, Sales → Values.

Calculate % Share: =Sales / Total Sales * 100

Use Pie or Donut Chart with dynamic labels.

📈 Visual: Donut chart 💡 Insight: Consumer segment has the highest contribution.

image
Sales by Country 🎯 Objective: Track performance by country.
🛠 Steps:

Create Pivot Table with Country as rows and Sales as values.

Sort in descending order.

Apply Heatmap or Conditional Formatting.

📈 Visual: Heatmap or conditional formatting table 💡 Insight: United States dominates; Africa underperforms.

image
Top 5 Performing Subcategories 🎯 Objective: Highlight top-selling product subcategories.
🛠 Steps:

Pivot Table: Sub-Category → Rows, Sales → Values.

Sort descending; filter top 5.

Use Column Chart to visualize.

image
📈 Visual: Column chart (Top 5 Subcategories) 💡 Insight: Phones and Accessories dominate sales.

⚙️ Dynamic Features Used ✅ Dynamic Charts with real-time filters via slicers

✅ Power Query for data import and transformation

✅ KPI Card Section with calculated metrics

✅ Interactivity through Pivot Filters and Timelines

📈 Additional Insights (Next Steps) Potential extensions to the dashboard:

🔄 Return Analysis: Explore return trends by product or region

📉 Top & Bottom Customers: Identify profitable and unprofitable clients

🌍 Market Comparison: Deep-dive into global performance

📦 Product-Level Analysis: Break down product-specific contribution

🎯 Significance This dashboard enables retail businesses to:

Track KPIs and sales metrics in real time

Identify profit-driving categories and regions

Optimize decision-making with visual clarity

Discover inefficiencies in returns and discounting

image
📷 Visuals Included This repository includes:

📌 Visuals for each solved problem statement

📌 Snapshots of the full dashboard

📌 Data insights and metrics in context
