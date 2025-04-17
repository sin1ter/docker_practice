# 🐳 Full Stack Docker Practice

This is a full-stack practice project using **Docker** to containerize both the frontend and backend components.

## 🛠️ Tech Stack

- 🧠 **Backend**: FastAPI (Python)
- 🎨 **Frontend**: React 
- 🐋 **Docker**: Docker & Docker Compose

## 📂 Project Structure

```
fullStack_docker/
│
├── backend/           # FastAPI backend
│   ├── main.py        # Entry point for the API
│   ├── requirements.txt
│   └── Dockerfile     # Backend container configuration
│
├── frontend/          # Frontend app (e.g. React)
│   └── Dockerfile     # Frontend container configuration
│
├── docker-compose.yml # Defines services
└── .gitignore         # Ignore environment and build files
```

## 🚀 Getting Started

### Prerequisites

- Docker and Docker Compose installed on your machine
- Git (for version control)

### Installation & Running

1. Clone the repository:
   ```bash
   git clone <repository-url>
   cd fullStack_docker
   ```

2. Start the full application:
   ```bash
   docker-compose up --build
   ```
   
   This command will:
   - Build both the frontend and backend containers
   - Start the services defined in docker-compose.yml
   - Connect the containers to allow them to communicate

3. Access the applications:
   - Backend API: http://localhost:8000
   - Frontend: http://localhost:3000

## 💻 Development

### Backend (FastAPI)

- **Entry File**: `main.py`
- **Install Dependencies Locally**:
  ```bash
  cd backend
  pip install -r requirements.txt
  ```
- **Run Locally** (outside Docker):
  ```bash
  uvicorn main:app --reload
  ```
- **API Documentation** (when running):
  - Swagger UI: http://localhost:8000/docs
  - ReDoc: http://localhost:8000/redoc

### Frontend

Navigate into the frontend directory and:

- **Install Dependencies**:
  ```bash
  npm install
  ```
- **Start Development Server**:
  ```bash
  npm start
  ```




This project is intended for practice and learning Docker with full-stack applications.
