# Week 05 — Neural Networks & Multilayer Perceptrons

## 📚 Topics Covered
- Neural Networks vs Logistic Regression 
- Structure of output layers for classification vs regression 
- Activation functions: Sigmoid, Tanh, ReLU, Softplus 
- Regularization in neural networks 
- Building and training Multilayer Perceptrons (MLPs)
- Applying neural networks on:
  - Advertising dataset (regression)
  - notMNIST dataset (classification)
  - KDD Cup 1999 dataset (network intrusion detection)

---

### ✅ Learning Objectives
- Understand how neural networks extend logistic regression to handle nonlinear and large-scale tasks.
- Implement different activation functions and interpret their outputs.
- Differentiate between regression and classification neural networks.
- Explore the role of **regularization (L1/L2)** in reducing overfitting.
- Train MLP models on real-world datasets and evaluate their performance.

---

### 📝 Short Answer Highlights
1. **Neural Networks vs Logistic Regression**  
   - Neural networks: multiple layers, nonlinear activation, handle unstructured data like text and images.  
   - Logistic regression: linear decision boundary, interpretable, efficient for small structured datasets .  

2. **Output Layer Differences**  
   - Classification: one neuron per class with softmax/sigmoid.  
   - Regression: single neuron outputting continuous values .  

3. **Activation Functions (input = -3)**  
   - Sigmoid: **0.047**  
   - Tanh: **-0.995**  
   - ReLU: **0**  
   - Softplus: **0.048**   

4. **Regularization**  
   Prevents overfitting, improves generalization, stabilizes training on limited or complex data .  

---

### 📊 Programming Assignments

#### 1. notMNIST Classification
ter images into 784 features.  
- MLP model:  
  - Dense (256, sigmoid, L2=0.01)  
  - Dense (128, sigmoid, L2=0.01)  
  - Dense (10, sigmoid, L2=0.01)  
- Optimizer: SGD with learning rate 0.1.  
- **Final losses**:  
  - Training: **1.690**  
  - Validation: **1.695**  

---

#### 2. Advertising Dataset (Regression)
- Input: TV ad budgets; Target: Sales.  
- Scaled features with `StandardScaler`.  
- MLP model:  
  - Dense(2, sigmoid) → Dense(1, linear).  
- Trained for 100 epochs, batch size = 256.  
- **Final RMSE**: ~**10.64**.  
- Visualized regression line and residuals.  

---

#### 3. KDD Cup 1999 Dataset (Network Intrusion Detection)
- Input: 494,021 rows × 42 features.  
- Preprocessed categorical features using one-hot encoding.  
- Converted target: normal (0) vs anomaly (1).  

**Logistic Regression Model (baseline):**  
- One dense sigmoid neuron.  
- Accuracy: **99.5%**  
- Confusion Matrix:  
[[48217 614]
[ 620 197560]]


**MLP Model (improved):**  
- Dense(4, relu) → Dense(2, relu) → Dense(1, sigmoid).  
- Final loss: **0.0244**  
- Accuracy: **99.7%**  
- Confusion Matrix:  
[[48746 586]
[ 91 197588]]


---

### 📂 Deliverables
- 📄 [Week 5 Short Answers PDF](./short_answers.pdf)  
- 📄 [Week 5 Assignment Notebook PDF](./assignment_notebook.pdf)  
- 📓 Example notebooks in `notebooks/`  
- 📝 Notes and reflections in `notes.md`

---

### 🔖 Reflections
- Neural networks generalize logistic regression by enabling nonlinear feature interactions.  
- Choice of activation function affects learning capability significantly.  
- Regularization is crucial for avoiding overfitting, especially with deep architectures.  
- Hands-on training with datasets (notMNIST, Advertising, KDD Cup 1999) demonstrated the versatility of MLPs for both **classification and regression** tasks.  

---

### ✅ Checklist
- [x] Upload Week 5 assignments  

---

