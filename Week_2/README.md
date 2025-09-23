# Week 02 — Decision Rules and Posterior Probabilities

## 📚 Topics Covered:
- Decision Rules with Loss Functions
- Posterior Probability Calculation
- Decision Making with Reject Action
- Support and Confidence in Association Rules

---

### ✅ Learning Objectives:
- Understand **decision rules** and their role in classification problems.
- Work with **loss functions** in decision-making, particularly in a two-class, two-action problem.
- Apply **posterior probabilities** to decide the most likely class in a given sample.
- Learn to use **decision rules with reject** to handle uncertain or borderline cases.
- Calculate **support and confidence** for association rules.

---

### 📝 Key Concepts & Explanations:
1. **Optimal Decision Rule**  
   Given loss values (λ values) for a two-class, two-action problem, the optimal decision rule helps determine the best class based on minimizing the loss.  
   The rule can be defined as:  
   R(𝞪1/X) = 12(1 - P(C1/X))
   R(𝞪2/X) = 5 * P(C1/X)

The decision rule:  
- **Choose 𝞪1** if \( P(C1/X) > \frac{12}{17} \)
- **Choose 𝞪2**

2. **Adding the Reject Option**  
Introducing a third action (reject) changes the decision rule to provide an option to **reject** if the probability does not clearly favor 𝞪1 or 𝞪2.  
- **Choose reject (𝞪r)** if the conditions for 𝞪1 or 𝞪2 are not met.

3. **Posterior Probabilities**  
For a given new sample (e.g., x = -0.1), calculate the posterior probability for each class.  
**Posterior Probability Calculation**:
P(C1/X) = 0.652
P(C2/X) = 1 - P(C1/X) = 0.348

This indicates that class C1 is more probable and should lead to choosing 𝞪1.

4. **Interpreting Results with Reject**  
When adding a **reject** option:
- **Choose 𝞪1** if \( P(C1/X) > 0.91 \)
- **Choose 𝞪2** if \( P(C2/X) < 0.2 \)
- If neither condition is met, **reject (𝞪r)**.

5. **Support and Confidence in Association Rules**  
- **Support**: The frequency with which a rule occurs in the dataset.
- **Confidence**: The likelihood of the rule being true given the antecedent.
Example:
- **Rule**: `broccoli -> rice`  
  - Support = 2/7 (2 out of 7 customers bought both broccoli and rice)
  - Confidence = 2/5 (2 out of 5 customers who bought broccoli also bought rice).

---

### 📊 Week 2 Results:
- The decision rule for a **two-action problem** showed how loss functions influence action choices.
- **Posterior probabilities** calculation helped solidify understanding of class predictions.
- The **reject option** proved valuable in situations with uncertain data.
- **Support and Confidence** values gave insights into item associations in market basket analysis.

---

### 📂 Deliverables:
- 📄 [Week 2 Assignment PDF](./assignment.pdf)
- 📝 Notes and reflections in `notes.md`

---

### 🔖 Reflections:
- This week reinforced my understanding of decision-making frameworks, especially in the presence of multiple outcomes.
- The **reject decision rule** is practical for real-world situations where you don’t want to commit to a decision without strong evidence.
- I learned the importance of calculating **posterior probabilities** for more informed decision-making and evaluating model performance in classification tasks.

---

### ✅ Checklist:
- [x] Upload Week 2 assignment

---

## 📂 Repository Structure:
