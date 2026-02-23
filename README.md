Customer Segmentation Using K-Means Clustering
* Overview

  This project implements customer segmentation on the Online Retail II dataset using K-means clustering. The objective is to identify meaningful customer groups based on purchasing behaviour. The implementation follows the Week 5 core requirements, including feature engineering, scaling, clustering, and cluster evaluation.

* Dataset

  The dataset contains transactional retail data including invoices, quantities, prices, customer identifiers, and dates. The unit of analysis was defined at the customer level, where transactional records were aggregated to construct behavioural features.

Feature Engineering

  The following customer-level features were constructed:

 * TotalSpend – Total monetary value of purchases

 * TotalTransactions – Number of invoices

 * TotalQuantity – Total units purchased

 * AvgBasketValue – Average spend per transaction

 * DistinctProducts – Unique products purchased

 * Recency – Days since last purchase

 * CustomerLifespan – Duration between first and last purchase

  These features capture spending intensity, engagement, and purchasing diversity.

Data Preprocessing

 * Negative or return-related transactions were handled appropriately.

 * Data was aggregated at the customer level.

 * All numerical features were standardised using feature scaling.

 * Scaling was necessary to ensure equal contribution in Euclidean distance computation.

Clustering Approach

 * K-means clustering was applied to the scaled feature set.

  Selection of k

  * The Elbow Method was used to analyse inertia values.

  * The elbow point suggested k = 4 as a balanced choice.

  * The Silhouette Score (0.3906) indicated moderate separation and cohesion.

Cluster Evaluation

  * Cluster sizes were examined to assess distribution balance.

  * Cluster centres were interpreted on the original scale.

  * PCA projection was used to visualise cluster separation.

  * Segments were distinguished based on spend, transaction frequency, recency, and product diversity.

Key Outputs

  * Elbow plot for optimal k selection

  * Silhouette score evaluation

  * Cluster size distribution

  * Cluster profile summary table

  * PCA cluster visualisation

Conclusion

  The implementation produces structured customer segmentation with interpretable behavioural patterns. The clustering solution is supported by quantitative validation and visual inspection, meeting the Week 5 analytical requirements.
