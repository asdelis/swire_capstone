# IS 6813: Swire Capstone Project

**Group 5:**
Andrew Delis
Nidal Arain 
Joonas Tahvanainen
Kleyton Polzonoff



## Business problem and project objective

To streamline logistics operations, the client needs a structured approach for balancing its in‑house fleet of Red Trucks with alternative delivery methods (ARTM)—partner‑operated vehicles and third‑party White Trucks. Red Trucks strengthen customer relationships and drive revenue; ARTM offers flexibility, though with less direct oversight.

To ensure both high service standards and cost efficiency, we’ll implement precise fleet‑allocation guidelines informed by customer profiles, transaction history, geography, and delivery costs. This framework will leverage customer segmentation to group similar profiles, enabling smarter, data‑driven decisions.

By applying these insights, we’ll deliver actionable recommendations to optimize fleet distribution and boost overall operational performance.

## Analytics approach

We began with an open-ended exploration, since there was no predefined roadmap for achieving the project goals. A thorough EDA phase examined transaction trends, engineered new features, and profiled customers to inform our modeling strategy.

After transforming and aggregating the data into a modeling-ready format, we evaluated a range of methods—classification, regression, time‑series forecasting, and clustering. Ultimately, K‑means clustering emerged as the primary driver of our insights.

We applied clustering to segment customers into three groups, using engineered variables (including an RFM score that captures order recency, frequency, and volume) to define each segment’s characteristics.

Because clustering is unsupervised, we then trained decision trees and multinomial logistic regression models to “re-predict” cluster assignments. This secondary modeling wasn’t intended for production use, but to identify the key features that distinguish each customer segment.

## Solution and business value

Our framework is transparent, replicable, and easy to follow—offering clear visibility into the fleet‑allocation decision process.

By strategically reallocating resources, the company could have saved approximately \$770,000 over the past two years. These savings stem from expanding Red Truck coverage for high‑value customers, optimizing delivery frequency, and reducing overall volume by 3%. This shift enables more efficient asset deployment and ensures key customers receive prioritized service—precisely what the client sought.

We applied this restructuring to just 14% of customers, aligning fleet assignments with shipment profiles and customer attributes to balance efficiency and quality. Post‑implementation, we expect not only continued cost savings but also increased sales, especially among high‑growth accounts.  

## Challenges and opportunities

A key challenge was the limited two-year historical window, which constrained our ability to evaluate long-term impacts. Wide probability ranges further complicated outcome predictions.

Customer order patterns were highly inconsistent, making it difficult to link growth to specific periods. Access to a longer dataset would improve forecast accuracy and actionability.

Integrating census data showed promise but underdelivered in this analysis. With refined methods and more extensive history, it could yield deeper insights in future projects.

Forecasting remains complex—even with solid data. Predictions should be presented only when backed by rigorous statistical models and clear confidence intervals; otherwise, it’s better to avoid overreaching conclusions.

Looking ahead, additional testing of fleet-distribution strategies and customer-order behaviors will be crucial for fine-tuning our approach. A more detailed revenue analysis—examining profit margins by customer segment—could further strengthen decision-making. 
