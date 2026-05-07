# 🚀 Setup Instructions

## Prerequisites

### Install uv
```bash
pip install uv
```

### Activate virtual environment
**Windows:**
```bash
.\.venv\Scripts\activate
```
**macOS/Linux:**
```bash
source .venv/bin/activate
```

### Install dependencies
```bash
uv pip install -e .
```

---

## 🐳 Running with Docker (Recommended)

### Step 1: Build the Docker image
```bash
docker compose build
```

### Step 2: Start the containers
```bash
docker compose up
```

### Step 3: Access the API
- FastAPI Swagger UI → http://localhost:8081/docs

---

## 💻 Running Locally (Without Docker)

```bash
cd backend
uvicorn app.main:app --host 0.0.0.0 --port 8081
```

---

## 🌿 Git Workflow

### Step 1: Create a new branch
```bash
git checkout -b SCRUM-7
```

### Step 2: Stage your changes
```bash
git add .
```

### Step 3: Commit with a meaningful message

| Type | Command |
|------|---------|
| New feature | `git commit -m "feat(SCRUM-7): description"` |
| Bug fix | `git commit -m "fix(SCRUM-7): description"` |
| Refactor | `git commit -m "refactor(SCRUM-7): description"` |

### Step 4: Push to remote
```bash
git push -u origin SCRUM-7
```

### Step 5: Clean up after merging
```bash
git branch -d SCRUM-7
```