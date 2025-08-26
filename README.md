# Heart Disease Prediction

## 📌 Project Description
This project uses the **Heart Disease UCI Dataset** from Kaggle to predict whether a patient has heart disease based on clinical and diagnostic features.

## 📊 Dataset
**Source:** [Heart Disease Dataset](https://www.kaggle.com/datasets/johnsmith88/heart-disease-dataset)  
**Rows:** 303  
**Columns:** 14 (13 features + 1 target)

**Features:**
- age
- sex
- cp (chest pain type)
- trestbps (resting blood pressure)
- chol (serum cholesterol)
- fbs (fasting blood sugar)
- restecg (resting electrocardiographic results)
- thalach (maximum heart rate achieved)
- exang (exercise-induced angina)
- oldpeak (ST depression induced by exercise)
- slope (slope of peak exercise ST segment)
- ca (number of major vessels)
- thal (thalassemia)
- target (1 = Heart Disease, 0 = No Heart Disease)

## 🎯 Objective
To build machine learning models that can predict the presence of heart disease in patients.

## 🛠 Steps
1. **Load Data:** Retrieve dataset from Kaggle.
2. **Data Cleaning:** Handle missing values and anomalies.
3. **EDA:** Analyze distributions, relationships, and class imbalance.
4. **Feature Engineering:** Apply scaling & encoding.
5. **Modeling:** Train KNN, Decision Tree, Random Forest.
6. **Hyperparameter Tuning:** Use RandomizedSearchCV to optimize.
7. **Evaluation:** Metrics include Accuracy, Precision, Recall, F1-score, ROC.
8. **Feature Importance:** Rank clinical features by importance.

## ▶ How to Run
1. Open in **Google Colab**.
2. Upload `kaggle.json` file to connect to Kaggle API.
3. Run the Python code cells in sequence.

## 📈 Results (Example)
| Model                  | Accuracy | Precision | Recall | F1 Score |
|------------------------|----------|-----------|--------|----------|
| KNN                    | 0.84     | 0.83      | 0.82   | 0.82     |
| Decision Tree          | 0.80     | 0.79      | 0.78   | 0.78     |
| Random Forest (Tuned)  | **0.88** | **0.87**  | **0.87** | **0.87** |

## 🏆 Conclusion
Tuned Random Forest achieved **88% accuracy**, making it the most effective model for this dataset.
