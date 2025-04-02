 <H1> CreditCard_Customer_segmentation
 </H1>
 <p> The Credit Card Customer Segmentation project is an analysis and segmentation of credit card customers <br>
 (Customer Segmentation) using Machine Learning (Clustering) to enable banks or card issuers to understand customer behavior and use it for business purposes.</p>

<H2>Dataset</H2>
<p> import dataset from Kaggle. We can dowload dataset from  <br>
  this link : https://www.kaggle.com/datasets/rupindersinghrana/credit-card-customer-segmentation </p>

<H2> Problem statement </H2>
<p> Credit card issuers and banks have a large customer base, each with their own unique card usage behaviors. Some people use high limits and pay in full every month. Others have riskier behaviors, such as being late on payments or not using their cards at all. Banks need an effective way to segment their customers by credit rating.</p>

<H2> Step  </H2>
<H3> Data Preprocessing </H3>
<p> - Loaded the dataset and performed an initial inspection. <br>
    - Read the dataset using pandas. <br>
    - Check data structure (df.info(), df.describe())  <br> 
    - Check for missing values ​​(df.isnull().sum()). 
</p>
<H3> Statistical Summary </H3>
<p> - Generate summary statistics using df.describe() to check mean, min, max, and quartiles. <br>
    - Look for anomalies in numeric variables
</p>
<H3> Outlier Detection </H3>
<p> - Detected and removed outliers in features using the IQR method (Interquartile Range).<br>
    - Calculated the IQR for each feature. <br>
    - Defined outliers as values below the lower bound or above the upper bound of the IQR. <br>
    - Removed rows with outliers to ensure cleaner data for model training.</p>

<H3>  Using K-Means Clustering </H3>
<p> - Use the Elbow Method to check the Optimal Number of Clusters <br>
    - Use KMeans to group customers based on their credit card usage behavior </p>
<H3>  Final Result </H3>
<p> - This visualization represents customer segmentation using K-Means Clustering, categorizing credit card users into two main groups based on Avg_Credit_Limit (Average Credit Limit) and Total_Credit_Cards (Total Number of Credit Cards Owned). <br>
  - In the final result, High Credit Users (Blue) have a high number of credit cards (around 4-7) and have a high average credit limit (ranging from ~20,000 to 100,000+). Therefore ,Likely to be experienced users with strong financial capacity. <br>       
    Low Credit Users (Green) have fewer credit cards (around 1-4) and have a lower average credit limit (mostly between 0-20,000). So, Could be new customers or those who use credit cards less frequently.  <br>
  - In conclusion , Customers with more credit cards generally have higher credit limits while Customers with fewer credit cards typically have lower credit limits.
</p>
