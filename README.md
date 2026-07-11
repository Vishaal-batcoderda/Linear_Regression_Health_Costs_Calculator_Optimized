# Healthcare Cost Prediction Using Linear Regression (Optimized)

This project is an extension of my original **Healthcare Cost Prediction** project from the freeCodeCamp Machine Learning with Python certification.

Instead of relying on a machine learning library to train the model, I wanted to understand what actually happens behind the scenes. So I rebuilt the entire Linear Regression algorithm from scratch using **NumPy** and pure mathematics.

The goal of this project was not just to get accurate predictions, but to understand how gradient descent updates the model parameters, how the cost decreases over time, and how feature engineering improves performance.

---

## Previous Version (freeCodeCamp)

If you're interested in the original implementation that follows the freeCodeCamp workflow using TensorFlow/Keras, you can find it here:

🔗 **Original Project:**  
https://github.com/Vishaal-batcoderda/Linear_Regression_Health_Costs_Calculator

This repository is the continuation of that project with a manual implementation of Linear Regression.

---

## Project Summary

The model predicts **medical insurance expenses** using patient information such as:

- **Age**
- **Sex**
- **BMI**
- **Number of children**
- **Smoking status**
- **Region**

Unlike the original version, this implementation does **not** use TensorFlow or scikit-learn's Linear Regression model.

Instead, every step of the learning process is implemented manually.

---

## What I Changed

Compared to the original implementation, this version includes:

- Manual implementation of Linear Regression
- Feature normalization
- Gradient Descent optimization
- L2 Regularization
- Polynomial feature engineering
- Cost function visualization
- Manual Mean Absolute Error calculation

The objective was to understand the mathematics behind the algorithm instead of treating it as a black box.

---

## Feature Engineering

To better capture non-linear relationships, I added two interaction features:

- `bmi × smoker`
- `age × smoker`

These features significantly improved the model's prediction performance.

---

## How the Model Works

The workflow followed in this project is:

1. Load the dataset
2. Convert categorical variables using One-Hot Encoding
3. Split the dataset into training and testing sets
4. Create additional polynomial features
5. Normalize all features
6. Initialize weights and bias
7. Compute predictions
8. Calculate the cost function
9. Compute gradients
10. Update parameters using Gradient Descent
11. Repeat until convergence
12. Evaluate using Mean Absolute Error (MAE)

---

## Concepts Implemented

Everything below was implemented manually:

- Linear Regression
- Batch Gradient Descent
- Cost Function (Mean Squared Error)
- Gradient Computation
- Weight Updates
- Bias Updates
- Feature Scaling
- One-Hot Encoding
- Polynomial Features
- L2 Regularization
- Mean Absolute Error (MAE)

---

## Visualizations

The notebook includes:

- Cost vs Iterations graph
- Prediction vs Actual Expenses scatter plot

These plots make it easier to understand how the model learns during training.

---

## How to Run This Project

This project was developed and tested using **Google Colab**.

### Steps

1. Open the notebook in Google Colab.
2. Run the cells from top to bottom.
3. The dataset is downloaded automatically.
4. The model trains using Gradient Descent.
5. The notebook displays:
   - Cost reduction
   - Training progress
   - Mean Absolute Error
   - Prediction plots

No additional setup is required when using Google Colab.

---

## Results

- Successfully predicts healthcare expenses using a manually implemented Linear Regression model.
- Achieves the freeCodeCamp challenge requirement of **Mean Absolute Error below 3500**.
- Demonstrates that Linear Regression can be implemented from scratch without relying on machine learning libraries.

---

## What I Learned

This project helped me understand concepts that are usually hidden behind machine learning libraries.

Some of the biggest takeaways were:

- How Gradient Descent actually updates parameters
- Why feature normalization improves convergence
- The role of regularization in reducing overfitting
- How feature engineering can improve predictions
- Why optimization is the heart of machine learning

Building everything manually gave me a much deeper understanding than simply calling a library function.

---

## Acknowledgements

The original challenge and dataset are provided by **freeCodeCamp** as part of their **Machine Learning with Python Certification**.

This optimized implementation is my own extension of that project to better understand the mathematics behind Linear Regression.

---

## Future Improvements

Some ideas I'd like to explore next:

- Mini-Batch Gradient Descent
- Stochastic Gradient Descent
- Adam Optimizer
- Ridge vs Lasso Regression comparison
- More advanced feature engineering
- Hyperparameter tuning

---

## Repository Structure

```
.
├── Linear_Regression_Health_Costs_Calculator_Optimized.ipynb
├── README.md
└── insurance.csv (downloaded automatically in Colab)
```

---

## Final Thoughts

Completing the freeCodeCamp challenge taught me **how to use** Linear Regression.

Building this optimized version taught me **how Linear Regression actually works.**

That difference made this project one of the most valuable learning experiences in my machine learning journey.
