# Marketing Campaign Profit Analysis

## Project Overview

This project focuses on optimizing marketing campaign strategies using machine learning models to maximize profit. By predicting customer responses to marketing offers, the project aims to enhance the efficiency of campaigns, increasing profits and reducing unnecessary expenditures. The analysis evaluates different models and their ability to predict responses, providing insights and recommendations for improving marketing efforts.

## Dataset

The dataset used in this project contains customer information, including past campaign responses, demographic details, and spending habits. Key features include:

- **AcceptedCmp1-5**: Indicates whether the customer accepted offers from previous campaigns.
- **Response**: Target variable indicating if the customer accepted the most recent campaign offer.
- **Income**: Customer's yearly household income.
- **MntWines, MntFruits, MntMeatProducts, MntFishProducts, MntSweetProducts, MntGoldProds**: Amount spent on various product categories.
- **Recency**: Number of days since the last purchase.
- **Total_Children**: Total number of children in the household.
- **Total_Spent**: Total amount spent on all products.

## Project Workflow

1. **Data Preprocessing**: 
   - Handled missing values by imputing with the median.
   - Converted categorical variables to numerical values using one-hot encoding.
   - Engineered new features, such as total number of children and total amount spent on products.

2. **Model Training and Evaluation**:
   - Trained multiple machine learning models, including Random Forest, Gradient Boosting, and Logistic Regression.
   - Evaluated the models based on their ability to predict customer responses and their impact on estimated profits.

3. **Profit Analysis**:
   - Calculated the estimated profit for each model on the test set.
   - Compared the profitability of different strategies: contacting everyone, contacting no one, and using the best-performing model.

## Key Findings

- **Random Forest** emerged as the best-performing model, with an estimated profit of **$116.00** on the test set.
- The strategy of contacting customers based on the model's predictions significantly outperformed the blanket strategy of contacting everyone, with a **119.83%** improvement in profit.
- Key features driving model performance included **'Recency'**, **'Total_Spent'**, and **'Income'**.

## Recommendations

- **Targeted Marketing**: Focus marketing efforts on customers with high spending and recent purchases to maximize response rates and profitability.
- **Model Enhancement**: Consider improving recall for responders through model adjustments or incorporating additional data.
- **Continuous Learning**: Regularly update the model with new data to maintain accuracy and relevance.

## Conclusion

This project demonstrates the value of data-driven decision-making in marketing campaigns. By leveraging machine learning models, businesses can optimize their marketing strategies, leading to substantial improvements in profitability and resource allocation.
