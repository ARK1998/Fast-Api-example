# FastAPI Notes Management System

![FastAPI-0.104.1](https://img.shields.io/badge/FastAPI-0.104.1-informational)
![Python-3.7+](https://img.shields.io/badge/Python-3.7+-blue)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-13+-blue)
![Vue.js](https://img.shields.io/badge/Vue.js-3-green)

A modern, asynchronous REST API for notes management built with **FastAPI**, **PostgreSQL**, and **SQLAlchemy**. Features complete CRUD operations, JWT authentication, and an optional Vue.js frontend.

## 🚀 Quick Start

### Prerequisites
- Python 3.7+
- PostgreSQL
- Node.js 16+ (for frontend)
- Docker & Docker Compose (optional)

### Local Development

1. **Clone & Setup**
   ```bash
   git clone https://github.com/ARK1998/Fast-Api-example.git
   cd Fast-Api-example
   python -m venv venv
   source venv/bin/activate  # Linux/Mac
   # .\venv\Scripts\Activate.ps1  # Windows
Install Dependencies

bash
pip install -r requirements.txt
Database Setup

bash
# Create PostgreSQL database
createdb fast_api_dev
# Update DATABASE_URL in .env file
Run Application

bash
uvicorn app.main:app --reload --port 8000
Docker Deployment
bash
docker-compose up -d --build
📁 Project Structure
text
Fast-Api-example/
├── app/
│   ├── main.py              # FastAPI application
│   ├── models.py            # SQLAlchemy models
│   ├── schemas.py           # Pydantic schemas
│   ├── database.py          # Database configuration
│   └── dependencies.py      # Authentication & dependencies
├── tests/                   # Test suite
├── vue-client/              # Vue.js frontend
├── requirements.txt         # Python dependencies
└── docker-compose.yml       # Container orchestration
🔌 API Endpoints
GET /notes - Retrieve all notes

POST /notes - Create new note

GET /notes/{id} - Get specific note

PUT /notes/{id} - Update note

DELETE /notes/{id} - Delete note

GET /docs - Interactive API documentation

🛠️ Features
FastAPI with automatic OpenAPI documentation

PostgreSQL database with SQLAlchemy ORM

JWT Authentication support

Pytest test suite

Docker containerization

Vue.js 3 frontend (optional)

CORS enabled for frontend integration

🧪 Testing
bash
pytest tests/ -v
📚 Documentation
Interactive API Docs: http://localhost:8000/docs

Redoc Documentation: http://localhost:8000/redoc

Auto-generated OpenAPI schema

🌐 Frontend (Vue.js)
bash
cd vue-client
npm install
npm run dev
Frontend runs on: http://localhost:5173

🔧 Environment Variables
Create .env file:

env
DATABASE_URL=postgresql://user:password@localhost:5432/fast_api_dev
SECRET_KEY=your-secret-key
ALGORITHM=HS256
🤝 Contributing
Fork the repository

Create feature branch (git checkout -b feature/amazing-feature)

Commit changes (git commit -m 'Add amazing feature')

Push to branch (git push origin feature/amazing-feature)

Open a Pull Request

📝 License
Distributed under the MIT License. See LICENSE for more information.

👤 Author
ARK1998 - GitHub

🙏 Acknowledgments
FastAPI documentation and community

PostgreSQL team

Vue.js ecosystem

Docker community