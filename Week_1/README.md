# DATA-55000 — Supervised Machine Learning

This repository contains Week_1 coursework, assignments and projects for **DATA-55000: Supervised Machine Learning**.
The goal of this repository is to track my weekly progress, document learnings and provide reproducible code and notes for each module.

---

## 📅 Week 01 — Introduction to Machine Learning

### ✅ Learning Objectives
- Define **Machine Learning (ML)** and its role in solving real-world problems.
- Distinguish between **Supervised** and **Unsupervised** learning.
- Understand the **dimensions of supervised learning algorithms**:
  - **Model**: The mathematical framework used for predictions.
  - **Loss Function**: The error measurement between predictions and actual values.
  - **Optimization Procedure**: Iterative process to minimize loss and improve accuracy.
- Learn to evaluate models with a **confusion matrix** using **precision, recalland accuracy**.
- Identify limitations of the **Perceptron** and how gradient descent with MSE addresses them.
- Apply **Occam’s Razor** in choosing simpler models over complex ones.

---

### 📝 Key Concepts & Explanations
1. **What is Machine Learning?**  
   ML enables computers to automatically learn from historical data without explicit programming.  
   Applications: speech recognition, image classification, medical predictions, business forecasting.

2. **Supervised vs. Unsupervised Learning**  
   - **Supervised Learning**: Works with labeled datasets, making it best for predictive modeling tasks.  
   - **Unsupervised Learning**: Groups unlabeled data into clusters or discovers hidden patterns.  
   → For labeled training pairs, **Supervised Learning is optimal**.

3. **Dimensions of Supervised Learning**.
   - **Model**: Maps input to output (e.g., linear regression, decision trees).
   - **Loss Function**: Quantifies error (e.g., MSE, cross-entropy).
   - **Optimization Procedure**: Updates model parameters to minimize loss (e.g., gradient descent).

4. **Confusion Matrix Example**  
- Precision = 0.86  
- Recall = 0.89  
- Accuracy = 0.87.
**Interpretation**: The model is performing well with balanced precision and recall, meaning it correctly identifies positives while keeping false alarms relatively low.

5. **Limitations of the Perceptron**  
- Works only for linearly separable data.  
- Struggles with convergence on non-linear datasets.  
- Uses a step function, which is not differentiable.  

**Solution**: Gradient Descent with **Mean Squared Error (MSE)** in Multi-Layer Perceptron (MLP) allows optimization and handles non-linear patterns.

6. **Occam’s Razor** — Why Simpler Models Are Better.
- Easier to interpret and communicate.
- Less resource-intensive, faster to train.
- Lower risk of overfitting.
- More stable and cost-effective.

---

### 📊 Week 1 Results
- Learned the foundation of supervised ML.
- Understood trade-offs between **simplicity vs. complexity** in modeling.
- Achieved working knowledge of confusion matrix metrics.
- Identified how optimization improves learning in neural networks.

---

### 📂 Deliverables
- 📄 [Week 1 Assignment PDF](./assignment.pdf)
---

### 🔖 Reflections
- This week helped me build a **solid foundation** in the basics of ML.  
- I realized that **model interpretability** is often as important as predictive accuracy.  
- Understanding **error metrics** like precision and recall made me appreciate their importance in imbalanced datasets (e.g., medical diagnosis, fraud detection).  
- I see how **gradient descent** is the backbone of modern ML optimization.

---
