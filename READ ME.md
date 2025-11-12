🛒 Amazon India Sales Analytics Dashboard | Tableau Project

In the fast-moving world of e-commerce, every order tells a story — of customer behavior, delivery performance, and business rhythm.

This Tableau project visualizes Amazon India’s Sales Operations, turning thousands of sales records into a clear and interactive picture of performance — from order quantities and courier statuses to weekly trends and regional distribution.

It’s not just about numbers. It’s about how operations data reveals efficiency, customer satisfaction, and the hidden flow of business decisions.

🎯 Project Objective

Amazon generates millions of transactions every day — but operational intelligence often hides beneath raw order data.
The goal of this project was to create a single-page Tableau dashboard that:

Maps sales quantity trends by week and product category.

Tracks courier performance (Shipped, Unshipped, Cancelled).

Monitors regional order distribution across Indian states.

Highlights B2B vs retail share, sales channel mix, and size-level breakdowns.

In short — to visualize the heartbeat of Amazon’s sales pipeline.

🧩 Data Model & Files
File	Description
Amazon Sale Report.csv	Raw dataset containing 116,649 orders — product category, courier status, channel, amount, size, quantity, state, and service level.
Amazon.Sales.India.Dashboard.twbx	Tableau packaged workbook with all visuals, metrics, and filters.
Amazon.Sales.Dashboard.png	Dashboard preview for documentation.
Tableau Public Link
	Interactive version of the dashboard.
⚙️ Tools & Techniques

Tableau Desktop / Tableau Public – interactive visualization and data modeling

Excel / CSV – data cleaning and formatting

Mapbox integration – state-level visualizations

Calculated Fields in Tableau:

Total_Quantity = SUM([Qty])

Total_Amount = SUM([Amount])

B2B_Flag = IF [is_b2b] = TRUE THEN "B2B" ELSE "Retail" END

Ship_Status = IF CONTAINS([Courier Status], "Shipped") THEN "Shipped" ELSEIF ... END

🧮 Data Preparation

1️⃣ Cleaned Missing & Categorical Values

Replaced null courier statuses and category blanks.

Unified inconsistent product categories (case normalization).

2️⃣ Feature Engineering

Extracted week numbers and months from Order Date.

Derived B2B / Non-B2B flag.

Standardized courier states for map compatibility.

3️⃣ Validation

Cross-checked quantity vs total amount to verify data accuracy.

📊 Dashboard Storyline

The Tableau dashboard was designed as a multi-layer visual system — combining performance, logistics, and regional data.

1️⃣ Top-Level KPIs

At the top sit six major indicators:

Total Products: 7,190

Total Categories: 9

Total Sizes: 11

Total Quantity: 116,649

Total Amount: ₹78,592,678

Total B2B Orders: <1% of total

Each KPI updates dynamically with filters.

2️⃣ Sales Trends by Week & Category

A dual-axis chart shows weekly order quantities by category — exposing seasonal peaks in May and June, likely influenced by mid-year promotional campaigns and Prime Day preparations.

3️⃣ Courier & Channel Performance

Shipped: 94.2%

Unshipped: 5.7%

Cancelled: <0.1%

Amazon.in dominates the channel split (99.8%), proving direct channel trust and customer dependency over third-party retail.

4️⃣ Regional Insights

A Mapbox-powered map highlights India’s sales distribution:

Maharashtra, Karnataka, and Tamil Nadu top the chart — consistent with strong urban e-commerce penetration.

Eastern states and the northeast show emerging volume but lower B2B engagement.

The Top 10 State Breakdown table links directly to service levels (Expedited vs Standard), offering operational benchmarking.

5️⃣ Category & Size Distribution

Horizontal bars reveal how M, L, and XL sizes dominate apparel sales, indicating preference clustering.
Categories such as Clothing, Footwear, and Electronics drive recurring revenue volumes.

6️⃣ Courier Status + Service Efficiency

Bar charts show shipped quantities vs cancelled or pending.
The insight? Amazon’s fulfillment accuracy exceeds 94%, signaling logistics maturity and minimal return-to-seller rates.

🔍 Analytical Highlights
Metric / Insight	Observation
Fulfillment Accuracy	94% of orders are successfully shipped.
Cancellation Rate	Only 0.1%, indicating strong order confidence and system reliability.
Regional Dominance	Maharashtra & Karnataka lead, followed by Tamil Nadu and Telangana.
Sales Channel Mix	99.8% Amazon.in — centralized logistics system performing optimally.
Size Preference	M & L sizes account for over 30% of total sales volume.
🎨 Design Philosophy

Amazon’s brand is synonymous with clarity, trust, and operational precision, and the dashboard reflects exactly that:

Color Scheme: Amazon’s signature teal-blue base with orange and cyan accents.

Visual Layout: Horizontal grid alignment for efficiency metrics at the top, regional & product insights at the bottom.

Typography: Segoe UI — modern, legible, and consistent with Amazon’s UI aesthetic.

Interactivity: Filters for category, courier status, and channel make this a functional business command center.

🧠 Insights & Business Value

1️⃣ Operations Excellence – With shipment reliability above 94%, Amazon’s backend performance aligns with its customer promise: “Delivering smiles.”
2️⃣ Low Cancellation, High Trust – The micro 0.1% cancellation rate reflects customer and seller alignment.
3️⃣ Strategic B2B Expansion Opportunity – B2B orders represent <1%, signaling potential growth avenues in bulk procurement or seller network optimization.
4️⃣ Predictable Sales Cycles – Weekly and monthly spikes indicate campaign-driven growth, ideal for demand forecasting models.

💡 What I Learned

This project was a deep dive into operational storytelling through data.
It refined how I approach large transactional datasets and turn them into clean, executive-ready visuals.

It taught me:

How to create hierarchical layouts that tell layered stories (macro → micro).

The importance of operational KPIs in retail analytics.

How regional sales mapping reveals both market dominance and opportunity zones.

That dashboards can serve as both analytical tools and strategic mirrors for leadership.