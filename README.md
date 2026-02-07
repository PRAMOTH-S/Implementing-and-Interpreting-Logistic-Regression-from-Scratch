# Implementing-and-Interpreting-Logistic-Regression-from-Scratch
This project implements Logistic Regression from scratch using NumPy, including sigmoid activation, binary cross-entropy loss, and gradient descent optimization. The custom model is trained on synthetic data and evaluated against scikit-learn’s Logistic Regression, with performance comparison and coefficient interpretation.
# Deliverable 2: Performance Comparison Summary
The custom Logistic Regression model and the scikit-learn Logistic Regression model were evaluated using accuracy, precision, recall, and log loss.
The custom model achieved an accuracy of approximately 82.5%, with precision and recall values close to the scikit-learn implementation. The scikit-learn model performed marginally better overall due to optimized solvers and built-in regularization.
Despite this, the small difference in performance confirms that the custom implementation correctly captures the underlying mathematics of logistic regression.
# Deliverable 3: Interpretation of Learned Coefficients
The learned coefficients represent how each feature influences the probability of predicting the positive class.
Features 1 and 2 have the highest positive coefficients, meaning they contribute most strongly to increasing the probability of class 1. As the values of these features increase, the model becomes more confident in predicting the positive outcome.
Features 0 and 4 have the most negative coefficients, meaning they reduce the probability of the positive class. Higher values of these features push the prediction toward class 0.
The sign of each coefficient indicates whether the feature has a positive or negative effect, while the magnitude reflects its relative importa#nce.
# Loss Function Comparison
Log loss was computed using predicted probabilities for both the custom model and the scikit-learn model, as required. The scikit-learn model achieved a slightly lower log loss due to numerical optimizations, while the custom model demonstrated comparable behavior, confirming correct probability estimation.
# Hyperparameter Justification
The learning rate was set to 0.01 to ensure stable convergence without overshooting the minimum of the loss function. The number of iterations was set to 10,000 to allow sufficient time for convergence, which was confirmed by observing a stable decrease in the loss during training.
# Conclusion
This project successfully demonstrates the implementation of Logistic Regression from scratch using NumPy. The close alignment between the custom and scikit-learn models validates the correctness of the implementation and provides insight into feature importance through coefficient interpretation.
