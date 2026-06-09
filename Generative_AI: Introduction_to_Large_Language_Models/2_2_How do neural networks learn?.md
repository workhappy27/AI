***

# 📘 How Neural Networks Learn

## 🔹 1. Basic Idea

* Neural networks learn by:
  * Modeling relationship between **inputs (X)** and **output (Y)**
* Similar to **supervised learning**

✅ Input: Features (independent variables)  
✅ Output: Target (dependent variable)

***

## 🔹 2. Learning Mechanism

* Network adjusts:
  * **Weights**
  * **Biases**

👉 Goal:

* Improve predictions by reducing error

***

## 🔹 3. Backpropagation (Core Learning Method)

* Main technique used to train neural networks

✅ Key Idea:

* Adjust weights **based on error**

***

## 🔹 4. Training Process (Epochs)

* Learning happens in cycles called **epochs**
* Each epoch has **2 phases**:

***

## 🔹 5. Forward Phase

### ✅ Steps:

1. Input data enters network
2. Multiply inputs by weights
3. Add bias
4. Apply activation function
5. Generate **predicted output**

✅ Example:

* Input → prediction = **0.622**

***

## 🔹 6. Backward Phase

### ✅ Steps:

1. Compare:
   * Predicted output vs actual output
2. Calculate error (loss function)
3. Adjust:
   * Weights
   * Biases

👉 Goal:

* Reduce difference between prediction and actual value

***

## 🔹 7. Optimization

* Uses algorithms like:
  * **Gradient Descent (SGD)**

✅ Purpose:

* Decide how much to update weights

***

## 🔹 8. Iterative Learning

* Process repeats:
  * Epoch 1 → adjust
  * Epoch 2 → better prediction
  * Epoch 3 → further improvement

👉 Continues until:

* Error is very small
* Model stabilizes (**convergence**)

***

## 🔹 9. Final Output

* Final set of:
  * Weights
  * Biases

✅ Represents a **trained neural network**

***

## 🔁 Complete Learning Flow

👉 **Input → Forward Pass → Prediction → Error Calculation → Backward Pass → Update Weights → Repeat**

***

## ✅ Key Concepts

* **Epoch** → one full training cycle
* **Loss function** → measures error
* **Backpropagation** → updates weights
* **Optimization** → minimizes error
* **Convergence** → stable accurate model

***

## ✅ One-Line Summary

**Neural networks learn by repeatedly making predictions, measuring errors, and adjusting weights using backpropagation until the predictions become accurate.**

***

## ✅ Simple Memory Trick

👉 **Predict → Compare → Correct → Repeat**

***
