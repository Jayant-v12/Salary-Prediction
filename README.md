
# Salary Prediction using Ensemble Learning

This project aims to predict employee salaries using ensemble learning techniques. It leverages multiple machine learning models to improve prediction accuracy based on key features like age, gender, education level, job title, and experience.

## 📁 Files in This Repository

- **`Salary_Prediction_Model.ipynb`**
  Contains all the code for data preprocessing, model training, evaluation, and visualization.

- **`salary_data.csv`**
  Dataset containing employee attributes and corresponding salaries (6,704 records).

## 📊 Dataset Overview

The dataset includes the following columns:

| Column               | Description                              |
|----------------------|-------------------------------------------|
| Age                  | Age of the employee                      |
| Gender               | Gender (Male/Female)                     |
| Education Level      | Highest qualification                    |
| Job Title            | Current role or designation              |
| Years of Experience  | Work experience in years                 |
| Salary               | Annual salary (Target variable)          |

## 🛠️ Technologies & Libraries Used

- **Python**
- **pandas, numpy** – Data handling and manipulation
- **matplotlib, seaborn** – Data visualization
- **scikit-learn** – Machine learning models and evaluation

## 🤖 Machine Learning Models Used

This project uses the following **ensemble regression models** from `scikit-learn`:

1. **Random Forest Regressor**
2. **Gradient Boosting Regressor**
3. **AdaBoost Regressor**
4. **Voting Regressor** (combination of the above)

## ⚙️ Model Evaluation Metrics

Each model was evaluated on an 80/20 train-test split using:

- **R² Score** (Coefficient of Determination)
- **MSE** (Mean Squared Error)
- **RMSE** (Root Mean Squared Error)

| Model              | R² Score | MSE          | RMSE ($) |
|--------------------|----------|--------------|----------|
| **Random Forest**  | **0.9813** | 53,254,937 | **7,298** |
| Voting Regressor   | 0.9391   | 173,519,622  | 13,173   |
| Gradient Boosting  | 0.9246   | 215,008,153  | 14,663   |
| AdaBoost           | 0.8132   | 532,515,686  | 23,076   |

## 🚀 How to Run the Project

1. Clone this repository:
   ```bash
   git clone https://github.com/Jayant-v12/Salary-Prediction.git
   ```
2. Navigate to the project folder:
   ```bash
   cd Salary-Prediction
   ```
3. Open the Jupyter Notebook:
   ```bash
   jupyter notebook Salary_Prediction_Model.ipynb
   ```

## 📈 Results Summary

The **Random Forest Regressor** delivered the best overall performance, posting the highest R² score (0.9813) and the lowest MSE/RMSE among all four models — a clean win across every metric. Years of experience was by far the strongest predictor of salary, followed by age, job title, and education level.

## 🔮 Future Scope

- Feature engineering for better model accuracy
- Real-time salary prediction with new data
- Further tuning of hyperparameters across ensemble models

## 📝 Acknowledgements

- Dataset curated for educational purposes
- Inspired by practical applications in HR analytics and data science

---
Made by [Jayant Singh](https://github.com/Jayant-v12)
