# Sales Performance Analysis – 2019

**Company:** Electra Retail Inc. (fictional electronics retailer)

**Prepared for:** Sales Strategy Team (primary), Executive Management (secondary)

**Analytics Stack:** Power BI (with DAX measures & calculated columns)

## 1. Project Background
Electra Retail Inc. sells consumer electronics across major U.S. cities (laptops, smartphones, monitors, TVs, accessories, and select home electronics). This report analyzes 2019 transactions to identify which products, time windows, and cities should be prioritized to maximize revenue in the coming planning cycle.

## 2. Project Goals & Audience

- **Audience:** Sales Strategy Team → to drive portfolio/market actions; Executives → to align spend and targets.
- **Primary Goal:** Determine which products and markets to prioritize and when to concentrate promotions to lift revenue efficiently.
- **Secondary Goals:**
    - Separate revenue drivers from unit/volume drivers.
    - Pinpoint peak demand windows and high-growth markets.

## 3. Data Structure Overview

Transactional dataset (2019). Each row = one order.

**Columns**

Order ID, Product, Quantity Ordered, Price Each, Order Date, Purchase Address, Month, Sales, City, Hour.

**Key DAX artifacts** (created in Power BI)
- Monthly MoM Growth % (product and total)
- Average Order Value (AOV)
- Price-range banding
- Date from datetime

## 4. Executive Summary (30-second read)

- **Topline:** **$34.49M** total sales; **AOV** ≈ $193; latest MoM growth ≈ **44%** into year-end.
- **Units:** **209K** total products sold.
- **Products:** **MacBook Pro ($8.0M), iPhone ($4.8M), ThinkPad ($4.1M)** lead revenue; accessories dominate unit volume but contribute marginal revenue.
- **Geography:** **San Francisco** is the largest market (~$8.3M). **Seattle** is the **top growth city (+53.6% MoM)**. The **top 3 cities account for ~53%** of sales.
- **Timing:** Sales peak **7 PM**; steady demand across days; **weekend share ≈ 28.5%.**
- **Price Behavior:** Purchases **> $1,000** contribute **$8.0M—entirely** from **MacBook Pro at $1,700**.

### Dashboard Previews
Here are the snapshots from my analysis dashboard:

- Executive Summary Dashboard (Page 1)
![Page 1 Dashboard](/Images/Executive%20Page%20Dashboard.png)

- Product Deep Dive Dashboard (Page 2)
![Page 2 Dashboard](/Images/Product%20Page%20Dashboard.png)

- Time & Geographic Insights Dashboard (Page 3)
![Page 3 Dashboard](/Images/Time%20&%20Location%20Page%20Dashboard.png)

[View Interactive Dashboard here on the Power BI service](https://app.powerbi.com/groups/me/reports/105f400e-f7e7-4177-b2e0-8368d2956900/66e708631715771ae331?experience=power-bi)

## 5. Insights Deep-Dive
### 5.1 Sales Trend & Seasonality
- Monthly sales climb from **$1.8M (Jan)** to **$4.6M (Dec)—~2.5×** increase, driven by holiday demand and Q4 promotions.
- Latest **MoM growth ≈ 44%**, reflecting a strong finish.
### 5.2 Product Insights
**Revenue leaders (2019):**

- **MacBook Pro Laptop – $8.0M** (top contributor; also **Top Product AOV ≈ $1,703)**.
- **iPhone – $4.8M; ThinkPad Laptop – $4.1M; Google Phone – $3.3M; 27″ 4K Gaming Monitor – $2.4M**.

**Volume leaders (Top-10 by quantity):**

- Accessories (AAA/AA batteries, USB-C & Lightning cables, wired headphones) dominate **units** but contribute **little revenue** per order.

**Momentum:**

- **Top product growth rate ≈ 46.1% MoM** (product-level), with **MacBook Pro** showing a dramatic **December spike** in the “Top-5 over time” view.

- **AOV by product (new, corrected):** MacBook Pro **$1,703**, ThinkPad **$1,001**, iPhone **$701**, Google Phone **$601**, high-value monitors/TVs in the **$300–$400** range.

**Key take:** Revenue is concentrated in **high-ticket devices**, while **accessories** are **attachment opportunities** rather than standalone revenue drivers.

**Clarification (bias check):** The **>$1,000 price band** revenue **($8.0M)** comes **exclusively** from the **MacBook Pro ($1,700)**—so comparisons by price band should treat this as a **single-product effect**, not a broad category behavior.

### 5.3 Time & Day Patterns
- **Peak hour:** **7 PM**; sustained high throughput **10 AM–9 PM**.

- **Week patterns:** Demand is **balanced** across days (slight mid-week edge Tue/Wed); **weekends ≈ 28.5%** of sales.
**Implication: Evening** is the prime window for **high-impact offers** and **retargeting**; weekdays are not meaningfully weaker than weekends.

### 5.4 Geographic Insights

- **Largest markets by revenue: San Francisco (~$8.3M), Los Angeles (~$5.5M), New York City (~$4.7M) → Top-3 share ≈ 53.3%.**
- **Fastest growth (latest MoM): Seattle (+53.6%), Dallas (+53%), New York (+51%), Portland (+46%), Boston (+45%).**
- **AOV by city:** Highest in **Atlanta (~$196), New York (~$196), Seattle (~$195)**; most major cities cluster **$191–$196** → pricing power fairly consistent, with a slight premium in high-income metros.

### 5.5 Price-Range Behavior (contextualized)

- **>$1,000** band = **$8.0M** (solely MacBook Pro).
- **$301–$700** bands together ≈ **$10.4M**, driven by smartphones and monitors.
- **<$300** = small revenue share, despite large **unit** volume (accessories).

## 6. Recommendations
**A.**  **Product Portfolio & Packaging**
1.	**Prioritize premium laptops & smartphones** (MacBook Pro, ThinkPad, iPhone) in 2020 planning—assortment depth, feature variants, and financing options.
2.	**Accessory Attach Strategy:**
    - Create **bundles** (laptop + monitor + cable + headphones) and **checkout add-ons** to monetize high volume SKUs.
    - Set **attach-rate** targets (e.g., +5–8% per premium device) and track in weekly dashboards.
3.	**Lift non-flagship phones/monitors** via **good-better-best** pricing ladders and **trade-in promos** near evening peaks.

**B. Time-Based Sales Activation**

4.	**“Prime-Time” campaigns 5–9 PM** (email/SMS retargeting, site banners, limited-time bundles) to exploit the **7 PM peak**.
5.	**Q4 Front-loading**: Start holiday build-up in **late October** (pre-order perks, financing), since Dec dominates.
6.	**Post-holiday recovery:** Counter the January slump with **accessory bundles** and **service add-ons** (warranty/AppleCare-like).

**C. Market & Geo Focus**

7.	**Double-down in top-revenue cities** (SF, LA, NYC) with premium device availability and local partnerships.
8.	**Ride the growth curve in Seattle & Dallas** (top MoM growth) with **timed promotions** and **inventory flex**; set city-level growth OKRs (e.g., **+10–12% QoQ**).
9.	**City-specific AOV nudges** (Atlanta/NY/Seattle show higher AOV): promote **higher-spec configurations** and **financing** in these metros.

**D. Measurement & Enablement**

10.	**KPI pack for 2020:**
    - Revenue by product & city; MoM growth; AOV; attach rate for accessories; evening-window conversion.
11.	**Experiments:** A/B evening promos vs. all-day; bundle vs. no-bundle; Seattle/Dallas lift tests.
12.	**Data enrichment:** Add **customer ID stitching** (enable **repeat rate, CLV**), and **traffic → conversion** tracking for more surgical decisions.

## 7. Caveats & Assumptions
- **Scope:** Single year **(2019)**; comparisons are **within-year** (MoM), not YoY.
- **Price band caveat:** The **>$1,000** band is **entirely MacBook Pro ($1,700)**—avoid generalizing that band to multiple products.
- **Cleaning:** Minimal record cleaning; derived columns & measures built in **DAX** (Month, Hour, City, AOV, MoM growth, price bands).
- **Missing metrics:** No direct fields for **site traffic, conversion rate, or repeat customers**—not reported to avoid unfounded claims.
- Data source: Public/online dataset (Kaggle)- Find the data here: [Sales Data Analysis](https://www.kaggle.com/datasets/beekiran/sales-data-analysis)

## 8. Next Steps
- Stand up a **city × product** weekly review with targets from the recommendations above.
- Implement **evening-window automation** and **bundle attach tracking** in the BI layer.
- Request engineering support for **customer identity** to unlock **repeat/retention** analysis and **CLV-based** prioritization.



