# Student Stress Level Prediction

This project predicts **student stress levels (0, 1, 2)** using machine learning.  
It covers data exploration, statistical analysis, and model building with Logistic Regression.

---

## 📊 Dataset
- **Rows:** 1,100  
- **Columns:** 21 (all numeric)  
- **Target:** `Stress Level`  
- **No missing values / no duplicates**

Main features include:  
Anxiety Level, Self Esteem, Mental Health History, Depression, Headache, Blood Pressure, Sleep Quality, Breathing Problem, Noise Level, Living Conditions, Safety, Basic Needs, Academic Performance, Study Load, Teacher Student Relationship, Future Career Concerns, Social Support, Peer Pressure, Extracurricular Activities, Bullying.

---

## 🔎 Key Insights
- Balanced target classes:  
  - Stress Level 0 → 373  
  - Stress Level 1 → 358  
  - Stress Level 2 → 369  

- **Strong positive correlations with Stress Level:**  
  Anxiety (0.74), Depression (0.73), Bullying (0.75), Career Concerns (0.74), Peer Pressure (0.69), Headache (0.71)  

- **Strong negative correlations with Stress Level:**  
  Self Esteem (-0.76), Sleep Quality (-0.75), Safety (-0.71), Basic Needs (-0.71)  

- **VIF check:** all < 10 → no severe multicollinearity.

---

## 🤖 Model
- **Algorithm:** Logistic Regression  
- **Train Accuracy:** 0.91  
- **Test Accuracy:** 0.89  

### Classification Report (Test)
| Class | Precision | Recall | F1 | Support |
|-------|-----------|--------|----|---------|
|   0   |   0.90    | 0.87   |0.89|   95    |
|   1   |   0.88    | 0.89   |0.89|   92    |
|   2   |   0.90    | 0.92   |0.91|   88    |
| **Overall** | | | **Acc = 0.89** | 275 |

### Confusion Matrix
|        | Pred 0 | Pred 1 | Pred 2 |
|--------|--------|--------|--------|
| True 0 |   83   |   7    |   5    |
| True 1 |   6    |   82   |   4    |
| True 2 |   3    |   4    |   81   |

---

## 🛠 Tech Stack
- Python  
- pandas, numpy  
- seaborn, matplotlib  
- scikit-learn  
- statsmodels  

---

## 🚀 How to Run
1. Clone repo & go inside  
   ```bash
   git clone <repo-url>
   cd <repo-folder>```
   
###Install requirements:
```bash
pip install -r requirements.txt
```

Open and run `Notebook.ipynb` in **Jupyter Notebook** or **Google Colab**.

---

## 📌 Learnings
- Stress is influenced by **psychological, academic, and social factors together**.  
- Improving **sleep, self-esteem, and support systems** can help reduce stress.  
- Logistic Regression provides a strong baseline with **≈90% accuracy**.  

---

## 📧 Contact
**Author:** Sai Subba Rao Mahendrakar
**Email:** sai.subbu.in@gmail.com

