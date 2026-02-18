📦 Retail Supply Chain Analytics
End-to-End Omnichannel Inventory & Availability Case Study
1️⃣ Project Overview

The objective is to design an analytics foundation that supports operational decision-making across:

Store and e-commerce sales

Daily inventory positions

Inventory movements and replenishment

Cross-channel availability

The focus of this project is not static reporting — it is a decision infrastructure that helps teams move from reactive firefighting to disciplined, data-informed planning.

2️⃣ Business Context

Physical retail stores

Distribution centers

A growing e-commerce channel

As the company expanded into omnichannel fulfillment, operational complexity increased:

Inventory is shared across channels

Demand varies by location and season

Lead times fluctuate

Forecast errors compound over time

This created systemic supply chain issues, including:

Stockouts in some locations

Excess inventory in others

Reactive replenishment

Low trust in planning metrics

3️⃣ Core Business Problems
🔹 Stockouts & Availability Gaps

Inventory appears sufficient at the network level but fails at specific SKU-location combinations.

🔹 Excess Inventory

Slow-moving products tie up working capital and increase markdown risk.

🔹 Reactive Replenishment

Frequent emergency reallocations and inconsistent replenishment cadence.

🔹 Misaligned Metrics

Different teams interpret availability, efficiency, and service levels differently.

4️⃣ Project Objective

Design a clean analytical framework that:

Defines availability and inventory efficiency consistently

Connects sales behavior to stock positioning

Analyzes replenishment cadence and magnitude

Enables cross-channel performance comparison

Establishes trusted, reconciled metrics

5️⃣ Dataset Scope

Time horizon: 2026–2028

The dataset includes:

Store + online sales transactions

Daily inventory snapshots

Inventory movement events

Product and location reference data

6️⃣ Data Architecture

The project follows a structured layered approach:

Raw → Bronze → Silver → Dimensional Model

Bronze Tables

bronze__product_master__lite

bronze__location_master__lite

bronze__sales_transactions__lite

bronze__inventory_snapshots__lite

bronze__inventory_movements__lite

Silver Layer Goals

Standardize date/time formats

Clean and align keys

Reconcile movements with inventory changes

Prepare data for dimensional modeling

7️⃣ Analytical Framework

The project follows a structured logic:

Business Question → Required Data → Metric Design → Decision Support

8️⃣ Core Analytical Questions & KPIs
📌 Availability

Question: Where and when do we run low or out of stock?

Metrics include:

Daily on-hand inventory by SKU & location

Low-stock flags

Channel comparison (Store vs WEB vs DC)

📌 Sales Impact

Question: Which SKUs and locations drive the most volume and revenue proxy?

Metrics include:

Sales quantity

Revenue proxy (qty × unit_price)

Category & channel comparison

📌 Inventory Efficiency

Question: Which SKUs are overstocked vs fast-moving?

Metrics include:

Average on-hand inventory

Demand proxy (sales volume)

Identification of slow movers

📌 Replenishment Behavior

Question: How often and how much are we replenishing?

Metrics include:

Count of REPLENISH events

Replenishment frequency by SKU/location

Comparison of cadence vs stock levels

📌 Data Reconciliation / Sanity Checks

To ensure credibility:

Sales should reduce inventory directionally

Replenishments should increase inventory

Flag abnormal negative or extreme quantities

9️⃣ Dashboard Structure

The BI layer supports decision-oriented views:

Availability & Stock Health

Sales & Revenue Proxy Performance

Inventory Efficiency Analysis

Replenishment Monitoring

Cross-Channel Comparison

Each dashboard is tied to a specific operational decision.

🔟 Key Capabilities Demonstrated

This project demonstrates:

Operational systems thinking

Supply chain metric design

Dimensional modeling readiness

Event-stream and snapshot reconciliation

Cross-functional stakeholder alignment

Decision-oriented analytics

1️⃣1️⃣ Technical Stack

SQL (data cleaning & modeling)

Dimensional modeling (Kimball-style)

Bronze → Silver transformation logic

BI layer (Power BI or similar)

Time-series aggregation

Data validation & reconciliation logic

1️⃣2️⃣ What Makes This Project Strong

This project emphasizes:

✔ Trade-offs over isolated optimization
✔ Operational realism over theoretical modeling
✔ Data credibility before dashboarding
✔ Decision support over descriptive reporting
