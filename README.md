# Credit Card Customer Segmentation for Targeted Marketing Campaigns

![credit card segmentation](https://github.com/farisassallami/Credit-Card-Customer-Segmentation/assets/111199631/34a09563-586c-409b-a108-1a39c5d91a47)

Image Source: https://www.codersarts.com/post/credit-card-customer-segmentation-clustering-classification

## Business Problem
A credit card company aims to improve its marketing strategies by effectively segmenting its customer base. By leveraging Python and employing the Silhouette Score and Elbow Plot techniques, the company seeks to identify distinct groups within its customer population. This segmentation will enable the organization to tailor its marketing campaigns, develop personalized offers, and enhance customer satisfaction, ultimately leading to increased customer retention and revenue growth.

## Business Objectives:
1. Improve Marketing Strategies: Identify customer segments with similar behaviors, preferences, and characteristics to design targeted marketing campaigns and promotions.

2. Enhance Customer Satisfaction: Develop personalized offers and services based on each customer segment's needs and preferences, leading to higher customer satisfaction and engagement.

3. Optimize Resource Allocation: Allocate marketing resources efficiently by focusing efforts on the most profitable customer segments, resulting in cost savings and increased return on investment.

## Customer Segmentation & Profiling:
   - Utilize Python's clustering algorithm such as K-means to group customers based on their attributes.
   - Evaluate the quality of the clustering using the Silhouette Score, which measures the compactness and separation of the clusters.
   - Analyze the characteristics and behaviors of each customer segment.
   - Identify key attributes that differentiate the segments and provide actionable insights for targeted marketing campaigns.
## Expected Outcome:
The credit card company expects to gain valuable insights into its customer base by successfully segmenting customers using Python and employing the Silhouette Score and Elbow Plot techniques. This segmentation will empower the company to develop personalized marketing strategies, tailor product offerings, and allocate resources effectively. By targeting specific customer segments with relevant campaigns, the company aims to improve customer satisfaction, boost customer retention, and drive revenue growth.
   
### Elbow Plot Analysis:
   - Using the Elbow Plot technique to determine the optimal number of clusters for customer segmentation.
   - Applying the selected clustering algorithm for various cluster numbers and plot the corresponding sum of squared distances.
   - Identifying the elbow point where the rate of decrease in the sum of squared distances significantly diminishes.
   
![elbow plot](https://github.com/farisassallami/Credit-Card-Customer-Segmentation/assets/111199631/8fba13d4-c655-484f-b670-a55c4e42b295)

   -  The inertia plot does not have a very pronounced elbow at any number, but the graph seems to level off at 4 clusters. 4 would be one candidate for a good number of clusters.

### Silhouette Score Evaluation:
   - We will Calculate the Silhouette Score for each clustering solution.
   - We will Compare the scores to determine the clustering solution that maximizes the separation between clusters while maintaining their compactness.
   
![silhouette scores](https://github.com/farisassallami/Credit-Card-Customer-Segmentation/assets/111199631/40ead40b-02b0-4675-bae3-06a260d9add0)

   - The graph shows that 3 would be another candidate for a good number of clusters since it has the highest Silhouette Score.

### Fitting 2 different KMeans models (one with 3 clusters and one with 4 clusters) 

   - Displaying the silhouette scores will again confirm the best number of clusters.
   
   - Silhouette Score using 3 clusters: 0.29
   - Silhouette Score using 4 clusters: 0.24
   
   - 3 Clusters has the highest silhouette score


 ### Recommendations:

- Based on their debt, Cluster 0 customers are also good candidates for credit card offers. The offers should have moderate credit limits and moderate interest rates though, because Cluster 0 customers have no defaults despite their lower debts.  They have some long-term potential as a credit customer because they are young and new to the workforce--perhaps they will earn higher credit limits and lower interest rates as they demonstrate more successful money management skills.

- Based on their longer experience with employment, income, and money management, Cluster 1 customers are good candidates for credit card offers.  The offers should have high credit limits because they have significant income that they are willing to spend.  They should have lower interest rates because Cluster 1 customers know how to manage their debt.
  
- Cluster 2 customers were also young like cluster 0, but they were more educated.  In the future they will convert to cluster 1 customers.
