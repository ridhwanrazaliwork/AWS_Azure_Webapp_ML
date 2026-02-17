# Student Performance Prediction - Data Science Web Application

A machine learning project that predicts student exam performance based on various demographic and educational factors. The model is deployed as a web application using Flask, with infrastructure on AWS and Azure.

## Dataset

**Source:** [Kaggle - Students Performance in Exams](https://www.kaggle.com/datasets/spscientist/students-performance-in-exams)

The dataset includes student performance data across math, reading, and writing scores, along with features such as:
- Gender
- Race/Ethnicity
- Parental Level of Education
- Lunch Type (standard/free-reduced)
- Test Preparation Course Completion

## Project Structure

```
├── notebook/              # Jupyter notebooks (EDA, Model Training)
├── src/                   # Source code for ML pipeline
├── templates/             # Flask web app templates
├── requirements.txt       # Python dependencies
├── setup.py              # Project setup configuration
└── data/                 # Dataset location
```

## Tech Stack

**Machine Learning & Data Processing:**
- Pandas, NumPy
- Scikit-learn, CatBoost, XGBoost
- Matplotlib, Seaborn (visualization)

**Web Application:**
- Flask (Python web framework)

**Deployment:**
- **AWS:**
  - Elastic Beanstalk (application hosting)
  - EC2 (compute instances)
- **Azure:** Web application frontend/services

## Deployment Overview

### What is AWS Beanstalk?
AWS Elastic Beanstalk is a Platform-as-a-Service (PaaS) that automatically handles application deployment, scaling, and infrastructure management. You upload your code, and Beanstalk takes care of the rest—no need to manually manage EC2 instances, load balancers, or databases. It simplifies deployment of web applications.

### Architecture
- **AWS Beanstalk** manages the Flask application deployment and auto-scaling
- **EC2 instances** run the application behind the scenes (managed by Beanstalk)
- **Azure** hosts the web frontend or additional services
- Docker containers may be used for consistent deployment (ECR - Elastic Container Registry integration pending)

## Installation

```bash
# Clone the repository
git clone <repo-url>

# Install dependencies
pip install -r requirements.txt

# Install the project in development mode
pip install -e .
```

## Usage

### Run Locally
```bash
python app.py
```

### Run Notebooks
Navigate to the `notebook/` folder and open the Jupyter notebooks for data exploration and model training.

## Next Steps

- [ ] Complete AWS Beanstalk deployment configuration
- [ ] Finalize Azure integration
- [ ] Set up CI/CD pipeline
- [ ] Add Docker containerization (if using ECR)
- [ ] Add comprehensive API documentation

## Author
Ridhwan (ridhwanrazaliwork@gmail.com)


## Reference
MLOPS Udemy course from Krish Naik
---
*More details to be added as project development progresses.*
