# Customer Feedback Satisfaction Analysis

## Project Overview
This project analyzes a customer feedback dataset using clustering techniques to segment customers based on their demographics and purchase behavior. The analysis aims to identify patterns in customer satisfaction and loyalty.

## Dataset Overview
The dataset consists of **38,444** customer records with the following features:

- **CustomerID**: Unique identifier for each customer  
- **Age**: Age of the customer  
- **Gender**: Male or Female  
- **Country**: Country of residence  
- **Income**: Annual income of the customer  
- **ProductQuality**: Rating of product quality (1-10)  
- **ServiceQuality**: Rating of service quality (1-10)  
- **PurchaseFrequency**: Number of purchases made  
- **FeedbackScore**: Customer feedback score (Low, Medium, High)  
- **LoyaltyLevel**: Customer loyalty level (Bronze, Silver, Gold)  
- **SatisfactionScore**: Overall satisfaction score (0-100)  

## Key Analysis & Methodology
1. **Data Cleaning & Preprocessing**  
   - Checked for missing values (None found).  
   - Encoded categorical variables (Gender, Country, FeedbackScore, LoyaltyLevel).  
   - Scaled numerical features using **StandardScaler**.  

2. **Exploratory Data Analysis (EDA)**  
   - Age, Income, and Satisfaction Score distributions were visualized using histograms.  
   - Gender and country distributions were analyzed using pie charts and count plots.  
   - Boxplots were used to detect outliers in **Income**.  

3. **Customer Segmentation using K-Means Clustering**  
   - Applied **Elbow Method** to determine the optimal number of clusters (**K=4**).  
   - Segmented customers based on **Age, Income, Product Quality, Service Quality, Purchase Frequency, Feedback Score, and Loyalty Level**.  
   - Assigned each customer to a cluster and visualized clusters using scatter plots.  

4. **Cluster Interpretation**  
   - **Cluster 0**: High purchase frequency, high satisfaction.  
   - **Cluster 1**: Moderate purchase frequency, low service quality rating.  
   - **Cluster 2**: Lower purchase frequency, average satisfaction.  
   - **Cluster 3**: High-income customers, very frequent purchases.  

5. **Demographic Breakdown**  
   - Analyzed age and income distribution within each cluster using boxplots.  
   - Examined gender and country distribution across clusters using count plots.  

## Results & Insights
- Customers with **higher purchase frequency and better service quality ratings** tend to have higher satisfaction scores.  
- Income does not directly impact satisfaction but correlates with purchase frequency.  
- Different clusters indicate distinct customer personas, helping businesses tailor marketing strategies.  

## Technologies Used
- **Python (Pandas, NumPy, Matplotlib, Seaborn, Scikit-Learn)**  
- **Machine Learning: K-Means Clustering**  
- **Data Visualization: Seaborn, Matplotlib**  

