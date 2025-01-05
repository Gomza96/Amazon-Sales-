# Amazon-Sales- Analysis with python
## Introduction

Amazon handles a vast array of products and customers, and this project aims to analyze the sales data to:
- Identify top-performing products and regions.
- Understand sales trends over time.
- Optimize inventory based on size and regional preferences.
- Improve fulfillment and delivery processes.

---

## Dataset Description

The dataset contains the following columns:

- **Product Information**: Categories, prices, shipment details.
- **Sales Data**: Total sales, quantity sold, and transaction details.
- **Customer Insights**: Region and demographics.
- **Temporal Data**: Sales trends over time (daily, monthly).

---

## Methodology

### Data Cleaning
- Removed unnecessary columns like `New`, `PendingS`, and `Fulfilled-by`.
- Handled missing values (e.g., dropped rows with missing `Currency` and `Amount`).
- Converted `Date` to datetime format and postal codes to integers.
- Removed duplicate records and standardized column names.

### Feature Engineering
- Extracted the `Month` from the `Date` to analyze time-based patterns.

### Summary Statistics
- Displayed basic statistics for numerical columns like `Price`, `Quantity`, and `Total Sales`.

### Grouping and Aggregation
- Grouped data by categories (e.g., product category, region) to uncover trends.

### Data Visualizations
- Used `Matplotlib` and `Seaborn` to visualize sales trends, product popularity, and regional performance.

---

## Key Insights

1. **Top-Selling Products**:
   - **T-shirts**: 47,000 units sold, generating ₹40 million in sales.
   - **Shirts**: 46,000 units sold, generating ₹20 million in sales.
   - **Shoes and Watches**: Lowest-performing categories.

2. **Order Fulfillment**:
   - **90%** of orders shipped successfully.
   - **6%** remain unshipped, and **4%** are still in transit.

3. **Regional Insights**:
   - Maharashtra and Karnataka are the top-performing states.

4. **Size Preferences**:
   - Heatmap analysis revealed the most popular sizes for different products.

---

## Visualizations

### Key Visuals:
1. **Bar Chart**: Top-selling products.
2. **Stacked Bar Graph**: Sales across the top 5 states.
3. **Heatmap**: Popular product sizes by sales.
4. **Line Graph**: Sales trends over time.

---

## Technologies Used

- **Python**: Data analysis and visualization.
- **Pandas**: Data wrangling.
- **Seaborn & Matplotlib**: Data visualization.


---

## Future Work

1. **Prediction Models**:
   - Use machine learning (e.g., Random Forest) to predict sales based on region, size, and product category.
2. **Clustering**:
   - Implement clustering techniques to group products or regions based on sales patterns.
3. **Recommendation System**:
   - Suggest optimal inventory strategies for underperforming regions or categories.
