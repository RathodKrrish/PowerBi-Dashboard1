
# Sales and Orders Dashboard (Power BI)

## Objective

This project is a learning dashboard created with Microsoft Power BI to analyze sales, orders, and profit data. It is intended as a portfolio piece for skill enhancement rather than a stakeholder presentation. The goal is to demonstrate data modeling and visualization capabilities (trends over time, product performance, customer segmentation, etc.) in an interactive report. Each page of the dashboard offers a different perspective, allowing exploration of key business metrics.

## Features and Pages Overview

* **Multi-Page Dashboard:** Six pages of interactive visualizations covering different aspects of sales and order data.
* **Time Series Analysis:** Trends of sales and profit by year, quarter, and month.
* **Product & Category Metrics:** Rankings of products and product lines by sales and orders.
* **Customer Insights:** Customer order details, repeat vs. new order analysis, and customer segments.
* **Geographical Analysis:** Maps and charts showing sales, profit, and order counts by country.
* **Key Performance Indicators (KPIs):** Summary cards and gauges highlighting profit margin, top products, and progress toward revenue targets.

## Charts and Insights (Page by Page Breakdown)

### Page 1 – Sales and Profit Trends

* **Yearly Sales & Profit (Line Chart):** A dual-line chart compares *Sum of Sales* (blue) and *Sum of Profit* (teal) by year (2003–2005). Sales peak in 2004 (~~\$4.2M) and dip in 2005 (~~\$2.0M); profit follows a similar trend but on a smaller scale. This highlights 2004 as the strongest year and 2005 as a slowdown.
* **Quarterly Sales & Profit (Area Chart):** An area chart shows *Sum of Sales* and *Sum of Profit* by quarter (Q1–Q4). It reveals a seasonal pattern: Q4 has the highest combined sales (\~\$4M) and profit, indicating strong holiday-period performance. Q1 is the lowest, suggesting a post-holiday dip.
* **Monthly Profit (Line Chart):** A line chart of *Sum of Profit* by month number (1–12) across all years. There is a notable profit spike around month 11 (November/December), reinforcing the year-end sales surge. The chart shows fluctuations each year, indicating that certain months consistently yield higher profit.
* **Sales by Product Line (Stacked Bar Chart):** A horizontal stacked bar chart breaks down *Sum of Sales* by product line (Classic Cars, Motorcycles, Planes, etc.) and year (color-coded). Classic Cars have the largest total sales (~~\$4M over 2003–05), followed by Planes and Vintage Cars (~~\$3–4M each). Each colored segment shows contributions from 2003 (blue), 2004 (orange), and 2005 (purple). This reveals Classic Cars’ dominance and year-over-year growth for each category.

### Page 2 – Product and Order Metrics

* **Sales by Product (Bar Chart):** A horizontal bar chart of *Sum of Sales* by product name. The top entry is **“1992 Ferrari 360 Spider red”** (approx. \$0.20M sales), followed by other high-end models. This visualization highlights which individual products generate the most revenue.
* **Order Count by Product Line (Bar Chart):** A bar chart of *Count of Orders* (labeled *TotalSpentOn\_QtyOrdered*) by product line. Classic Cars and Vintage Cars have the highest order counts (\~1,000+ orders), while Trains and Ships have the fewest. This indicates product lines that are most in demand.
* **Profit Trend (Line Chart):** A line chart of *Sum of Profit* over time (by year, quarter, and month). Profit peaks occur in January 2004 and 2005 (around \$0.4M), suggesting early-year boosts. The line remains relatively lower mid-year. This chart complements Page 1 by showing finer time granularity for profit fluctuations.
* **Order Quantities (Treemap):** A treemap displaying *Sum of Quantity Ordered* by product line. Each rectangle’s size corresponds to total units sold. Classic Cars occupy the largest area, indicating the highest volume sold, followed by Motorcycles and Planes. Smaller areas for Trains and Ships show they contributed few units.
* **Profit Margin KPI:** A numeric card showing *Profit Margin %* (39.84%). This single-value KPI summarizes overall profitability (profit as a percentage of sales). It provides a quick benchmark of how much of revenue is retained as profit.
* **Top Product KPI:** A KPI card labeled “Most Ordered Product” displays **1992 Ferrari 360 Spider red**. This highlights the product with the highest number of orders, emphasizing its popularity in inventory.
* **Geographic Sales (Map):** A world map with bubbles indicating *Sum of Sales* by country. The largest bubble is over the USA (North America), indicating the highest sales volume there. Other bubbles appear in Europe (e.g. France, UK) and Asia/Australia, showing that sales are distributed globally but concentrated in major markets.

### Page 3 – Orders and Customer Analysis

* **Orders Table:** A detailed table listing individual orders with columns: *Customer Name*, *Order Date*, *Order Number*, *Product Name*, and *Sum of Profit*. This tabular view allows examination of specific transactions. The sample shows multiple orders by “West Coast Collectables Co.”, including model purchases and associated profit. The table’s total profit (approx. \$3.83M shown) provides context for the dataset’s scale.
* **Repeat vs. New Orders (Bar Chart):** A bar chart (blue vs. orange) showing *Count of Orders* by customer, categorized as **“Repeat”** or **“New”** (based on a binary flag “is Order Repeat or not”). Most listed customers (e.g., Alpha Cognac Co., American Collectables) have orders marked “Yes” (repeat), while a few have “No”. This suggests many customers placed more than one order.
* **Revenue by Repeat Status (Cards):** Two KPI cards show *Total Revenue* for repeat vs. new orders. Orders from one-time customers (“No”) account for about **\$7.387M**, whereas repeat customers (“Yes”) contribute **\$1.466M**. This indicates that roughly 83% of revenue comes from non-repeat buyers, highlighting an opportunity to grow repeat business.
* **Revenue vs. Target (Gauge):** A radial gauge chart titled *“Total\_Revenue and TargetRevenue”*. The needle points near \$8.85M, showing performance against a set target (appears around \$9M). The nearly-full blue arc indicates that the revenue is very close to the goal, demonstrating that sales targets have almost been met.
* **Customer Category Distribution (Pie Chart):** A pie chart of *Count of Customer by Category* with slices for **High** (green), **Medium** (blue), and **Low** (red) customer value segments. The chart shows the majority of customers are in the Medium category (largest blue slice), followed by Low and High. This distribution helps understand the customer base composition by value.

### Page 4 – Geographical Sales & Orders

* **Profit by Country (Bar Chart):** A horizontal bar chart of *Sum of Profit* by country. The USA tops the list (~~\$1.0M profit), followed by Spain (~~\$0.2M) and France (\~\$0.15M). Other countries like Australia and New Zealand contribute much smaller profits. This highlights the USA as the most profitable market by far.
* **Order Count by Country (Map and Bar):** The world map (middle) and bar chart (right) both show *Count of Orders* by country. The bar chart shows USA around **950 orders**, far exceeding the next country (Spain \~150). The map uses blue dot sizes to reinforce this geographic distribution (largest dot over USA). This confirms that most orders originate from the USA, with a few hundred from countries like Spain, France, Australia, etc.
* **Sales Flow (Sankey Diagram):** A Sankey (flow) diagram illustrating the path from *Country* ➔ *City* ➔ *Customer Name* ➔ *Sales Amount*. In the screenshot (filtered for Australia), flows show, for example, Australia → Melbourne → “Australian Collectors…” → \$82,261.22. This visual highlights how country-level sales break down into cities and key customers, providing insight into regional contributions.
* **Sales by Country (Table):** A table listing each *Country* and its *Sum of Sales*. It confirms numerical totals: e.g., Australia \$509,385, USA \$0 (hidden by screenshot, presumably the largest), and a grand total of **\$8.853M**. This complements the charts by giving exact figures for each country’s sales.

### Page 5 – Top Products

* **Top Product Sales (Bar Chart):** A single bar chart showing *Sum of Sales* for the top-selling products. The example shows the top 5 products by revenue, with **1992 Ferrari 360 Spider red** highest at about \$0.20M. The other bars represent the next best-selling items (e.g., “2001 Ferrari Enzo” etc.). This page quickly highlights which specific products are the strongest revenue drivers.

### Page 6 – Order Status & Delivery

* **Orders by Year and Line (Stacked Bar):** A horizontal bar chart (titled “Count of TotalSpentOn\_QtyOrder by ProL”) showing the count of orders by year (2003, 2004, 2005) with stacks for each product line (Classic Cars, Motorcycles, etc.). The bars suggest 2004 had the highest total orders (\~150), 2005 a bit lower (\~160), and 2003 the fewest (\~120). Different colors indicate order status (Disputed, In Process, On Hold, Resolved, Shipped), revealing nearly all orders are “Shipped” (blue).
* **Orders by Status (Donut Chart):** A donut chart labeled “Count of orderNumber by status”. It shows the overwhelming majority of orders (large blue segment) are **Shipped**, with very small slivers for In Process, On Hold, Resolved, and Disputed. This indicates operational efficiency: most orders are successfully shipped.
* **Order Status by Country (Bar Chart):** A bar chart “Count of status by country” with status color-coding. The USA has the highest bar (\~100), almost entirely in blue (Shipped), confirming its high shipped-order count. Other countries (Spain, France, Australia, etc.) each have small totals, meaning few orders or mostly shipped. This mirrors Page 4’s findings but broken down by status.
* **Average Delivery Time (Bar Chart):** A bar chart of *Average Delivery Days* by country. It shows **Singapore** with the longest average (\~10 days), followed by Japan (\~8 days) and the Philippines. On the shorter side, **Belgium** and **Switzerland** have the fastest average delivery (\~3–4 days). This highlights regional differences in shipping speed.

## Key KPIs / Highlights

* **Overall Profit Margin:** \~39.8% (from Page 2 KPI card), indicating strong profitability relative to sales.
* **Total Sales vs. Target:** Actual sales \~\$8.85M, just below a \~\$9M goal (Page 3 gauge), meaning nearly 100% of the target met.
* **Sales Breakdown:** USA dominates sales and profit (highest figures on Pages 4 and 6). Europe (especially Spain and France) are secondary markets.
* **Top Product:** *1992 Ferrari 360 Spider red* is the single best-selling product (\~\$0.2M sales, Page 5) and most ordered item (Page 2).
* **Customer Contributions:** A few key customers (e.g., West Coast Collectables Co.) appear multiple times with high-profit orders (Page 3 table).
* **Repeat Business:** Approximately 83% of revenue (\$7.39M vs. \$1.47M) comes from non-repeat customers (Page 3 cards), highlighting an opportunity to improve customer retention.
* **Order Fulfillment:** \~88% of orders are shipped on time (Page 6 donut), and delivery times vary by country (fastest in EU, longest in Asia Pacific).

## Tools Used

* **Microsoft Power BI Desktop:** Primary tool for data modeling and visualization.
* **Built-in and Custom Visuals:** Line charts, bar/column charts, treemaps, pie/donut charts, maps, KPI cards, and a custom Sankey diagram.
* **DAX Measures:** Calculated metrics (e.g., *Profit Margin%*, *Target Revenue*) using Data Analysis Expressions.
* **Data Sources:** (If applicable) sales/order dataset loaded into Power BI (details omitted for privacy as this is a portfolio project).

## How to View

1. **Open in Power BI Desktop:** Download or open the included `XYZCompanyDashboard.pbix` file with Power BI Desktop (free from Microsoft).
2. **Navigate Pages:** Use the left pane tabs to switch between pages (Page 1–Page 6). Each page title is visible at the top.
3. **Interact:** Hover over visuals for tooltips, click on bars/slices/maps to cross-filter other charts, and explore filters (e.g., select a country on the map to drill into that region’s data). The dashboard is fully interactive.
4. **Refresh Data (Optional):** If connected to live data or Excel/CSV sources, click **Refresh** to update the visuals with the latest data. Otherwise, the report is viewable offline with embedded data.

## Screenshots

**Page 1 – Sales and Profit Trends:** Shows annual and quarterly sales vs. profit. The line charts (top) compare sales (blue) and profit (teal) by year and quarter, highlighting 2004 as a peak. The monthly profit line (bottom-left) shows a late-year spike. The stacked bars (bottom-right) break down total sales by product line across years (Classic Cars dominate).

**Page 2 – Product and Order Metrics:** Displays product performance and KPIs. The top-left bar ranks products by sales (Ferrari is top), and the bar next to it shows order counts by product line (Classic Cars lead). Center KPI cards show profit margin (\~39.8%) and the most-ordered product. The treemap (bottom-left) shows order quantities by product line. The map (bottom-right) indicates sales distribution by country (large bubble over USA).

**Page 3 – Orders & Customers:** Focuses on customer orders and revenue. The table (top) lists orders with profit. The right bar chart compares repeat vs. new orders by customer. KPI cards (bottom-left) sum revenue from repeat vs. new buyers. The gauge (bottom-center) shows total revenue against target. The pie (bottom-right) shows customer categories (High/Med/Low).

**Page 4 – Geographical Analysis:** Highlights country-level metrics. The bar chart (top-left) shows profit by country (USA leads). The map (top-center) and bar (top-right) show order counts by country (USA far outnumbers others). The Sankey diagram (bottom-center) flows country → city → customer → sales (filtered to Australia in the view shown). The table (bottom-left) lists total sales by country (USA and others, totaling \~\$8.85M).

**Page 5 – Top Products:** A simple bar chart of the top-selling products by revenue. The screenshot (cropped) shows the five highest products; the Ferrari model is clearly the top seller. This single chart provides a quick view of bestsellers.

**Page 6 – Order Status & Delivery:** Covers order processing metrics. The top-left bar chart shows order counts by year and status (mostly shipped). The donut (bottom-left) confirms that nearly all orders are shipped. The bar (top-right) shows count of orders by country and status (USA has the most, almost all shipped). The bottom-right bar shows average delivery days by country (Singapore highest, EU countries shortest).

## Author and Contribution

**Author:** 
**Krish Rathod**, Data Analytics Student. This dashboard was developed as a personal portfolio project to practice Power BI skills. It is not an official business report. Contributions, feedback, or suggestions are welcome via GitHub issues or pull requests. Feel free to adapt or build upon this work for learning purposes (with credit).
