## End to End MAchine Learning Project
# Student Performance Prediction using Machine Learning

This project predicts **students' exam performance** (math, reading, writing scores) using multiple regression models.  
The dataset is taken from Kaggle:  
[Students Performance in Exams](https://www.kaggle.com/datasets/spscientist/students-performance-in-exams)

---

## Dataset

- **Shape:** 1000 rows × 8 columns  
- **Features:** Gender, Race/Ethnicity, Parental Education, Lunch, Test Preparation Course  
- **Target:** Math/Reading/Writing scores  

---

## Project Workflow

1. **Data Ingestion** – Load dataset from `data/`  
2. **Exploratory Data Analysis (EDA)** – Visualize distributions, correlations  
3. **Data Preprocessing** – Handle categorical encoding, missing values, train-test split  
4. **Model Training** – Train multiple regression models  
5. **Evaluation** – Compare models using **R² score**  

---

## Model Performance

| Model Name              | R² Score |
|--------------------------|----------|
| **Ridge Regression**     | **0.8806** |
| Linear Regression        | 0.8803   |
| CatBoost Regressor       | 0.8516   |
| AdaBoost Regressor       | 0.8498   |
| Random Forest Regressor  | 0.8473   |
| Lasso Regression         | 0.8253   |
| XGBoost Regressor        | 0.8216   |
| K-Neighbors Regressor    | 0.7838   |
| Decision Tree Regressor  | 0.7603   |

**Best Model:** Ridge Regression (R² = 0.8806)  

<p align="center">
  <img src="results/model_comparison.png" alt="Model Comparison" width="500"/>
</p>

---

## Tech Stack

- **Language:** Python 3  
- **Libraries:** Pandas, NumPy, Scikit-learn, CatBoost, XGBoost, Matplotlib, Seaborn  
- **Environment:** Jupyter Notebook + VS Code  

---

## How to Run

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/student-performance-ml.git
   cd student-performance-ml
2. **Create a virtual environment**
   ```bash
   python -m venv venv
3. **Install dependencies**
   ```bash
   pip install -r requirements.txt
4. **Run the Pipeline** 
   ```bash
   python src/pipelines/train_pipeline.py


## Results

**Ridge Regression** achieved the highest accuracy with an **R² score of 0.8806**.
