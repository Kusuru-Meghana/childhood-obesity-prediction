# Childhood Obesity Prediction  
**Predicting childhood obesity using 2020 NSCH data**

---

## 📌 Project Overview  
The goal of this project is to use data from the **2020 National Survey of Children's Health (NSCH)** to predict whether children aged 10–17 are **overweight or obese** based on their lifestyle, demographic, and family characteristics.

---

## 💡 Why This Matters  
Childhood obesity is a major public health concern linked to long-term health problems such as **diabetes, heart disease, and mental health issues**.  
Understanding which factors are most associated with higher BMI can help inform **prevention strategies** and guide interventions at both family and policy levels.

---

## 📊 Dataset Information  

- **Source**: U.S. Census Bureau & HRSA Maternal and Child Health Bureau  
- **Year**: 2020  
- **Total respondents**: ~42,777 children nationwide  
- **Target group for this project**: Children aged **10–17 years**  
- **Target variable**: `BMICLASS` (BMI category based on parent-reported height/weight)  

| Value | Meaning |  
|-------|----------|  
| 1     | Underweight (<5th percentile) |  
| 2     | Normal (5th–84th percentile) |  
| 3     | Overweight (85th–94th percentile) |  
| 4     | Obese (≥95th percentile) |  

For modeling, this was simplified into a **binary classification problem**:  
- `0` → Underweight or Normal  
- `1` → Overweight or Obese  

---

## 🔍 Methods  

1. **Exploratory Data Analysis (EDA)**  
   - Distribution of obesity rates across age, sex, household language, and lifestyle factors.  
   - Visualizations using `matplotlib` and `seaborn`.  

2. **Feature Engineering & Preprocessing**  
   - Filtering valid rows (age 10–17, valid BMI values).  
   - Handling missing/special codes.  
   - Creating binary target variable `ObeseBinary`.  

3. **Modeling**  
   - Machine learning models (e.g., Logistic Regression, Random Forest, XGBoost).  
   - Train-test split and evaluation metrics (accuracy, precision, recall, F1).  

4. **Evaluation**  
   - Compared model performance.  
   - Identified most important predictors of obesity.  

---

## 📈 Results (Summary)  
- Lifestyle factors like **physical activity, screen time, and sleep** were strongly associated with obesity.  
- Socio-demographic factors such as **income level and household language** also played a role.  
- The best-performing model achieved **X% accuracy** and provided insights into the most predictive features.  

---

## ⚙️ How to Run  

1. Clone this repository:  
   ```bash
   git clone https://github.com/Kusuru-Meghana/childhood-obesity-prediction.git
   cd childhood-obesity-prediction
