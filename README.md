# Telme

Welcome to **Telme**, a smart solution that uses **machine learning models (K-means and Logistic Regression)** to assign users to clusters and recommend the best plan based on their input. This project demonstrates a seamless **telecommunication plan recommendation engine** built with **Python, Flask, and Scikit-learn**.

---

## Table of Contents
- [Features](#features)
- [Tech Stack](#tech-stack)
- [Prerequisites](#prerequisites)
- [Installation](#installation)
- [Usage](#usage)
- [Project Structure](#project-structure)
- [How it Works](#how-it-works)

---

## Features
- **User Input Handling**: Collects user details including city, days since joining, plan changes, and current plans.
- **K-means Clustering**: Assigns the user to an appropriate cluster based on input.
- **Logistic Regression**: Recommends the ideal plan for the user.
- **Flask Backend API**: Handles form submissions and API requests.
- **Dynamic Frontend**: Corporate-styled user interface using Bootstrap.

---

## Tech Stack
- **Backend**: Python, Flask, Scikit-learn
- **Frontend**: HTML, CSS (Bootstrap), JavaScript
- **Machine Learning Models**: K-means, Logistic Regression
- **Data Handling**: Pandas, Numpy
- **Deployment**: Local development with Flask

---

## Prerequisites
Make sure you have the following installed:
- Python 3.8+
- Pip (Python package manager)
- Git (for cloning the repository)

---

## Installation

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/your-username/plan-recommendation-system.git
   cd plan-recommendation-system

2. **Create and Activate a Virtual Environment**:
   ```bash
   python -m venv .venv
   source .venv/bin/activate  # On Windows: .venv\Scripts\activate


3. **Install Dependencies**:
   ```bash
   pip install -r requirements.txt


4. **Run the Flask App**:
   ```bash
   python app.py


5. Access the App: Open your browser and visit http://127.0.0.1:5000.


## Usage
- Open the Web Interface: Enter your city, days since joining, total plan changes, and current plan selections.
- Submit the Form: The app assigns you to a cluster and recommends the ideal plan based on your input.
- View Recommendation: See the recommended plan displayed in the web interface.


## Project Structure
   ```perl
   plan-recommendation-system/
   │
   ├── templates/
   │   └── index.html               # Frontend HTML
   ├── .venv/                       # Virtual environment (ignored in Git)
   ├── app.py                       # Flask backend
   ├── FinalScript.py               # Main ML logic
   ├── requirements.txt             # Python dependencies
   ├── models/                      # Serialized ML models and encoders
   │   ├── kmeans_model.pkl
   │   ├── logistic_model.pkl
   │   ├── city_encoder.pkl
   │   ├── plan_encoder.pkl
   │   └── scaler.pkl
   └── README.md                    # Project documentation
```

## How it Works
- User Input: The user provides details such as city, days since joining, total plan changes, and selected plans.
- K-means Clustering: The user is assigned to one of three clusters.
- Logistic Regression: Based on the cluster and city, a recommended plan is generated.
- Plan Recommendation: The recommended plan is displayed on the frontend

