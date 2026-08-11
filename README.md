# Thiranex-Task-2-Customer-Segmentation
Customer segmentation analysis using K-Means clustering and Power BI to identify customer groups based on demographics and spending behavior
# Customer Segmentation Analysis

## Project Overview

This project was completed as part of my **Data Analytics Virtual Internship at Thiranex**.

The goal of this project is to segment customers based on their demographic characteristics and spending behavior using **K-Means clustering**. The resulting customer segments were analyzed and visualized through an interactive **Power BI dashboard**.

## Objective

- Analyze customer demographic and spending data
- Identify groups of similar customers
- Apply K-Means clustering for customer segmentation
- Understand the characteristics of each customer segment
- Create an interactive Power BI dashboard
- Generate business insights for targeted customer strategies

## Dataset

The dataset contains **1,000 customer records** with the following attributes:

| Column | Description |
|---|---|
| CustomerID | Unique customer identifier |
| Gender | Customer gender |
| Age | Customer age |
| Annual Income (k$) | Annual income in thousands of USD |
| Spending Score (1-100) | Customer spending behavior score |

## Tools & Technologies

- **Python**
- **Pandas**
- **NumPy**
- **Scikit-learn**
- **Matplotlib**
- **Seaborn**
- **Power BI**
- **Jupyter Notebook / Google Colab**

## Methodology

### 1. Data Cleaning

The dataset was inspected for missing values and data quality issues.

Missing numerical values were handled using the median, while missing gender values were filled using the most frequent gender.

### 2. Exploratory Data Analysis

Exploratory analysis was performed to understand:

- Customer age distribution
- Annual income distribution
- Spending score distribution
- Gender distribution
- Relationships between income, age, and spending behavior

### 3. Feature Selection

The following numerical features were selected for clustering:

- Age
- Annual Income (k$)
- Spending Score (1-100)

`CustomerID` was not used for clustering because it is only an identifier.

`Gender` was retained for analyzing the characteristics of the resulting segments.

### 4. Data Standardization

The selected numerical features were standardized using `StandardScaler` so that variables with different ranges could be compared fairly during clustering.

### 5. K-Means Clustering

The **Elbow Method** was used to determine an appropriate number of clusters.

Based on the analysis, **4 clusters** were selected.

K-Means clustering was then applied to group customers with similar characteristics.

## Customer Segments

Four customer segments were identified:

| Customer Segment | Customers | Avg Age | Avg Income (k$) | Avg Spending Score |
|---|---:|---:|---:|---:|
| Moderate Customers | 333 | 35.55 | 49.42 | 47.68 |
| Young Active Spenders | 327 | 27.44 | 29.61 | 60.32 |
| Affluent Low-Engagement | 212 | 45.14 | 81.16 | 30.34 |
| High-Income Low-Spending | 128 | 66.70 | 107.58 | 4.98 |

## Key Insights

### Young Active Spenders

This segment contains younger customers with relatively low income but higher spending scores. Affordable products, promotional offers, and digital marketing campaigns could be effective for this group.

### Moderate Customers

This is the largest segment with 333 customers. These customers have moderate income and spending levels. Loyalty programs and regular promotions could help increase their engagement.

### Affluent Low-Engagement

These customers have relatively high income but lower spending scores. Personalized recommendations and premium offers could help improve their engagement.

### High-Income Low-Spending

This segment has the highest average income but the lowest spending score. It represents an important opportunity for targeted marketing and personalized offers.

## Power BI Dashboard

An interactive Power BI dashboard was created to visualize the customer segments and their characteristics.

The dashboard includes:

- Total Customers
- Average Age
- Average Annual Income
- Average Spending Score
- Customers by Segment
- Average Spending by Segment
- Average Income by Segment
- Age vs Spending Score
- Income vs Spending Score
- Gender Distribution by Segment
- Customer Segment slicer
- Gender slicer

## Project Files

| File | Description |
|---|---|
| `Thiranex_Task2_Customer_Segmentation.ipynb` | Python analysis and K-Means clustering |
| `Thiranex_Task2_Customer_Segmentation.pbix` | Power BI interactive dashboard |
| `customer_segmentation_final.csv` | Final dataset with cluster and segment labels |
| `README.md` | Project documentation |

## Conclusion

This project demonstrates how customer data can be analyzed using **K-Means clustering** to identify meaningful customer groups.

The combination of **Python for data analysis and clustering** and **Power BI for interactive visualization** helped transform customer data into actionable business insights.

The analysis can support targeted marketing, personalized offers, customer engagement strategies, and better understanding of customer behavior.

## Internship

**Data Analytics Virtual Internship - Thiranex**

**Task 2: Customer Segmentation Project**
