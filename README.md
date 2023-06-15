# Logistic-Regression

Logistic regression is a statistical model commonly used for binary classification problems, where the target variable has two possible classes. However, logistic regression can also be extended to handle multi-class classification tasks.

Here are some key details about logistic regression:

1. Assumption: Logistic regression assumes that the relationship between the features and the log-odds of the target variable is linear. It models the log-odds using a logistic function, also known as the sigmoid function.

2. Sigmoid function: The sigmoid function is used as the activation function in logistic regression. It maps any real-valued number to a value between 0 and 1, representing the probability of the positive class. The sigmoid function is defined as:
sigmoid(z) = 1 / (1 + exp(-z)) where z is the linear combination of features and their corresponding weights
or y = 1 / (1 + np.exp(-(m * x + c)))

3. Training process: Logistic regression learns the optimal weights by minimizing a cost function, typically the log loss or cross-entropy loss. This optimization is performed using iterative numerical optimization algorithms, such as gradient descent.

4. Model interpretation: In logistic regression, the weights associated with each feature indicate the strength and direction of their influence on the target variable. Positive weights suggest a positive association, while negative weights suggest a negative association.

5. Decision boundary: Logistic regression defines a decision boundary that separates the classes in the feature space. For binary classification, the decision boundary is a linear hyperplane. In multi-class classification, multiple decision boundaries are used.

6. Regularization: Logistic regression can be regularized to prevent overfitting. Regularization techniques, such as L1 (Lasso) or L2 (Ridge), can be applied to penalize large weights and control model complexity.

7. Evaluation: The performance of a logistic regression model can be evaluated using various metrics such as accuracy, precision, recall, F1-score, and area under the ROC curve (AUC-ROC).

Logistic regression is widely used in various domains, including healthcare, finance, marketing, and social sciences, for tasks such as disease prediction, customer churn analysis, spam detection, and sentiment analysis.

# Sigmoid vs Softmax

The sigmoid function is used for the two-class logistic regression, whereas the softmax function is used for
the multiclass logistic regression.

The main advantage of using Softmax is the output probabilities range. The range will 0 to 1, and the sum
of all the probabilities will be equal to one. If the softmax function used for multi-classification model it
returns the probabilities of each class and the target class will have the high probability.

![image](https://github.com/TITHI-KHAN/Logistic-Regression-/assets/65033964/d022c8d9-5e94-44ec-b4ad-0ca7d7b773f8)

# Linear Regression

Linear regression is a statistical modeling technique used to establish a relationship between a dependent variable and one or more independent variables. It assumes a linear relationship between the variables and aims to find the best-fitting linear equation that describes the data.

Here are some key details about linear regression:

1. Assumption: Linear regression assumes a linear relationship between the independent variables (predictors) and the dependent variable (response). It assumes that the relationship can be represented by a straight line.

2. Equation: In simple linear regression, with one independent variable, the equation takes the form:
y = mx + c

where y is the dependent variable, x is the independent variable, m is the slope (regression coefficient), and c is the y-intercept.

3. Multiple linear regression: When there are multiple independent variables, the equation becomes:
y = b0 + b1x1 + b2x2 + ... + bnxn

where y is the dependent variable, x1, x2, ..., xn are the independent variables, and b0, b1, b2, ..., bn are the regression coefficients.

4. Training process: Linear regression aims to find the optimal regression coefficients that minimize the sum of squared differences between the predicted values and the actual values in the training data. This is typically done using the least squares method or other optimization techniques.

5. Model interpretation: In linear regression, the regression coefficients indicate the change in the dependent variable associated with a one-unit change in the corresponding independent variable, holding other variables constant. The intercept term (c or b0) represents the expected value of the dependent variable when all independent variables are zero.

6. Evaluation: The performance of a linear regression model can be evaluated using metrics such as the coefficient of determination (R-squared), root mean squared error (RMSE), mean absolute error (MAE), and others. These metrics assess the goodness of fit and predictive accuracy of the model.

7. Extensions: Linear regression can be extended to handle nonlinear relationships by introducing polynomial terms, interaction terms, or using techniques like polynomial regression, stepwise regression, or ridge regression.

Linear regression is widely used for tasks such as prediction, forecasting, trend analysis, and understanding the relationship between variables in various fields including economics, finance, social sciences, and engineering.

![image](https://github.com/TITHI-KHAN/Logistic-Regression-/assets/65033964/6ca2e744-7b68-4e91-a052-446236631454)

![image](https://github.com/TITHI-KHAN/Logistic-Regression-/assets/65033964/3258640b-12b1-435b-9443-2a6f7ec3abd2)

# Logistic Regression

![image](https://github.com/TITHI-KHAN/Logistic-Regression-/assets/65033964/027dc8ce-efe1-4f2e-b27d-4fdafbccb9ac)

![image](https://github.com/TITHI-KHAN/Logistic-Regression-/assets/65033964/eb14a233-c30e-4a94-a668-e929e3c5b34b)

![image](https://github.com/TITHI-KHAN/Logistic-Regression-/assets/65033964/ad306d3a-c538-441e-a60a-af131784c844)

# Linear Regression vs Logistic Regression

Linear regression and logistic regression are both popular statistical modeling techniques, but they have some fundamental differences in their purpose, assumptions, and application areas. Here's a comparison between linear regression and logistic regression:

1. Purpose:

Linear Regression: Linear regression is used to model and predict continuous numeric variables. It aims to establish a linear relationship between the dependent variable and one or more independent variables.
Logistic Regression: Logistic regression is used for binary classification problems. It models the relationship between the independent variables and the probability of a binary outcome (e.g., yes/no, 0/1).

2. Dependent Variable:

Linear Regression: The dependent variable in linear regression is continuous and assumes a wide range of possible values.
Logistic Regression: The dependent variable in logistic regression is binary or categorical. It represents the probability of a binary outcome and is typically coded as 0 or 1.

3. Assumptions:

Linear Regression: Linear regression assumes a linear relationship between the independent variables and the dependent variable. It also assumes that the residuals (the differences between predicted and actual values) are normally distributed and have constant variance.
Logistic Regression: Logistic regression assumes that the relationship between the independent variables and the log-odds of the binary outcome is linear. It assumes independence of observations and no multicollinearity among the independent variables.

4. Model Output:

Linear Regression: The output of linear regression is a continuous predicted value that can take any value along the range of the dependent variable.
Logistic Regression: The output of logistic regression is the predicted probability of belonging to a specific class (e.g., probability of being in class 1). It is constrained between 0 and 1.

5. Model Interpretation:

Linear Regression: In linear regression, the regression coefficients indicate the change in the dependent variable associated with a one-unit change in the corresponding independent variable.
Logistic Regression: In logistic regression, the regression coefficients represent the change in the log-odds of the binary outcome associated with a one-unit change in the corresponding independent variable.

6. Application Areas:

Linear Regression: Linear regression is commonly used in tasks such as predicting housing prices, analyzing the impact of variables on sales, estimating future values based on historical data, and other regression problems where the dependent variable is continuous.
Logistic Regression: Logistic regression is widely used in binary classification problems, such as predicting whether a customer will churn, classifying emails as spam or not spam, determining the likelihood of a disease occurrence, and other cases where the outcome is binary.

It's important to choose the appropriate regression technique based on the nature of the problem and the type of data you are working with. Linear regression is suitable for continuous outcome variables, while logistic regression is suitable for binary classification problems.

![image](https://github.com/TITHI-KHAN/Logistic-Regression-/assets/65033964/5b7c57f0-59bb-4b6b-974a-64ab44f7c537)


