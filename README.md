# Happy-Customers

The project involved developing a machine learning model to predict customer satisfaction for a company. The model utilized six features: whether the project was delivered on time, whether the content met expectations, whether the customer was able to order everything they wanted, price, courier service, and the user-friendliness of the app.

The first step in the project was to perform exploratory data analysis (EDA) to detect correlations between these features. Next, I used the lazypredict library to identify the best-fitting algorithms for the dataset. I then employed the Hyperopt library to optimize the parameters of the algorithms selected by lazypredict.

The Quadratic Discriminant Analysis (QDA) classifier yielded the highest accuracy at 77%. The recall for class 0 (unhappy customers) was 0.79, indicating that most unhappy customers were correctly identified. This insight allows the company to better address the concerns of dissatisfied customers and understand what causes their dissatisfaction.

To further improve the model, I used the StackingClassifier and VotingClassifier to ensemble the best-performing algorithms. I also employed the RFE (Recursive Feature Elimination) library for feature selection, which revealed that three features were not correlated with customer satisfaction. This finding suggests that the company can remove three questions from its questionnaire, allowing it to focus on the most relevant factors affecting customer satisfaction. This reduction in data collection can significantly lower costs and improve the management of key parameters.

## Requirements

```pip install -r requirements.txt```

