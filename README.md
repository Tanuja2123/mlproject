# Machine Learning Project – End-to-End Deployment

This repository contains an end-to-end implementation of a Machine Learning project, including data preprocessing, model training, evaluation, and deployment using a Flask web application. It follows a modular and structure suitable for real-world projects.

## 🔍 Project Overview

The project demonstrates the full cycle of a machine learning pipeline:
- Collecting and processing data
- Building and evaluating ML models
- Creating reusable components (e.g., data transformation, model prediction)
- Saving models and preprocessing pipelines
- Building a Flask API for model inference
- Packaging with proper project structure and automation

## 🗂️ Project Structure

mlproject/
│
├── artifacts/ # Stores artifacts like models, preprocessed data
├── src/
│ └── mlproject/ # Core source code
│ ├── components/ # Data transformation, model training modules
│ ├── pipelines/ # Training pipeline
│ ├── utils.py # Utility functions
│ ├── logger.py # Logging setup
│ └── exception.py # Custom exception class
│
├── app.py # Flask app for prediction
├── templates/ # HTML templates for UI
│
├── notebook/ # Jupyter notebooks for initial exploration
│
├── requirements.txt # Python dependencies
├── setup.py # Package configuration
├── README.md # Project documentation


## ⚙️ How to Run the Project

### 1. Clone the Repository

```bash
git clone https://github.com/Tanuja2123/mlproject.git
cd mlproject

python -m venv venv
source venv/bin/activate     # On Windows: venv\Scripts\activate

pip install -r requirements.txt

python app.py 

🧠 Technologies Used
Python

Scikit-learn

Pandas, NumPy

Flask

HTML/CSS (for frontend)

Pickle (for model serialization)

📁 Key Files Explained
app.py: Starts the Flask app, handles routes, and predicts user input.

training_pipeline.py: Orchestrates data transformation and model training.

utils.py: Common utility functions like saving/loading objects.

logger.py / exception.py: For effective debugging and traceability.

templates/index.html: User interface for input submission.

artifacts/: Stores trained model and preprocessing files.


✨ Features
Modular design following clean code principles.

Logs and custom exceptions to make debugging easier.

Web-based UI for real-time prediction.

Easily extensible to different ML models or datasets.
