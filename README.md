# Student Stress & Burnout Prediction
## CS 210 - Data Management for Data Science | Rutgers University

## Project Overview
This project predicts student stress levels (Low/Medium/High) using academic, 
psychological, and lifestyle factors. We achieved 88.64% accuracy using an 
Ensemble Voting Classifier across 5 machine learning models.

## Datasets
- Primary: Student Stress Factors Dataset (Kaggle) — 1,100 records, 21 features
- Secondary: Student Stress Survey Dataset — 843 records, 26 features
- Both datasets stored in PostgreSQL relational database

## Technologies Used
- Python, Pandas, NumPy
- Scikit-learn, XGBoost
- PostgreSQL, SQLAlchemy
- Matplotlib, Seaborn
- Jupyter Notebook

## Models & Results
| Model | Accuracy | F1-Score |
|-------|----------|----------|
| Logistic Regression | 87.27% | 0.87 |
| Random Forest | 86.82% | 0.87 |
| SVM | 87.73% | 0.88 |
| XGBoost | 88.18% | 0.88 |
| Ensemble Voting | 88.64% | 0.89 |

## How to Run
1. Install requirements: pip install -r requirements.txt
2. Open projectfinal.ipynb in Jupyter Notebook
3. Run all cells in order

## Key Findings
- Blood pressure strongest predictor (17.5% importance)
- Sleep quality strong negative correlation with stress (-0.75)
- Self esteem strong negative correlation (-0.76)
- Feature engineering: social_vulnerability correlation 0.82
- Ensemble achieves 90% High stress recall
- False Negative rate for High stress: only 9.8%

## Dataset Journey
- Synthetic 150k dataset → 33% accuracy (random labels)
- Synthetic 1M dataset → 70% accuracy (synthetic ceiling)  
- Real survey dataset → 88.64% accuracy
