# 🎓 Student Performance Indicator

An **end-to-end Machine Learning project** that predicts **students' math scores** based on various socio-economic and academic factors.  
The project demonstrates the **complete ML lifecycle** – from data collection, EDA, feature engineering, model selection, web deployment, and containerization.

---


[![Python](https://img.shields.io/badge/Python-3.12-yellow?logo=python)](https://www.python.org/) 

## 🚀 Tech Stack
- **Python, Pandas, NumPy, Scikit-learn**
- **Flask** (backend web framework)
- **HTML, CSS, Simplified JavaScript** (frontend UI)
- **CatBoostRegressor, AdaBoostRegressor, RandomForestRegressor, LinearRegression, KNeighborsRegressor, DecisionTreeRegressor, XGBRegressor**  
- **Evaluation Metrics**: `r2_score`
- **GitHub Actions** (CI/CD automation)
- **Azure Web App & AWS Elastic Beanstalk** (cloud deployment)
- **Docker** (containerization)

---

## 📂 Project Structure

├── .github/workflows      # GitHub Actions CI/CD

├── data                   # Dataset

├── notebooks              # EDA & experiments

├── src                    # ML pipeline (data ingestion, transformation, trainer)

├── templates              # HTML pages (home, form, result)

├── static                 # CSS, JS files

├── app.py                 # Flask entrypoint

├── Dockerfile             # For containerization

├── requirements.txt       # Python dependencies

└── README.md              # Project documentation


## 📌 Project Lifecycle

### 1️⃣ Understanding the Problem Statement
- Objective: Predict **students’ math scores** based on features such as:
  - Gender
  - Ethnicity
  - Parental level of education
  - Lunch type
  - Test preparation course
  - Reading score
  - Writing score

---

### 2️⃣ Data Collection
- **Dataset Source**: [Kaggle - Students Performance in Exams](https://www.kaggle.com/datasets/spscientist/students-performance-in-exams?datasetId=74977)  
- **Size**: 1000 rows × 8 columns

| gender | race_ethnicity | parental_level_of_education | lunch        | test_preparation_course | reading_score | writing_score | math_score |
|--------|---------------|-----------------------------|--------------|--------------------------|---------------|---------------|------------|
| female | group B       | bachelor's degree           | standard     | none                     | 72            | 74            | 69         |
| female | group C       | some college                | standard     | completed                | 90            | 88            | 95         |
| male   | group A       | associate's degree          | free/reduced | none                     | 57            | 44            | 49         |

---

### 3️⃣ Data Checks & Exploratory Data Analysis (EDA)
- Missing value checks
- Outlier detection
- Distribution of categorical features
- Correlation heatmap

---

### 4️⃣ Feature Engineering
- Encoding categorical variables
- Normalization where required
- Train-test split

---

### 5️⃣ Model Training & Selection
- Trained multiple ML models:
  - **CatBoostRegressor**
  - **AdaBoostRegressor**
  - **RandomForestRegressor**
  - **Linear Regression**
  - **DecisionTreeRegressor**
  - **KNeighborsRegressor**
  - **XGBRegressor**
- **Model selection** based on highest `r2_score`.

---

### 6️⃣ Deployment
- **Flask Web App** with:
  - **Home Page**
  - **Prediction Form**
  - **Result Page**
- **GitHub Actions** CI/CD pipeline for automated deployment
- Deployment Targets:
  - [Azure Web App](#) 🔹 
  - [AWS Elastic Beanstalk](#) 🔹 
- **Dockerized container** for portability

 
[![Flask](https://img.shields.io/badge/Flask-Web%20App-lightgrey?logo=flask)](https://flask.palletsprojects.com/)  

---

## 🐳 Docker Support
Build and run locally using Docker:
```bash
# Build image
docker build -t student-performance .


# Run container
docker run -p 5000:5000 student-performance
```


[![Docker](https://img.shields.io/badge/Docker-Containerized-blue?logo=docker)](https://hub.docker.com/)  


---

## ⚡ CI/CD with GitHub Actions
- Linting, testing, and deployment automated
- Push to main branch → deploys app to Azure/AWS

[![CI/CD](https://github.com/AdMub/mlproject/actions/workflows/main.yml/badge.svg)](https://github.com/AdMub/mlproject/actions)  
[![Azure](https://img.shields.io/badge/Azure-Deployed-blue?logo=microsoft-azure)](https://your-azure-webapp-url)  
[![AWS](https://img.shields.io/badge/AWS-Deployed-orange?logo=amazon-aws)](https://your-aws-app-url)  

## 📊 Results
- The best performing model was chosen based on r2_score.
- Achieved strong predictive accuracy for math scores using socio-academic features.


## 🌍 Live Demo

🔹 Home: Click Here

<img width="1880" height="1028" alt="home" src="https://github.com/user-attachments/assets/a7301fa1-b4a8-4acf-8074-3af9755d8784" />


🔹 Form: Click Here

<img width="1862" height="977" alt="form" src="https://github.com/user-attachments/assets/c0490bd8-0742-412f-a5ed-97d558666f4b" />

🔹 Result: Click Here

<img width="1920" height="703" alt="result" src="https://github.com/user-attachments/assets/977b4923-351a-42de-86e0-d70c942f4b49" />



## ✨ Key Learnings
- Full-cycle ML project workflow
- Model comparison and selection
- Flask web development
- CI/CD deployment to cloud (Azure & AWS)
- Containerization with Docker

## 🤝 Contribution
Pull requests are welcome! For major changes, please open an issue first to discuss what you would like to change.

## 📜 License
This project is licensed under the MIT License.

[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)  


