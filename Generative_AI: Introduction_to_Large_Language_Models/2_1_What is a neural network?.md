<img width="1024" height="1024" alt="image" src="https://github.com/user-attachments/assets/e1ff4781-0b36-49ff-8e8b-436338667355" />***

# 📘 Neural Networks – Notes

## 🔹 1. What is a Neural Network?

* A **neural network** is a computational model inspired by the **human brain**
* Consists of interconnected units called **neurons (nodes)**

✅ Purpose:

* Learn relationships between **inputs and outputs**
* Solve problems like prediction, classification, and pattern recognition

***


<img width="1024" height="1024" alt="image" src="https://github.com/user-attachments/assets/0ef59aa1-2bb5-4e5d-8cd6-8e4018a4c351" />


## 🔹 2. Biological Inspiration

### 🧠 Human Neuron:

* Receives signals via **dendrites**
* Processes signals → computes weighted sum
* If threshold reached → sends signal via **axon**

👉 Neural networks mimic this process digitally

***

## 🔹 3. Artificial Neuron (Basic Working)

### ✅ Steps:

1. Inputs are received
2. Each input is assigned a **weight (importance)**
3. Inputs are multiplied by weights
4. Weighted values are **summed**
5. **Bias** is added
6. Result passed through an **activation function**
7. Output is generated

***

## 🔹 4. Activation Function

* Converts summed input into **final output**
* Decides whether neuron should “fire”

### ✅ Common Types:

1. **Threshold (Step Function)**
   * Output: 0 or 1
   * Used for simple decisions

2. **Sigmoid Function**
   * Output: between **0 and 1**
   * Used in binary classification

3. **Tanh (Hyperbolic Tangent)**
   * Output: between **-1 and 1**
   * Zero-centered

4. **ReLU (Rectified Linear Unit)**
   * Output: 0 if negative, else same value
   * Most widely used

***

## 🔹 5. Learning Process

* Uses **numeric data**
* Adjusts weights based on:
  * Importance of input
  * Prediction accuracy

👉 Goal: Improve predictions over time

***

## 🔹 6. Example (Loan Default Prediction)

* Inputs:
  * Amount
  * Grade
  * Purpose

* Output:
  * Default (1) or No Default (0)

✅ Process:

* Inputs → weighted → summed → activation → prediction

***

## 🔹 7. Perceptron (Basic Neural Network)

* Simplest neural network model
* Single layer
* Uses threshold activation

✅ Limitation:

* Can only solve **simple problems**

***

## 🔹 8. Network Topology

* Structure of the network (layers & connections)

👉 Determines:

* Complexity of problems it can solve

***

## 🔹 9. Key Concepts Summary

* **Weights** → importance of inputs
* **Bias** → extra adjustment
* **Activation function** → decides output
* **Layers** → input, hidden, output

***

## ✅ One-Line Definition

**A neural network is a brain-inspired system of interconnected nodes that learns patterns by weighting inputs and passing them through activation functions to produce outputs.**

***

## ✅ Simple Memory Trick

👉 **Input → Weight → Sum → Activate → Output**

***
