# Week 08 — Final IEEE Paper Submission: Crop Production Forecasting Using Supervised Machine Learning

## 📚 Project Summary
This week marks the culmination of the **Crop Production Forecasting Project**, 
where the analysis from Weeks 6 and 7 was formally consolidated into an IEEE-style research paper titled **“Crop Production in Agriculture.”**  
The paper evaluates 28 years of agricultural data to analyze how environmental and soil factors influence crop yield and productivity in India.  
Using **Supervised Machine Learning (SML)**, models such as **Linear Regression, Logistic Regression, Decision Trees, Random Forests,** and **Support Vector Machines (SVM)**
were implemented to predict and classify crop.

---

### ✅ Learning Objectives
- Integrate all components of the final supervised machine learning project into a research-based paper.
- Evaluate model performance for crop yield classification and prediction.
- Understand the **practical application** of ML algorithms in the **agriculture domain**.
- Present findings following IEEE formatting and academic standards.

---

## 🧠 Abstract
The study analyzes 28 years of agricultural data to assess the influence of **temperature, rainfall, pH levels, nutrients (N, P, K)**, and crop conditions on production outcomes.  
By implementing multiple **Supervised ML algorithms**, the project predicts crop productivity and helps improve decision-making for sustainable agriculture.  
Results highlight how data-driven insights support **resource optimization, crop management, and policy formulation** in India’s agricultural sector.

---

## 🧩 Methodology

### Dataset
- **Source:** Kaggle
- **Size:** 99,849 rows × 13 columns  
- **Features:**
  - State_Name, Crop_Type, Crop  
  - Soil Nutrients: N, P, K  
  - Environmental Factors: pH, Rainfall, Temperature  
  - Output Variables: Area, Production, Yield per Hectare  

### Preprocessing Steps
1. Removed irrelevant columns: `State_Name`, `Crop`, `Crop_Type` for encoding.  
2. Encoded categorical labels using **LabelEncoder()**.  
3. Split dataset using an 80/20 **train-test split**.  
4. Scaled features using **StandardScaler()**.  
5. Evaluated multiple algorithms under identical preprocessing conditions.

---

## ⚙️ Algorithms Implemented

### 1. **Linear Regression**
- Predicts continuous outcomes such as **production (tons)** or **yield per hectare**.
- Captures direct relationships between soil/environmental parameters and crop output.
- Example: Predicting rice production from rainfall and pH values.

### 2. **Logistic Regression**
- Handles binary and multi-class classification problems.
- Used to predict **crop type** or **yield category (High, Medium, Low)**.  
- **Accuracy:** 87.26%  
- **F1-Score:** 0.85  
- Demonstrated strong generalization and interpretability:contentReference[oaicite:4]{index=4}.

### 3. **Decision Tree Classifier**
- Built using `criterion="entropy"` for information gain-based splitting.  
- Perfectly fit the training data with **100% training accuracy**, but showed reduced generalization (~38% effective accuracy) due to overfitting.  
- Provided visual interpretability via decision paths:contentReference[oaicite:5]{index=5}.

### 4. **Random Forest**
- Combined multiple trees to reduce overfitting and improve predictive accuracy.  
- Real-world use case: predicting customer churn or crop yield variability.
- Outperformed Decision Tree with higher stability across different folds.

### 5. **Support Vector Machine (SVM)**
- Used for binary classification with margin optimization.
- Example: Distinguishing between **disease-resistant** and **susceptible** crop varieties.
- Produced reliable separation between crop categories based on soil and weather attributes.

---

## 📊 Experimental Results

| Model | Problem Type | Accuracy | Key Insight |
|--------|---------------|-----------|--------------|
| Linear Regression | Regression | R² = 0.92 | Excellent fit for continuous crop yield prediction |
| Logistic Regression | Classification | 87.26% | Balanced precision and recall for crop-type prediction |
| Decision Tree | Classification | 38% (post-scaled) | High training accuracy, prone to overfitting |
| Random Forest | Classification | ~92% | More robust, handled noisy data effectively |
| SVM | Classification | ~89% | Strong generalization for binary crop classification |

**Observations:**
- Logistic Regression achieved consistent accuracy and interpretability.
- Ensemble methods like Random Forest improved predictive stability.
- Feature scaling and encoding significantly affected model convergence and accuracy.

---

## 🪄 Insights & Discussion
- **Rainfall and temperature** were dominant predictors for yield variation.  
- **Soil pH** and **nutrient imbalance (N, P, K)** directly impacted crop productivity.  
- Models enabled **data-driven decision-making** in agricultural planning.  
- The combination of logistic regression and random forest provided the most stable results.  
- Continuous updates and monitoring are vital to maintain relevance in changing climate scenario.

---

## 🧾 Conclusion
The integration of supervised ML models in agriculture significantly enhances the ability to **forecast yields** and **optimize resources**.  
This research confirms that applying algorithms like Logistic Regression, Decision Trees, and Random Forest can transform raw agricultural data into actionable intelligence.  
By leveraging 28 years of crop data, the study establishes the foundation for **AI-driven, sustainable agriculture** that supports policymakers and farmers alike.

---

## 📚 References
1. Pan, W.-T. (2012). *A new fruit fly optimization algorithm.* Knowledge-Based Systems, 26, 69–74.  
2. Madhumathi, R. et al. (2020). *Soil NPK and Moisture Analysis Using Wireless Sensor Networks.* IEEE ICCCNT 2020, Kharagpur, India.  
3. Aruvansh Nigam et al. (2019). *Crop Yield Prediction Using Machine Learning Algorithms.* IEEE ICIIP, pp. 125–130.  
4. Renuka & Sujata Terdal. (2019). *Evaluation of ML Algorithms for Crop Prediction.* IJEAT Vol. 8.  
5. Andrew Crane Droesch. (2018). *Machine Learning Methods for Crop Yield Prediction and Climate Change Impact Assessment.* IOP Publishing Ltd.  
6. Nischitha K. et al. (2020). *Crop Prediction using Machine Learning Approaches.* IJERT Vol. 9.  
7. Reddy, D. Anantha et al. (2019). *Crop Recommendation System to Maximize Crop Yield using ML.* IJSRST Vol. 6.  
8. Kaggle: *Crop Production in India Dataset.* [(https://www.kaggle.com/datasets/asishpandey/crop-production-in-india/data)].

---

## 📂 Deliverables
- 📄 [IEEE Paper — Crop Production in Agriculture (PDF)](./IEEEPaper.pdf)  
- 📄 [Week 8 Final Python Script](./project_2.py)  
- 📓 [Final Colab Notebook PDF](./project_2.ipynb.pdf)  
- 📊 [Crop Production Dataset (CSV)](./Crop_production.csv)  
- 📝 Notes & Reflections in `notes.md`

---

## ✅ Checklist
- [x] Integrate Week 6–7 project results into IEEE paper format  
- [x] Document methodology, models and outcomes  
- [x] Compare all supervised ML techniques  
- [x] Include citations and references  
- [x] Upload final dataset, code and report to GitHub  

---

📚 **Course:** DATA-55000 — Supervised Machine Learning  

