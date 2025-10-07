# Week 07 — Crop Production Forecasting Using Supervised Machine Learning (Final Project Part 2)

## 📚 Topics Covered
- Application of supervised learning models on agricultural datasets
- Data preprocessing and feature scaling
- Crop type classification using Logistic Regression and Decision Tree models
- Model evaluation through accuracy and classification reports
- Comparison of model performance and insights from results

---

### ✅ Learning Objectives
- Train multiple supervised learning models on the **Crop Production dataset**.
- Preprocess large-scale agricultural data for classification tasks.
- Evaluate and compare **Logistic Regression** and **Decision Tree Classifier** models.
- Derive actionable insights from model results to improve agricultural decision-making.
- Understand how ML can support sustainable agriculture and yield prediction.

---

### 📝 Project Overview
The **Crop Production in India dataset** spans **28 years** and includes key agricultural parameters such as temperature, rainfall, pH, nutrient levels (N, P, K), area and crop yield.  
The goal was to **classify crop types** (Kharif, Rabi, Summer, etc.) based on environmental and soil features using supervised learning algorithms.

#### Dataset Summary:
- **Source:**: Kaggle
- **Rows:** 99,849  
- **Columns:** 13  
- **Features:** N, P, K, pH, rainfall, temperature, area, production, yield  
- **Target Variable:** `Crop_Type` (categorical)

---

### ⚙️ Data Preprocessing
Steps performed before modeling:
1. **Removed categorical columns:** `State_Name`, `Crop`, and `Crop_Type` (for encoding).  
2. **Encoded Target:** Converted `Crop_Type` labels into numerical values using **LabelEncoder()**.  
3. **Feature Scaling:** Standardized numerical features using **StandardScaler()** for model stability.  
4. **Data Split:**  
   - **Training Set:** 80%  
   - **Testing Set:** 20%  
   - **Random State:** 42 for reproducibility.

---

### 🤖 Machine Learning Models

#### 1. Logistic Regression
- Implemented using `sklearn.linear_model.LogisticRegression()`
- Handles multi-class classification of crop types based on environmental and soil parameters.
- Evaluated using **classification report** and **accuracy score**.

**Results:**
| Metric | Score |
|---------|-------|
| Precision | 0.87 |
| Recall | 0.84 |
| F1-Score | 0.85 |
| **Accuracy** | **87.26%** |

> The Logistic Regression model achieved strong performance, correctly classifying most crop types with high precision and recall.

---

#### 2. Decision Tree Classifier
- Implemented using `sklearn.tree.DecisionTreeClassifier(criterion="entropy")`
- Provides interpretable decision paths based on feature splits.
- Visualized tree structure and compared accuracy with Logistic Regression.

**Results:**
| Metric | Score |
|---------|-------|
| Precision | 1.00 |
| Recall | 1.00 |
| F1-Score | 1.00 |
| **Accuracy (raw)** | **100%** |
| **Adjusted Accuracy** | ~**38.25%** (after scaling adjustment) |

> While the Decision Tree model overfitted with perfect accuracy on training data, the realistic evaluation (~38%) showed lower generalization than Logistic Regression.

---

### 🔍 Comparative Analysis
| Model | Accuracy | Strengths | Limitations |
|--------|-----------|------------|--------------|
| Logistic Regression | 87.26% | Generalizes well, interpretable | Limited for non-linear boundaries |
| Decision Tree | 38–100% | Captures non-linear patterns | Prone to overfitting |

**Key Insight:** Logistic Regression provided a better generalization for large-scale, multi-class agricultural data, while Decision Tree’s performance highlighted the need for pruning or ensemble approaches like Random Forest for better stability.

---

### 🌾 Methodology Summary
1. **Data Exploration:**  
   - Used `data.describe()`, `.info()`, and `.corr()` to understand the dataset structure and relationships.  
   - Generated histograms for each numeric feature to visualize distributions.

2. **Model Implementation:**  
   - Built Logistic Regression and Decision Tree models using Scikit-learn.  
   - Evaluated models with accuracy, precision, recall, and F1-score.

3. **Insights:**  
   - Logistic Regression effectively classified crop seasons (Kharif, Rabi, Summer).  
   - Environmental factors like **rainfall** and **temperature** had moderate positive correlation with **production** and **yield**.

---

### 📊 Week 7 Results
- Demonstrated end-to-end supervised ML pipeline using real agricultural data.
- Achieved high accuracy in predicting crop types via Logistic Regression.
- Highlighted importance of data preprocessing and scaling in improving model accuracy.
- Provided groundwork for future improvements (e.g., Random Forest, Gradient Boosting).

---

### 🔖 Reflections
- Applying ML models to agriculture revealed how data can improve yield prediction and sustainable farming decisions.  
- Handling large datasets improved understanding of preprocessing and feature encoding.  
- Realized the significance of balancing **model complexity** and **interpretability**.  
- This project strengthens the bridge between **data science and agricultural innovation**.

---

### 📂 Deliverables
- 📄 [Week 7 Project Report](./Crop_Production_in_Agriculture.docx)
- 📄 [Week 7 Python Script](./project_2.py)
- 📄 [Week 7 Project Notebook (Colab PDF)](./project_2.ipynb.pdf)
- 📊 [Crop Production Dataset](./Crop_production.csv)
- 📝 Notes and reflections in `notes.md`

---

### ✅ Checklist
- [x] Load and preprocess dataset  
- [x] Implement Logistic Regression model  
- [x] Implement Decision Tree model  
- [x] Evaluate and compare model accuracy  

---
🗓️ **Week 07: Final Project (Part 2) — Supervised Learning Models**
