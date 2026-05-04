# Student Stress & Burnout Prediction
## CS 210 - Data Management for Data Science | Rutgers University

## Project Overview
This project predicts student stress levels (Low/Medium/High) using academic, 
psychological, and lifestyle factors using machine learning.
We achieved 88.64% accuracy using an Ensemble Voting Classifier.

## Dataset
- Source: Student Stress Factors Dataset (Kaggle)
- 1,100 records, 21 features
- Target variable: stress_level (0=Low, 1=Medium, 2=High)

## Technologies Used
- Python, Pandas, NumPy
- Scikit-learn, XGBoost
- PostgreSQL, SQLAlchemy
- Matplotlib, Seaborn
- Jupyter Notebook

## Models & Results
| Model | Accuracy |
|-------|----------|
| Logistic Regression | 87.27% |
| Random Forest | 86.82% |
| SVM | 87.73% |
| XGBoost | 88.18% |
| Ensemble Voting | 88.64% |

## How to Run
1. Install requirements: pip install -r requirements.txt
2. Open burnout_final.ipynb in Jupyter Notebook
3. Run all cells in order

## Key Findings
- Blood pressure is the strongest predictor of stress (17.5% importance)
- Sleep quality shows strong negative correlation with stress (-0.75)
- Self esteem shows strong negative correlation with stress (-0.76)
- Future career concerns strongly predict high stress (0.74)
