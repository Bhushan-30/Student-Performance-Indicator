# 🎓 Student Performance Prediction Web App

An interactive **Flask-based machine learning web application** that predicts student exam performance based on demographic and academic attributes.

Deployed on **AWS Elastic Beanstalk** with a **CI/CD pipeline** using **GitHub and AWS CodePipeline**.



## 🛠️ Project Overview

This project allows users to:

- Input student data (e.g., gender, ethnicity, lunch type, parental education).
- Run predictions using a trained **machine learning model**.
- View predicted scores for reading and writing performance.
- Use a **web interface** for live interaction.
- Benefit from automatic deployment with **CI/CD integration** via AWS.

Built with a modular structure for scalability and maintainability, and follows best practices for MLOps and deployment.

---

## 📂 Files and Structure

├── artifacts/                  # Trained models and preprocessor  
│   ├── model.pkl  
│   ├── preprocessor.pkl  
│   ├── train.csv / test.csv  
├── notebook/                   # Jupyter notebooks for EDA and model training  
│   ├── 1.EDA_Student_Performance.ipynb  
│   └── 2.Model_Selection.ipynb  
├── src/  
│   ├── pipeline/               # ML pipeline logic  
│   └── components/             # Data ingestion, transformation, model training  
├── static/                     # CSS styling  
│   └── style.css  
├── templates/                  # HTML templates  
│   ├── index.html  
│   └── home.html  
├── application.py              # Flask app entry point  
├── requirements.txt            # Python dependencies  
├── setup.py                    # Package setup  
├── .ebextensions/              # AWS Elastic Beanstalk environment config  

---

## 🚀 Getting Started

### Prerequisites

- Python 3.x
- pip (Python package manager)
- AWS account (for deployment)
- GitHub repository

### Installation (Local)

1. Clone the repository:
git clone https://github.com/your-username/student-performance-predictor.git
cd student-performance-predictor


2. Create and activate virtual environment:
python -m venv venv
source venv/bin/activate # Linux/macOS
venv\Scripts\activate # Windows


3. Install dependencies:
pip install -r requirements.txt


4. Run the app:
python application.py


Then open `http://localhost:5000` in your browser.

---

## 🧠 Machine Learning Workflow

- Performed **EDA** and feature analysis in Jupyter Notebooks.
- Applied **data preprocessing** using pipelines (encoding, scaling).
- Trained model using **Scikit-learn** (e.g., Random Forest or Linear Regression).
- Serialized model and preprocessor using `joblib`/`pickle` into `artifacts/`.
- Deployed prediction pipeline to serve real-time results in the web app.

---

## ☁️ AWS Deployment Overview

- **Platform**: AWS Elastic Beanstalk (Python environment).
- **CI/CD**: Configured using **AWS CodePipeline**.
- **Source**: GitHub (connected via GitHub App).
- **Trigger**: Auto deployment on push to `main` branch.
- **Environment Configuration**: Managed via `.ebextensions`.

---

## 🌐 Features

- 🔍 User input through a clean and simple form (Flask + HTML).
- 🧠 Real-time ML inference on form submission.
- 💾 Modular design using custom classes and pipeline architecture.
- 🔄 Auto-deployment using GitHub commits.
- 📊 Data analysis and model selection via Jupyter notebooks.

---

## 📌 Notes

- Be sure to upload your `model.pkl` and `preprocessor.pkl` before deployment.
- Customize the HTML (e.g., `home.html`) for a better UI/UX.
- Logs and errors are handled using `logger.py` and `exception.py`.

---

## ✨ Future Enhancements

- Add visualization of predictions or input distributions.
- Add support for batch predictions using file uploads (e.g., CSV).
- Extend to multi-subject predictions (Math, Reading, Writing separately).
- Use Docker for more portable deployment.

---

## 🤝 Contributing

Contributions are welcome! Feel free to fork the repo, open an issue, or submit a pull request.

---

## 🧠 Author

👤 Bhushan Deshmukh  
📨 bsdeshmukh98@gmail.com  
🔗 https://github.com/Bhushan-30


