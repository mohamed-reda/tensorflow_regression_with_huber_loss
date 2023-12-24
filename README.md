**Project Title: TensorFlow Regression with Huber Loss**

**README.md:**

# TensorFlow Regression with Huber Loss

This project demonstrates how to implement regression using TensorFlow with a focus on utilizing the Huber loss
function. The Huber loss is particularly useful in scenarios with outliers, as it provides a more robust alternative to
the standard mean squared loss.

## Exercise Overview

In this project, we tackle the following exercise:

**Change the Loss Function to Huber Loss**

*Problem Statement:* Change the loss function in the regression model from mean squared loss to Huber loss. The Huber
loss is less sensitive to outliers, making it a suitable choice for datasets with potential outliers.

*Solution:*
Find the line where the loss is defined and change it from:

```python
model.compile(optimizer=custom_optimizer, loss='mean_squared_loss')
```

to:

```python
model.compile(optimizer=custom_optimizer, loss='huber_loss')
```

Remember to rerun all cells after making changes to ensure the updated loss function is used.

## Key Takeaways

- The Huber loss is effective when dealing with datasets containing outliers.
- The implementation details showcase how to adapt the loss function in TensorFlow for regression tasks.

## Project Structure

1. **Introduction to TensorFlow:**
    - Data generation using NumPy.
    - Saving generated data into an npz file for future access.

2. **Solving with TensorFlow:**
    - Loading training data from the npz file.
    - Defining a regression model using TensorFlow's Sequential API.
    - Customizing the optimizer and changing the loss function to Huber loss.
    - Fitting the model to the training data.

3. **Extracting Model Parameters:**
    - Extracting weights and biases from the trained model for examination.

4. **Making Predictions:**
    - Demonstrating how to use the trained model to make predictions on new data.

5. **Plotting the Results:**
    - Visualizing the model outputs compared to the actual targets.

## Getting Started

1. Clone this repository: `git clone https://github.com/yourusername/tensorflow-regression-huber-loss](https://github.com/mohamed-reda/tensorflow_regression_with_huber_loss.git`
2. Navigate to the project directory: `cd tensorflow-regression-huber-loss`
3. Run the Jupyter notebook: `jupyter notebook`

Feel free to explore the notebook, experiment with the code, and adapt it to your specific use cases.

Happy coding! 🚀
---


to run jupyter:

jupyter notebook

(Use Control-C to stop this server)

----
pip install -r requirements.txt

python -m pip install jupyter

---
memory profile:

@memory_profiler.profile

python -m memory_profiler main.py

---

from line_profiler_pycharm import profile

@profile

python -m line_profiler main.py.lprof > results.txt
