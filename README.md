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

# Linear Regression vs Logistic Regression

# Linear Regression

![image](https://github.com/TITHI-KHAN/Logistic-Regression-/assets/65033964/6ca2e744-7b68-4e91-a052-446236631454)

![image](https://github.com/TITHI-KHAN/Logistic-Regression-/assets/65033964/3258640b-12b1-435b-9443-2a6f7ec3abd2)

# Logistic Regression

![image](https://github.com/TITHI-KHAN/Logistic-Regression-/assets/65033964/027dc8ce-efe1-4f2e-b27d-4fdafbccb9ac)

![image](https://github.com/TITHI-KHAN/Logistic-Regression-/assets/65033964/eb14a233-c30e-4a94-a668-e929e3c5b34b)

![image](https://github.com/TITHI-KHAN/Logistic-Regression-/assets/65033964/ad306d3a-c538-441e-a60a-af131784c844)

![image](https://github.com/TITHI-KHAN/Logistic-Regression-/assets/65033964/a1b58f25-cbd7-428a-a95b-911b005827d9)


