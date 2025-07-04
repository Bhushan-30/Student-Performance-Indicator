# Student Performance Prediction Web App 🎓📊

An end-to-end machine learning web application that predicts student exam scores based on demographic and academic inputs. The project includes data preprocessing, model training, Flask-based web deployment, and automated CI/CD using AWS Elastic Beanstalk and CodePipeline.

## 🚀 Features
- Predicts student performance using inputs like gender, ethnicity, parental education, lunch type, and test preparation.
- Interactive web UI built with Flask, HTML, and CSS.
- Pre-trained ML model using Scikit-learn (e.g., RandomForest or LinearRegression).
- Modular architecture with custom data pipeline and exception handling.
- Deployed on **AWS Elastic Beanstalk** with CI/CD via **GitHub + CodePipeline**.

## 🧠 Machine Learning Workflow
- Exploratory Data Analysis (EDA)
- Feature Engineering & Preprocessing (`preprocessor.pkl`)
- Model Selection and Training (`model.pkl`)
- Train/Test Split and Evaluation
- Prediction pipeline for real-time user inputs

## 📁 Project Structure

├── artifacts/ # Saved datasets and model files
│ ├── model.pkl
│ ├── preprocessor.pkl
│ ├── train.csv / test.csv
├── notebook/ # Jupyter notebooks for EDA and model training
│ ├── 1.EDA_Student_Performance.ipynb
│ └── 2.Model_Selection.ipynb
├── src/
│ └── pipeline/ # Custom ML pipeline scripts
│ └── components/ # Data ingestion, transformation, model training
├── static/ # CSS styling
│ └── style.css
├── templates/ # HTML templates
│ ├── index.html
│ └── home.html
├── application.py # Flask entry point
├── requirements.txt
├── setup.py
├── .ebextensions/ # AWS EB config


## ☁️ Deployment
- **Platform**: AWS Elastic Beanstalk (Python environment)
- **CI/CD**: AWS CodePipeline connected to GitHub (main branch)
- **Trigger**: Auto deployment on every push to GitHub


## 🛠 Tech Stack
- Python, Flask, Pandas, NumPy, Scikit-learn
- HTML, CSS (Jinja2 Templates)
- AWS Elastic Beanstalk, EC2
- GitHub, CodePipeline, Git

