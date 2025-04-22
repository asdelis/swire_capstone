# IS 6813: Swire Capstone Project

**Group 5:**
Andrew Delis
Nidal Arain 
Joonas Tahvanainen
Kleyton Polzonoff



## Project Overview
This project was conducted in collaboration with Swire Coca-Cola as part of the MSBA Capstone at the University of Utah. The goal was to optimize delivery operations by identifying which customers could be transitioned from Swire’s proprietary red truck fleet to third-party white truck delivery — without compromising future growth potential or customer satisfaction.

---

## Business Problem
Swire faces high delivery costs serving low-volume customers with its own fleet. While transitioning these customers to white truck (third-party) delivery could save costs, it also risks alienating customers with future growth potential. The challenge was to segment customers in a way that balances cost-efficiency with long-term value.

---

## Analytics approach

### Business Understanding
- Defined core objective: reduce logistics costs without sacrificing high-potential customers.
- Outlined customer types: local market partners, high-frequency buyers, and emerging accounts.

### EDA & Feature Engineering
- Created behavioral features using the **RFM (Recency, Frequency, Monetary)** framework.
- Enriched customer profiles using **public census data** (e.g., income, population).
- Visualized volume trends and delivery cost patterns by segment and region.

### Modeling & Segmentation
- Applied **PCA + K-Means clustering** to segment customers into meaningful profiles.
- Built a **Random Forest model** to validate clusters and extract feature importance.
- Developed an **ARIMA model** to forecast volume growth by Cold Drink Channel.
- Created a **Growth Potential Score** based on economic, volume, and frequency signals.

### Fleet Assignment Logic
Developed decision rules based on cluster, volume, and growth attributes:
- High-volume customers (>1,349 gallons/year) assigned to **Red Trucks**
- Low-demand customers and Cluster 3 assigned to **White Trucks**
- Cluster 2 split based on growth indicators and frequency

---

## Solution and business value

 **Cost Efficiency:** Confidently reroute true low-volume customers to reduce delivery expenses.  
 **Customer Retention:** Preserve high-touch service for promising accounts with strong growth signals.  
 **Scalable Framework:** Fleet assignments now follow clear business rules and scoring logic — ready to scale across markets.  
 **Strategic Insights:** Provided a deeper understanding of customer profiles based on behavioral and economic patterns.

Our framework is also transparent, replicable, and easy to follow—offering clear visibility into the fleet‑allocation decision process.

By strategically reallocating resources, the company could have saved approximately \$770,000 over the past two years. These savings stem from expanding Red Truck coverage for high‑value customers, optimizing delivery frequency, and reducing overall volume by 3%. This shift enables more efficient asset deployment and ensures key customers receive prioritized service—precisely what the client sought.

We applied this restructuring to just 14% of customers, aligning fleet assignments with shipment profiles and customer attributes to balance efficiency and quality. Post‑implementation, we expect not only continued cost savings but also increased sales, especially among high‑growth accounts.  

## Challenges and Opportunities

A key challenge was the limited two-year historical window, which constrained our ability to evaluate long-term impacts. Wide probability ranges further complicated outcome predictions.

Customer order patterns were highly inconsistent, making it difficult to link growth to specific periods. Access to a longer dataset would improve forecast accuracy and actionability.

Integrating census data showed promise but underdelivered in this analysis. With refined methods and more extensive history, it could yield deeper insights in future projects.

Forecasting remains complex—even with solid data. Predictions should be presented only when backed by rigorous statistical models and clear confidence intervals; otherwise, it’s better to avoid overreaching conclusions.

Looking ahead, additional testing of fleet-distribution strategies and customer-order behaviors will be crucial for fine-tuning our approach. A more detailed revenue analysis—examining profit margins by customer segment—could further strengthen decision-making. 

---

## Repo Contents

| Folder | Description |
|--------|-------------|
| `business_problem_statement/` | Overview of the project objectives and sponsor goals |
| `eda/` | Exploratory Data Analysis and feature generation |
| `modeling/` | Modeling scripts for clustering, random forest, and growth scoring |
| `presentation/` | Final group presentation slides (PDF format) |
| `README.md` | This file — summary of our group project and value delivered |

---

Thanks to Swire Coca-Cola and our faculty advisors for the opportunity to work on this impactful project!
