# 🩺 Diabetes Risk: Predictive & Prescriptive Analytics

### Transforming CDC Health Data into Actionable Clinical Insights

![Python](https://img.shields.io/badge/Python-3.8%2B-blue?logo=python&logoColor=white)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-F7931E?logo=scikit-learn&logoColor=white)
![TensorFlow](https://img.shields.io/badge/TensorFlow-FF6F00?logo=tensorflow&logoColor=white)
![XGBoost](https://img.shields.io/badge/XGBoost-eb8a24?logo=XGBoost&logoColor=white)

## Project Overview
Diabetes is a global health crisis, yet many cases are preventable through early detection. Using a massive dataset of **253,680 individuals** (CDC BRFSS 2015), this project identifies high-risk candidates and provides **Prescriptive Recommendations** based on American Diabetes Association (ADA) standards.

---

## Business Question:
**How do lifestyle choices and physical health indicators correlate with diabetes risk?**


## Dataset Information
* **Dataset:** CDC Diabetes 012 Health Indicators BRFSS 2015
* **Source:** [UCI Machine Learning Repository](https://archive.ics.uci.edu/dataset/891/cdc+diabetes+health+indicators)
* **Size:** 253,680 instances with 21 health-related features
* **Type:** Behavioral Risk Factor Surveillance System (BRFSS) telephone survey data

---


## Why This Project Stands Out
While many models focus solely on accuracy, our team prioritized **clinical interpretability** and **Recall**:
* **Prescriptive Logic:** We didn't just stop at a "0 or 1" prediction; we built logic to offer health advice based on a patient's unique risk profile (Low, Medium, High).
* **Advanced Feature Selection:** We used **Sequential Forward Selection (SFS)** to find the most impactful predictors, moving beyond basic correlation.
* **Recall-Optimized:** In healthcare, a "False Negative" (missing a sick patient) is dangerous. Our model is tuned to capture as many at-risk individuals as possible.



---


## Performance & Key Insights
### The Winning Architecture
| Model | F1-Score | Accuracy | Best For... |
| :--- | :--- | :--- | :--- |
| **Logistic Regression + SFS** | **0.746** | 74.08% | **Clinical Interpretability** |
| Random Forest | 0.734 | 73.06% | Capturing Non-Linearity |
| Neural Network (MLP) | 0.615 | 71.26% | Complex Feature Interaction |

### Top 4 Risk Indicators
Our analysis identified these as the primary drivers of diabetes risk:
1. **High Blood Pressure** (Strongest correlation)
2. **High Cholesterol**
3. **BMI (Body Mass Index)**
4. **Physical Mobility** (Difficulty walking/climbing stairs)



---

## Technical Workflow
1. **Data Wrangling:** Cleaned survey responses, handled missing values, and addressed class imbalances.
2. **EDA:** Analyzed 21 features across demographics, lifestyle, and pre-existing conditions.
3. **Modeling:** Comparative study of traditional ML vs. Deep Learning.
4. **Implementation:** Developed a prescriptive framework using CDC and National Library of Medicine guidelines.

---

## Repository Structure
* `diabetes_dataanalytics.ipynb`: Full Python pipeline (Cleaning → EDA → Modeling).
* `Diabetes Predictor.pdf`: Business-focused presentation of results and prescriptive logic.
* `README.md`: Professional documentation.

---

## The Development Team
* **Yi-Fang Chung** – Data Visualization & ML & Modeling
* **Thi Nguyet Anh Che (Andrea)** – Project Coordination & ML 
* **Quan Pham** – Data Engineering & EDA
* **Kaveh Jalilian** – Statistical Analysis & Modeling


---

## Future Roadmap
- [ ] **Wearable Integration:** Syncing real-time heart rate and activity data.
- [ ] **HbA1c Incorporation:** Adding clinical biomarker data for higher precision.
- [ ] **Deployment:** Wrapping the model in a Streamlit or Flask web application for patient self-assessment.

---
*This project was developed for educational purposes using the CDC Diabetes Health Indicators Dataset.*
