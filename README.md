# E-Commerce Product Return Prediction

## About the Project
Product returns are one of the most persistent challenges in e-commerce. They increase operational costs, complicate inventory planning, and undermine customer satisfaction. The purpose of this project was to design a machine learning framework capable of predicting whether a purchased product would be returned.  

By transforming historical purchase records into predictive insights, the project demonstrates how businesses can move from reactive handling of returns to proactive management. The dataset included customer demographics, product characteristics, and delivery details, all of which were explored through visualizations and statistical summaries. After cleaning and transformation, the data was split into training and testing sets to allow for a fair assessment of predictive models.  

## Methodology
The workflow began with exploratory data analysis to uncover trends in return behavior. Product categories and delivery speed immediately stood out as influential factors, while demographic characteristics added further nuance. Preprocessing involved handling missing values, encoding categorical features, and scaling numerical variables to ensure model stability.  

Two supervised learning models were developed and evaluated: Logistic Regression and K-Nearest Neighbors (KNN). Their performance was measured using accuracy, precision, recall, F1 score, and ROC AUC to provide both technical and business-oriented comparisons.  

## Model Comparisons
The two models were evaluated on the test set, and their results are summarized below:  

| Model               | Accuracy | Precision (0/1) | Recall (0/1) | F1 (0/1) | ROC AUC |
|----------------------|----------|-----------------|--------------|----------|---------|
| Logistic Regression | 0.92     | 0.92 / 0.92     | 0.92 / 0.91  | 0.92 / 0.91 | 0.976 |
| KNN (k=15)          | 0.89     | 0.85 / 0.95     | 0.96 / 0.82  | 0.90 / 0.88 | 0.957 |

Logistic Regression provided slightly higher accuracy and the advantage of interpretability, making it easier to explain the role of variables such as product category and delivery speed. KNN, while competitive in performance, required parameter tuning and showed higher sensitivity to the feature space.  

From a business perspective, Logistic Regression is the more practical choice for deployment due to its strong performance and transparency, while KNN serves as a useful benchmark to validate results.  

## Results and Insights
Across both models, the same predictors consistently influenced return likelihood. Certain product categories carried higher return risks, delivery delays were closely linked with dissatisfaction and returns, and specific customer segments exhibited repeat return behavior.  

The analysis confirms that return prediction is not only technically feasible but also actionable. By identifying transactions with a high likelihood of return, businesses can preemptively address issues through better product descriptions, optimized logistics, and targeted customer engagement.  

## Recommendations
The findings translate into three strategic recommendations for e-commerce businesses:  

1. Enhance product descriptions and imagery in high-risk categories to reduce mismatched expectations.  
2. Prioritize reliable and timely deliveries, as delays significantly increase return probabilities.  
3. Monitor and proactively engage customer segments with higher return tendencies, balancing satisfaction with profitability.  

Combining predictive accuracy with interpretability ensures both operational benefits and executive-level decision support. Logistic Regression, in particular, provides a balance between performance and clarity that makes it suitable for deployment at scale.  

This project demonstrates that product returns in e-commerce can be predicted with meaningful accuracy using supervised learning methods. Logistic Regression emerged as the most practical model, offering both strong predictive power and interpretability. KNN, while competitive, highlighted the trade-offs involved in parameter-sensitive approaches.  

The insights generated from this analysis have direct implications for inventory management, logistics optimization, and customer satisfaction strategies. By embedding predictive insights into day-to-day operations, e-commerce firms can reduce the financial burden of returns while strengthening customer loyalty and trust.  

## Repository Structure
