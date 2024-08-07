# BCG-Data-Science-Virtual-Internship--Churn-Analysis
Project: PowerCo Customer Churn Prediction
Objective:

To build a predictive model to identify customers at risk of churning and analyze the impact of price sensitivity on churn behavior. This project aims to help PowerCo understand the underlying factors driving customer churn and develop targeted retention strategies.

Business Context:

PowerCo, a major gas and electricity utility serving small and medium-sized enterprises, is experiencing increasing customer churn due to heightened competition in the energy market. The company seeks to understand the reasons behind customer attrition, with a particular focus on the impact of pricing on churn decisions.

Hypothesis:
Is price sensitivity a major factor for churning of customers ? 
Data
The project utilizes two main datasets:

client_data.csv: Contains information about PowerCo's customers, including their energy consumption, contract details, and churn status.
price_data.csv: Contains pricing information related to energy consumption.

EDA
In the EDA section, I performed various analyses to understand the distribution and relationship of different features with customer churn. I visualized the data using stacked bar plots and distribution plots for various features such as energy consumption, contract types, sales channels, and forecasted values.

Feature Engineering
Key Features
Duration Features: Calculated the duration in months for various contract-related dates such as activation date, end date, product modification date, and renewal date.
Price Volatility Metrics: Calculated price volatility metrics from the price_data.csv and added them to the main DataFrame.
Categorical Encoding: Transformed categorical features such as channel_sales and origin_up using one-hot encoding.
Boolean Encoding: Converted boolean features such as has_gas to binary flags.
Correlation Analysis
Performed correlation analysis to identify highly correlated features and reduce multicollinearity.

Random Forest Classifier
A Random Forest classifier was chosen for its robustness and ability to handle large datasets with higher dimensionality. The steps included:

Data Preprocessing: Handled missing values, normalized features, and split the data into training and testing sets.
Model Training: Trained the Random Forest model on the training set.
Model Evaluation: Evaluated the model's performance using metrics such as accuracy, precision, recall, and F1 score.

The Random Forest model provided insights into the key factors influencing customer churn. The following are some key findings:

Feature Importance: Identified the most important features contributing to churn prediction.
Model Performance: Achieved an accuracy of 90%, with precision and recall values indicating the model's reliability.

Key Business Insights
High Power Consumption: Customers with higher maximum power consumption tend to churn at a higher rate. Implementing targeted engagement strategies for these customers can help reduce churn.
Gas Contracts: Customers with gas contracts show slightly higher retention. Bundling gas with electricity services could improve overall retention rates.
Customer Tenure: Enhancing onboarding processes and implementing effective loyalty programs for new customers is crucial, as early customer experiences strongly correlate with long-term retention.
Sales Channels: Optimizing sales strategies and focusing on more effective channels can help reduce churn, as certain channels exhibit higher churn rates.
Competitive Pricing: Offering personalized and competitive pricing, especially for high-margin customers, can further increase retention.
Price Sensitivity: While price sensitivity is not the main driver of churn, it is a weak contributor. The main drivers include net margin, consumption over 12 months, and customer tenure. 
