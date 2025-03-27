# FastAPI Test Project

This project is a test automation setup for a FastAPI application, integrating GitHub Actions for continuous testing.

## 🚀 Project Overview
- Uses **FastAPI** for building APIs.
- Implements **pytest** for test automation.
- Configured **GitHub Actions** for automated testing.

---
## 🛠 Setup Instructions
### 1️⃣ Clone the Repository
```bash
git clone https://github.com/anisha992/Fastapi-Test-Project.git
cd Fastapi-Test-Project
```

### 2️⃣ Create & Activate Virtual Environment
```bash
python -m venv venv
# Activate the environment:
# Windows:
venv\Scripts\activate
# macOS/Linux:
source venv/bin/activate
```

### 3️⃣ Install Dependencies
```bash
pip install -r requirements.txt
```

### 4️⃣ Run the FastAPI Server
```bash
uvicorn main:app --reload
```

The API will be available at: [http://127.0.0.1:8000](http://127.0.0.1:8000)

---
## ✅ Running Tests
### Using Pytest Locally
```bash
pytest testAutomationPytest.py
```

To collect tests without running:
```bash
pytest --collect-only
```

---
## 🔄 GitHub Actions: CI/CD Setup
This project includes **GitHub Actions** for automated testing.

### Workflow File: `.github/workflows/test.yml`
- Runs **pytest** automatically on every push.
- Ensures code quality before merging.

To trigger GitHub Actions manually:
1. Push changes to GitHub:
   ```bash
   git add .
   git commit -m "Added new test cases"
   git push origin main
   ```
2. Check workflow runs in **GitHub Actions tab**.

---