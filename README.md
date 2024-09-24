# Customer Purchase Behavior - Electronic Sales Data Analysis

## Project Overview
This project focuses on analyzing customer purchase behavior using a dataset of electronic sales. The aim is to apply various machine learning techniques to gain insights, predict customer actions, and optimize business decisions. The dataset contains key information such as customer demographics, product types, pricing, and order status, making it ideal for different predictive and exploratory tasks.

## Dataset
The dataset used in this project is titled **Customer Purchase Behavior - Electronic Sales Data** and contains the following columns:

- Customer ID: Unique identifier for each customer
- Age: Age of the customer
- Gender: Gender of the customer
- Loyalty Member: Indicates whether the customer is part of the loyalty program
- Product Type: Type or category of the purchased product
- SKU: Unique identifier for the product
- Rating: Product rating provided by the customer
- Order Status: Status of the order (e.g., Completed, Cancelled)
- Payment Method: Payment method chosen by the customer
- Total Price: Total amount paid for the purchase
- Unit Price: Price per unit of the product
- Quantity: Number of products purchased
- Purchase Date: Date of purchase
- Shipping Type: Type of shipping used (e.g., Standard, Expedited)
- Add-ons Purchased: Number of add-ons bought with the product
- Add-on Total: Total price for the add-ons

## Machine Learning Problems Tackled

### Customer Segmentation (Clustering)
**Goal**: Group customers based on their demographics and purchasing behavior to create targeted marketing strategies.  
**Algorithm**: K-Means Clustering  
**Key Features**: Age, Gender, Loyalty Member, Total Price, Quantity, Add-ons Purchased  
**Output**: Creation of customer segments for personalized marketing strategies.

### Customer Churn Prediction (Classification)
**Goal**: Predict whether a customer is likely to stop purchasing (churn) based on their purchase history.  
**Algorithm**: Random Forest Classifier  
**Key Features**: Age, Gender, Loyalty Member, Total Price, Quantity, Order Status  
**Target**: Churn (inferred from Order Status - "Cancelled" = 1, "Completed" = 0)  
**Output**: Predicting the likelihood of churn for each customer.

### Price Prediction (Regression)
**Goal**: Predict the total price a customer will spend based on various product and customer features.  
**Algorithm**: Linear Regression  
**Key Features**: Age, Gender, Loyalty Member, Quantity, Product Type, Add-ons Purchased  
**Output**: Prediction of Total Price for a customer’s purchase.

### Product Recommendation (Association Rule Mining)
**Goal**: Recommend products to customers based on their previous purchase history.  
**Algorithm**: Apriori Algorithm  
**Key Features**: Customer ID, SKU (product codes)  
**Output**: Product recommendations based on frequently purchased items.

### Demand Forecasting (Time Series Prediction)
**Goal**: Forecast future demand for products based on historical sales data.  
**Algorithm**: ARIMA (AutoRegressive Integrated Moving Average)  
**Key Features**: Aggregated Quantity over Purchase Date  
**Output**: Prediction of sales quantities for future dates.

### Payment Method Prediction (Classification)
**Goal**: Predict the payment method a customer will use based on their purchase behavior and demographics.  
**Algorithm**: Random Forest Classifier  
**Key Features**: Age, Gender, Loyalty Member, Total Price, Quantity  
**Target**: Payment Method  
**Output**: Prediction of the Payment Method for future purchases.

## Tools and Libraries Used
- **Pandas**: For data manipulation and analysis.
- **NumPy**: For numerical computations.
- **Scikit-learn**: For machine learning models, including clustering, classification, and regression.
- **mlxtend**: For association rule mining (Apriori algorithm).
- **Statsmodels**: For time series forecasting (ARIMA model).
- **Matplotlib/Seaborn**: For data visualization.
- **StandardScaler/OneHotEncoder**: For data preprocessing.
