# Python Unit Testing with GitHub Actions

## 📌Overview

This project demonstrates **unit testing in Python using Pytest** and **Continuous Integration (CI) using GitHub Actions**.

The project contains two mathematical operations:

* Addition
* Subtraction

GitHub Actions automatically runs the unit tests whenever code is pushed to the `main` or `develop` branch or when a Pull Request targets these branches.

---

## 🛠️ Technologies Used

* Python
* Pytest
* Git
* GitHub
* GitHub Actions
* YAML

---

## 📂 Project Structure

```text
project/
│
├── src/
│   ├── __init__.py
│   └── math_operation.py
│
├── test/
│   ├── __init__.py
│   └── test_operation.py
│
├── .github/
│   └── workflows/
│       └── unittest.yml
│
└── requirements.txt
```

---

## 🧮 Mathematical Operations

The `src/math_operation.py` file contains two functions:

```python
def add(a, b):
    return a + b


def subtract(a, b):
    return a - b
```

---

## 🧪 Unit Testing

The `test/test_operation.py` file contains unit tests for the addition and subtraction functions.

```python
from src.math_operation import add, subtract


def test_add():
    assert add(2, 3) == 5


def test_subtract():
    assert subtract(5, 3) == 2
```

---

## ⚙️ GitHub Actions

The CI workflow is located at:

```text
.github/workflows/unittest.yml
```

The workflow performs these steps:

```text
Git Push / Pull Request
        ↓
GitHub Actions
        ↓
Checkout Code
        ↓
Setup Python
        ↓
Install Dependencies
        ↓
Run Pytest
        ↓
Tests Pass ✅ / Fail ❌
```

---

## ▶️ Run Tests Locally

Install dependencies:

```bash
pip install -r requirements.txt
```

Run the tests:

```bash
pytest
```

---

## 🎯 What I Learned

* Python unit testing with Pytest
* Git and GitHub
* Git branches
* Pull Requests
* GitHub Actions
* YAML workflow files
* Continuous Integration (CI)
* Automated testing

---

## 🚀 Future Improvements

The CI pipeline can later be extended with:

* Docker
* Docker Hub / AWS ECR
* AWS EC2
* Continuous Deployment (CD)
* MLflow
* DVC

---

## 👨‍💻 Author

**Pratik Choudhary**

AI/ML | Generative AI | MLOps
