# Retail Store & Product Clustering Analysis

# Business Problem
Retailers often struggle to understand why some stores perform better than others and which products drive sales.
Challenges include unpredictable demand, products that only sell when discounted, and stores with overlapping strategies.

# Proposed Solution
Applied unsupervised learning (K‑Means + PCA) to cluster both stores and products.
This revealed performance patterns and provided actionable strategies for pricing, promotions, and assortment optimization.

# Key Features
-> Demand Volatility: Measures how unpredictable sales are. High volatility = risky to stock, low volatility = stable demand.  

-> Product Responsiveness: Shows how much sales increase during promotions. High responsiveness = good for campaigns, low responsiveness = steady sellers.

-> Product Diversity Index: Counts how many unique products a store sells. High diversity = wide assortment, low diversity = focused assortment.

# Data
-> Retail dataset with store IDs, product SKUs, sales, prices, and discounts.

-> Aggregated at store and product levels to create meaningful features.

-> Cleaned and standardized for clustering.

# Model
-> Feature engineering: volatility, responsiveness, diversity.

-> Scaling and PCA for dimensionality reduction.

-> K‑Means clustering applied separately to stores and products.

-> Evaluation using Silhouette Score and Davies–Bouldin Index.

# Results
## Store Clusters

Cluster 0 – Top‑Performing Stores: High sales, moderate discounts, strong demand.

Cluster 1 – Low‑Activity Stores: Low sales, low discounts, weak engagement.

Cluster 2 – Balanced Stores: Average sales and discounts, stable but improvable.

Insight: Stores are more similar to each other, so differences mainly come from the products they stock.

## Product Clusters

Cluster 0 – Core Products: Steady sellers, low discounts, reliable demand.

Cluster 1 – Popular Products: High sales, moderate discounts, strong performers.

Cluster 2 – Promo‑Dependent Products: Expensive items that rely on discounts.

Cluster 3 – Slow Movers: Average pricing, weak demand.

Cluster 4 – Premium Products: High price, low sales, niche appeal.

Cluster 5 – Budget Products: Low price, high sales, strong volume drivers.

Insight: Products vary much more than stores. Cluster 5 drives volume, Cluster 2 depends on promotions, Cluster 4 underperforms.

# How Low‑Performing Stores and Products Can Increase Sales

## Stores

### Cluster 1 (Low‑Activity Stores) can improve by:

-> Introducing more budget and popular products (Clusters 1 & 5).

-> Running targeted promotions to attract customers.

-> Expanding product diversity to appeal to wider customer needs.


## Products

### Cluster 3 (Slow Movers) can improve by:

-> Bundling with popular products to increase visibility.

-> Offering small discounts to stimulate demand.


### Cluster 4 (Premium Products) can improve by:

-> Repositioning as niche or luxury items with targeted marketing.

-> Reducing price slightly or offering loyalty rewards.


### Cluster 2 (Promo‑Dependent Products) can improve by:

-> Using promotions strategically during peak seasons.

-> Adjusting base prices to reduce reliance on heavy discounts.

# Combined Insights

-> Products explain most store differences.

-> High‑performing stores stock popular and budget products.

-> Low‑activity stores often carry slow or niche products.

-> Promo‑dependent products can be used strategically in balanced stores.

# Installation

bash

git clone https://github.com/anu-006/Retail_Store_and_Product_Clustering.git

pip install -r requirements.txt

# Usage
This project can be applied in:

-> Retail strategy: Identify which stores need support and which products drive sales.

-> Marketing campaigns: Target promo‑sensitive products for discounts.

-> Inventory planning: Stock stable products more confidently, review niche products.

-> Assortment optimization: Match store clusters with product clusters to design smarter pricing and product mixes
