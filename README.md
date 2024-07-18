# Retail_Analysis_Walmart

# Table of Contents
1. Problem Statement
2. Project Objective
3. Data Description
4. Data Pre-processing Steps and Inspiration
5. Choosing the Algorithm for the Project
6. Motivation and Reasons For Choosing the Algorithm
7. Assumptions
8. Model Evaluation and Techniques
9. Inferences from the Same
10. Future Possibilities of the Project
11. Conclusion

# Problem Statement
A retail store with multiple outlets across the country faces issues in managing inventory to match the demand with supply. As a data scientist, you are tasked with deriving useful insights from the data and developing predictive models to forecast sales for the next X number of months/years.

# Project Objective
The objective of this project is twofold:
1. To derive actionable insights from the provided dataset that can help each store improve various operational areas.
2. To build a predictive model to forecast sales for each store for the next 12 weeks.

# Data Description
The dataset consists of 6435 rows and 8 columns, with the following features:
• Store: Store number
• Date: Week of Sales
• Weekly_Sales: Sales for the given store in that week
• Holiday_Flag: Indicates if it is a holiday week
• Temperature: Temperature on the day of the sale
• Fuel_Price: Cost of fuel in the region
• CPI: Consumer Price Index
• Unemployment: Unemployment Rate

# Data Pre-processing Steps and Inspiration
Data pre-processing involved the following steps:
• Handling Missing Values: Checked for missing values and ensured data completeness.
• Feature Engineering: Created additional features if necessary for better model performance.
• Normalization: Applied normalization to scale the features appropriately.
• Date Parsing: Converted the Date column to a datetime format for time series analysis.
• Outlier Detection and Removal: Identified and handled outliers in the sales data to improve model accuracy.

# Choosing the Algorithm for the Project
• We chose the Prophet algorithm for time series forecasting.

# Motivation and Reasons For Choosing the Algorithm
• Accuracy: Prophet is known for its high accuracy in time series forecasting.
• Handling Seasonal Effects: It effectively handles daily, weekly, and yearly seasonality.
• Flexibility: It can model missing data and large outliers, making it robust for retail sales data.

# Assumptions
• The sales data follows a seasonal pattern influenced by holidays, temperature, fuel price, CPI, and unemployment rate.
• The data provided is representative of future trends and patterns.
• No significant external factors will drastically alter the sales trends during the forecast period.

# Model Evaluation and Techniques
• Train-Test Split: The data was split into training and testing sets.
• Evaluation Metrics: Metrics like Mean Absolute Error (MAE) and Root Mean Squared Error (RMSE) were used to evaluate the model.
• Cross-Validation: Time series cross-validation was employed to ensure robustness.

# Inferences from the Same
• Store-wise Analysis: Identified stores with the highest and lowest sales.
• Seasonal Trends: Observed seasonal trends affecting sales.
• Holiday Impact: Assessed the impact of holidays on sales.

# Future Possibilities of the Project
• Enhancing Feature Set: Incorporate more external factors like promotional events and competitor pricing.
• Real-time Forecasting: Implement real-time sales forecasting for dynamic inventory management.
• Advanced Models: Explore advanced machine learning models for improved accuracy.

# Conclusion
• There is seasonal component in sales through holiday date, so the management have to taking into account the seasonal to stocking, merchandising, marketing etc. decision.
• Although Thanksgiving Holiday in November contributed more sales than other holiday, it seems that December has higher growth sales happening before Christmas.
• Store 20 indeed has a high sales volume for 3 years. However, it's growth has been dominated by holiday date.
