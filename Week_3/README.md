# Week 03 — Maximum Likelihood, Naive Bayes and PCA

## 📚 Topics Covered:
- Maximum Likelihood Estimation (MLE) for mean and variance
- Covariance and correlation matrices
- Bivariate normal distributions
- Gaussian Naive Bayes assumptions
- Document classification with Naive Bayes
- Dimensionality reduction with PCA and scree plots

---

### ✅ Learning Objectives:
- Apply **MLE** to estimate the mean and variance of a normal distribution.
- Compute **covariance matrices, correlation coefficients, and mean vectors** for bivariate normal datasets.
- Understand when a bivariate distribution has an **inclined slope** and how variance differs across axes.
- Identify which parts of a covariance matrix are used in **Gaussian Naive Bayes**.
- Classify text documents into categories using **Naive Bayes** with word counts.
- Learn how **Principal Component Analysis (PCA)** reduces dimensionality and interpret results with a **scree plot**.

---

### 📝 Key Concepts & Explanations:

1. **Maximum Likelihood Estimation (MLE)**   
   For the sample [4.43, -0.67, 1.60, 2.65, 3.89, 1.93, -1.52]:  
   - Mean (μ) = **1.76**  
   - Variance (σ²) = **4.168**

   → MLE provides unbiased estimates of distribution parameters.

---

2. **Bivariate Normal Distribution**   
   Given:  
x1 = [3.7, -1.6, -0.6, 0.8]
x2 = [0.7, 1.7, 5, 7]

- Mean vector = [0.58, 3.6]  
- Covariance matrix:  
  ```
  [ 1.995   -1.452 ]
  [ -1.452   2.527 ]
  ```
- Correlation matrix:  
  ```
  [1   0.288]
  [0.288  1]
  ```

→ Negative covariance indicates an **inclined slope** between variables.

---

3. **Gaussian Naive Bayes**   
- Assumes variables are **independent and Gaussian-distributed**.  
- Uses only the **diagonal entries** of the covariance matrix (ignores covariances).

---

4. **Text Classification Example**   
Training documents were divided into **Class_good** and **Class_bad**.  
For the test document:  
Document_?: love great terrible bad

Word frequencies showed **bad** and **terrible** dominated.  
→ Classified as **Class_bad**.

---

5. **Principal Component Analysis (PCA)**   
- Reduces high-dimensional data into fewer dimensions while preserving variance.  
- Extracts **principal components** as linear combinations of features.  
- **Scree graph** shows variance explained by each component.  
  → The “elbow” point helps decide how many components to keep.

---

### 📊 Week 3 Results:
- Learned to compute **mean, variance, covariance and correlation** using MLE.
- Applied **Gaussian Naive Bayes** to document classification.
- Understood how PCA simplifies complex datasets and how to interpret scree plots.

---

### 📂 Deliverables:
- 📄 [Week 3 Assignment PDF](./assignment.pdf)
- 📓 Example notebooks (to be developed in `notebooks/`)
- 📝 Notes and reflections in `notes.md`

---

### 🔖 Reflections:
- MLE gave hands-on practice in estimating parameters from raw data.  
- The **Naive Bayes text classification** showed how simple frequency counts can power classification.  
- PCA was insightful — especially understanding the **trade-off between dimensionality reduction and variance retention**.

---

### ✅ Checklist:
- [x] Upload Week 3 assignment
- [ ] Add Jupyter notebook for MLE and Naive Bayes
- [ ] Add PCA scree plot visualization
- [ ] Expand notes in `notes.md`

---
