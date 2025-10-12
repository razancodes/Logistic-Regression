# My Logistic Regression Implementation in Python

In this repository, I have created a Jupyter notebook that shows my complete implementation of Logistic Regression from scratch. Through this project, I aimed to deepen my understanding by combining mathematical theory with hands-on coding and visualization using `numpy` and `matplotlib`.

## Overview

Logistic Regression is a fundamental binary classification algorithm that models the probability of an input belonging to a class using the logistic sigmoid function. In my notebook, I cover the following:

- Loading and visualizing a binary classification dataset.
- The math behind logistic regression, including the sigmoid function and cost optimization.
- Writing the cost function manually (binary cross-entropy loss).
- Computing gradients of weights and bias for learning.
- Implementing gradient descent to optimize parameters.
- Evaluating the model and visualizing the decision boundary.

## What I Learned

### Logistic Function (Sigmoid)

I learned that the heart of logistic regression is the sigmoid function, which maps any real number \(z\) (which is a linear combination of input features and model parameters) to a value between 0 and 1:
<img width="249" height="199" alt="image" src="https://github.com/user-attachments/assets/f1a9dd81-277e-417c-af21-25aa1a2a6ade" />

where
<img width="208" height="83" alt="image" src="https://github.com/user-attachments/assets/c5e71dc1-b57a-4a78-abcc-94be033841a2" />

This output represents the probability of the input belonging to the positive class.

### Cost Function (Binary Cross-Entropy Loss)

To measure how well the model fits the data, I implemented the binary cross-entropy loss function:

<img width="734" height="94" alt="image" src="https://github.com/user-attachments/assets/66a9609d-9999-4f79-a974-c37fda2c24fe" />


This function heavily penalizes wrong predictions, guiding the model to improve.

### Gradients and Parameter Updates

Through calculus, I derived the gradients of the cost function with respect to each parameter, which are necessary for gradient descent:

<img width="370" height="207" alt="image" src="https://github.com/user-attachments/assets/2acd435b-5b04-4ec6-81fa-6acb68248311" />


Using these, I updated the parameters iteratively:
<img width="257" height="167" alt="image" src="https://github.com/user-attachments/assets/c6334012-2e56-4fa8-a407-10941c11dc25" />

where \(\alpha\) is the learning rate controlling the step size.

### Implementation Highlights

- I used `numpy` for efficient numerical computation and `matplotlib` for plotting data and results.
- I learned how to structure and vectorize the code for efficient training.
- I tracked the cost over iterations to ensure the model was converging.
- The notebook also includes detailed plots of the data points and the final decision boundary.

---

## How to Use This Repository

1. Clone the repository to your local machine.
2. Open the `logistic-regression.ipynb` notebook with Jupyter Notebook or any Jupyter-compatible environment.
3. Run all cells step-by-step to see the training process and visualize the results.
4. Feel free to modify parameters like learning rate, number of iterations, or try your own dataset for further experimentation.

---

## Results and Insights

- The model training shows a clear decrease in the cost function over epochs.
- Accuracy on training data is printed, and the decision boundary effectively separates the classes.
- This process helped me solidify my understanding of both the theory and implementation of logistic regression.

---

## Requirements

- Python 3.x
- `numpy`
- `matplotlib`
- `pandas` (for data handling)

You can easily install these with:
`pip install numpy matplotlib pandas`

---

Feel free to dive into the code, ask questions, or suggest improvements!

