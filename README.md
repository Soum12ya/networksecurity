# 🔐 Network Security - Phishing Data Detection (End-to-End ML Project)

## 🚀 Overview
This project focuses on detecting phishing websites using machine learning. It implements an end-to-end ML pipeline with AWS EC2 deployment, experiment tracking via DagsHub and MLflow, and a robust CI/CD pipeline using GitHub Actions.

## 📌 Features
- Data preprocessing and feature engineering
- Exploratory Data Analysis (EDA)
- Model training and evaluation using various ML algorithms
- Experiment tracking with **DagsHub** & **MLflow**
- API for real-time phishing detection using **FastAPI & Flask**
- Deployment on **AWS EC2**
- Dataset stored in **AWS S3** for scalability
- CI/CD pipeline with **GitHub Actions**

## 📁 Dataset
The phishing dataset is securely stored in an **AWS S3 bucket**, allowing easy access for experiments and model training.

## 📊 Tech Stack
- **Programming Language:** Python
- **Machine Learning:** Scikit-learn, XGBoost, Random Forest
- **Experiment Tracking:** DagsHub, MLflow
- **Web Framework:** FastAPI, Flask
- **Cloud Services:** AWS EC2, S3
- **CI/CD:** GitHub Actions, Docker, AWS CodePipeline

## 🔧 Setup Instructions
### 1️⃣ Clone the Repository
```sh
 git clone https://github.com/your-username/phishing-detection.git
 cd phishing-detection
```
### 2️⃣ Create and Activate a Virtual Environment
```sh
 python -m venv venv
 source venv/bin/activate   # On Windows: venv\Scripts\activate
```
### 3️⃣ Install Dependencies
```sh
 pip install -r requirements.txt
```
### 4️⃣ Set Up AWS Credentials
Ensure your AWS credentials are configured properly to access **S3** and **EC2**.
```sh
 aws configure
```

### 5️⃣ Run the Application
```sh
 uvicorn app:app --host 0.0.0.0 --port 8000   # For FastAPI
 python app.py   # For Flask
```

## 📦 CI/CD Pipeline
### ✅ Steps in the Pipeline
1. **Version Control**: GitHub repository management
2. **Automated Testing**: Pytest for unit tests
3. **Dockerization**: Containerizing the application
4. **Deployment**: Deploying on AWS EC2
5. **Experiment Tracking**: Logging models with MLflow and DagsHub
6. **Monitoring & Logging**: Using Prometheus/Grafana for insights

## 🎯 API Endpoints
| Endpoint | Method | Description |
|----------|--------|-------------|
| `/predict` | POST | Detects phishing attempts based on URL input |
| `/train` | POST | Triggers model training and logs experiments |

## 🤝 Contributing
We welcome contributions! Open issues, submit PRs, and improve the project.

## 📞 Contact
For any queries, reach out via [LinkedIn](https://www.linkedin.com/in/soumyajit-bhandary-20b348254/) or [Email](mailto:soumyajitbhandary9@gmail.com).
