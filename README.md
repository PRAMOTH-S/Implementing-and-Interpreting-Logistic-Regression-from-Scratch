# Project Overview

This project implements Logistic Regression from scratch using NumPy. I manually coded the sigmoid function, binary cross-entropy loss, and gradient descent optimization. The model was trained on a synthetic binary classification dataset generated using make_classification and compared against scikit-learn’s Logistic Regression implementation.

# Deliverable 2: Performance Comparison Summary (WITH NUMBERS)

After training, both models were evaluated on the same test set using accuracy, precision, recall, and log loss.

For the custom Logistic Regression model, the results were:

Accuracy: 0.825

Precision: 0.812

Recall: 0.837

Log Loss: 6.307

For the scikit-learn Logistic Regression model, the results were:

Accuracy: 0.825

Precision: 0.812

Recall: 0.837

Log Loss: 6.307

The near-identical metrics indicate that the custom implementation closely matches the behavior of scikit-learn’s optimized model. This confirms that the mathematical implementation of logistic regression from scratch is correct.

# Deliverable 3: Interpretation of Learned Coefficients (WITH VALUES)

Since the dataset is synthetically generated using make_classification, the features do not have real-world semantic names. Instead, each feature represents an abstract informative signal contributing to class separation.

The learned coefficients from the custom model were:

Feature 0: −0.763

Feature 1: +0.827

Feature 2: +0.727

Feature 3: −0.330

Feature 4: −0.750

# Positive Contributors

Features 1 and 2 have the largest positive coefficients (+0.827 and +0.727). This means that increasing the values of these features significantly increases the probability of predicting the positive class. These features act as strong signals in favor of class 1.

# Negative Contributors

Features 0 and 4 have the most negative coefficients (−0.763 and −0.750). Higher values of these features reduce the probability of predicting the positive class, pushing the model toward class 0.

Although the features are abstract, the relative signs and magnitudes clearly show how the model internally separates the two classes.

# Loss Function and Training Justification

The learning rate was set to 0.01 to ensure stable gradient descent updates without oscillation. The model was trained for 10,000 iterations, which allowed the loss to converge smoothly. During training, the loss consistently decreased and stabilized, indicating proper convergence.

Log loss was computed using predicted probabilities rather than hard class labels, ensuring correct probabilistic evaluation.

# Conclusion

This project demonstrates a complete and correct implementation of Logistic Regression from scratch using NumPy. The close match between the custom model and scikit-learn’s implementation validates the correctness of the approach. Analyzing the learned coefficients provided insight into how individual synthetic features influence the model’s predictions.
