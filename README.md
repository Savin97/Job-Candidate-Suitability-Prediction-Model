# Job Candidate Suitability Prediction Model

## 📌 Overview
This project predicts whether a job candidate is **suitable (1)** or **not suitable (0)** for a given position based on applicant data.  
It uses statistical analysis, preprocessing pipelines, and multiple classification algorithms to build and compare predictive models.

---

## 🛠 Tech Stack
- **Language:** Python  
- **Libraries:** scikit-learn, Pandas, NumPy, Matplotlib, Seaborn  
- **Techniques:** Data cleaning, feature encoding, Logistic Regression, KNN, Random Forest, Adaboost  
- **Evaluation:** Cross-validation, ROC curves, AUC score

---

## 📂 Project Structure
```
.
├── notebooks/
│   └── Job_Candidate_Suitability_Prediction_Model.ipynb  # Main exploratory notebook
├── src/                                                  # Scripts (optional if refactored)
├── data/                                                 # Data files (not included in repo)
├── models/                                               # Saved models (gitignored)
├── reports/                                              # Plots, metrics, evaluation reports
├── requirements.txt                                      # Python dependencies
├── README.md                                             # Project documentation
└── LICENSE                                               # License file
```

---

## 🔍 Steps & Methodology
1. **Data Preprocessing**
   - Handled missing values and outliers
   - Encoded categorical variables using one-hot encoding
   - Normalized numerical features

2. **Feature Engineering**
   - Created derived features for better representation of candidate profile

3. **Model Training**
   - Trained and compared Logistic Regression, KNN, Random Forest, and MLP
   - Tuned hyperparameters via GridSearchCV

4. **Evaluation**
   - Used 5-fold cross-validation for reliability
   - Plotted ROC curves and calculated AUC scores
   - Compared performance across models

---

## 📊 Results
| Model               | Accuracy  | ROC AUC  |
|---------------------|-----------|----------|
| Logistic Regression | 0.79      | 0.909    |
| KNN                 | 0.79      | 0.865    |
| Random Forest       | **0.85**  | 0.919    |
| Adaboost            | 0.83      | **0.925**|

---

## 📈 Visualizations
- Correlation heatmap of features:

<img width="644" height="418" alt="image" src="https://github.com/user-attachments/assets/1b57e154-6240-42b9-b082-2f3d1de192a2" />


- ROC curves for all models:

<img width="1632" height="498" alt="image" src="https://github.com/user-attachments/assets/e307e9aa-f8ee-4bbf-b45f-653d0069fae5" />


- Confusion matrix for chosen model (Logistic Regression):

<img width="515" height="455" alt="image" src="https://github.com/user-attachments/assets/ce0458a4-8fb4-4d2f-a426-785cf2f4b5a8" />


---

## 🚀 How to Run
1. Clone the repository:
```bash
git clone https://github.com/Savin97/Job-Candidate-Suitability-Prediction-Model.git
cd Job-Candidate-Suitability-Prediction-Model
```

2. (Optional) Create and activate a virtual environment:
```bash
python -m venv .venv
source .venv/bin/activate   # Windows: .venv\Scripts\activate
```

3. Install dependencies:
```bash
pip install -r requirements.txt
```

4. Run the notebook:
```bash
jupyter notebook notebooks/Job_Candidate_Suitability_Prediction_Model.ipynb
```
