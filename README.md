# E-Commerce Customer Behavior & Segmentation 🛒

## 📌 Executive Summary
This project segments an e-commerce customer base into behavior-driven groups, enabling the business to pivot from "one-size-fits-all" marketing to highly targeted retention and upsell strategies. By analyzing transaction, engagement, and satisfaction signals across 350 customer records, this pipeline identifies distinct lifetime value (LTV) and churn-risk profiles that directly inform pricing, loyalty programs, and reactivation decisions.

## 🎯 Key Business Insights & Strategies
Through unsupervised learning, the customer base was segmented into 5 distinct cohorts. The top strategic priorities include:

1. **Protecting the High-Value Loyal Segment:** Identified a premium cohort with high average spend (~1455), high item volume, and high recent activity (~11.3 days since purchase). 
   * *Strategy: Premium loyalty tiers and cross-sell bundles.*
2. **Reactivating the Churn-Risk Segment:** Isolated a group with the longest inactivity (~51.1 days) and poor satisfaction tendencies. 
   * *Strategy: Win-back campaigns, personalized reminders, and service recovery offers.*
3. **Upgrading Mid-Tier Segments:** Highlighted clusters with moderate-to-high ratings and steady purchase frequency (spend ~775 to ~1164). 
   * *Strategy: Tiered membership perks, threshold discounts, and targeted recommendations to move them upward.*

## 🛠️ Technical Implementation
* **Data Engineering:** Pandas-based cleaning, handling missing values, Label/One-Hot encoding, and standardizing features (`StandardScaler`).
* **Unsupervised Clustering:** `K-Means` clustering (optimized to $k=5$ via the Elbow method). Evaluated cluster quality using a Silhouette Score of ~0.488.
* **Benchmarking & Visualization:** Validated the approach using `DBSCAN` as an alternative clustering method, and implemented `PCA` (2 components) for 2D cluster visualization.
* **Tech Stack:** Python, `scikit-learn`, `pandas`, SQL-style group aggregations.

---
*Developed by [Kinshuk Gupta](https://www.linkedin.com/in/kinshukgupta18/) | B.Tech in Data Science & AI, IIT Bhilai*
