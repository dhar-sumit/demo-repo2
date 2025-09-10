# 🚀 GitHub Actions CI/CD Demo – Python Project

This repository demonstrates how to set up a **Continuous Integration (CI) pipeline** using **GitHub Actions** for a simple Python project.

The pipeline automatically builds, tests, and validates code changes on every push or pull request to ensure code quality and reliability.


---


## 📌 Features of the Workflow

* ✅ **Triggers** on `push` and `pull_request` events to the `main` branch.
* ✅ **Environment Setup**: Installs Python 3.x and dependencies from `requirements.txt`.
* ✅ **Linting**: Runs `flake8` to check for code quality issues.
* ✅ **Testing**: Executes unit tests with `pytest` and uploads JUnit XML reports.
* ✅ **Caching**: Uses dependency caching to speed up subsequent runs.
* ✅ **Notifications**: Sends email updates on workflow status (success/failure).


---


## 📂 Project Structure

```
demo-repo2/
│── .github/
│   └── workflows/
│       └── main.yml  
│── src/
│   └── calc.py
│── tests/
│   └── test_calc.
│── .gitignore  
│── requirements.txt   
│── README.md                
```


---


## 📊 CI/CD Pipeline Overview

1. Code pushed to GitHub (`main` branch).
2. GitHub Actions workflow (`main.yml`) is triggered.
3. Pipeline runs:

   * Install dependencies
   * Run linting (`flake8`)
   * Run unit tests (`pytest`)
   * Cache dependencies
   * Notify results
4. Status is reported via GitHub UI and email notification.


---


## 🛠️ Running Locally

You can reproduce the workflow locally for quick validation.

```bash
# Create virtual environment
python -m venv .venv  

# Activate environment
# On Linux/macOS:
source .venv/bin/activate  
# On Windows:
.venv\Scripts\activate  

# Install dependencies
pip install -r requirements.txt  

# Run tests
flake8 src tests
pytest
```

---


## 📌 GitHub Actions Status

[![CI](https://github.com/dhar-sumit/demo-repo2/actions/workflows/main.yml/badge.svg)](https://github.com/dhar-sumit/demo-repo2/actions/workflows/main.yml)


---


## ✅ Key Learnings

* GitHub Actions fundamentals (triggers, jobs, steps).
* Automating build and test workflows for reliability.
* Using caching to optimize execution time.
* Integrating notifications for instant feedback.
