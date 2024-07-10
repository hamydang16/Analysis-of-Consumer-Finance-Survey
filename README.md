
# Analysis of Consumer Finance Survey
One of the residual effect of COVID-19 pandemic is the surge in the number of investors as technology makes it much easier to participate in the financial market. For many funds managers, it would probably be helpful to build a profile of possible clients based on the the ability to take risks as well as other helpful attributes.
This portfolio will attempt to focus on business owners in the US, since this segment of the population is more prone to external shocks, instead of the whole population with the help of **K-Means and Hierarchical Clustering**.

## Proposal

<div class="alert alert-block alert-info">
<ol>
  <li> How can we cluster business owners in the US to better identify different types of investors?</li>
  <li> What are the influential attributes in determining the clusters?
</li>

</div>


## Process

- Data source and processing
- Exploratory Data Analysis
- Feature selection
- Build K-Means and Agglomerative Hierarchical Clustering Model
- Cluster insight



## Data source

The Survey of Consumer Finance (SCF), which is sponsored by the US Federal Reserve, tracks balance sheets, pensions, income and demographical information about families in the US. The ***public extract file for 2022*** is used for this project. 

This is a large dataset with almost 25,000 rows and 357 columns. At the same time, some index can be quite difficult to decipher and read. This [Codebook](https://sda.berkeley.edu/sdaweb/docs/scfcomb2022/DOC/hcbkfx0.htm) contains explanations for all the features. 

The data can be found at this [page](https://www.federalreserve.gov/econres/scfindex.htm)


## Screenshots
![image](https://github.com/MQ-COMP2200-COMP6200/portfolio-part-4-hamydang/assets/160813113/7fc0c2ee-f1b0-41c4-9874-be07b1c5bfb3)

## Cluster insight

#### Question 1: How can we cluster business owners in the US to better identify different types of investors?
Using KMeans as a starting point and then refining through Agglomerative Hierarchical Clustering, we are able to identify 5 clusters with characteristics as detailed in the table below.

![image](https://github.com/MQ-COMP2200-COMP6200/portfolio-part-4-hamydang/assets/160813113/5b562f6c-e5de-41c9-9083-8fe20ceac0b1)

#### Question 2: What are the influential attributes in determining the clusters?
By making use of Principal Component Analysis, we were able to extract the most influential financial features such as **asset, capital gains, debt and value of houses**.


## Lessons Learned
- Build unsupervised learning models: K-Means and Agglomerative Hierarchical Clustering
- Finding optimal number of K with the Elbow Method, Silhouette Score, and Dendrogram
- Perform Principal Component Analysis to reduce dimensionality
- Cluster insight
