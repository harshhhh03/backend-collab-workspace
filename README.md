# Backend Collaborative Workspace (FastAPI)

This project is a backend service for a real-time collaborative workspace, built as part of the PurpleMerit Backend Developer Assessment.

The focus of this implementation is on backend architecture, API design, real-time communication concepts, and cloud-ready deployment.

---

## Tech Stack
- Backend Framework: FastAPI (Python)
- API Documentation: Swagger (OpenAPI)
- Real-Time Communication: WebSocket (FastAPI)
- Deployment: Render (Cloud Platform)
- Version Control: GitHub

---

## Features Implemented
- Health check API
- REST API structure (API-first design)
- WebSocket endpoint for real-time collaboration events
- Swagger-based API documentation
- Cloud deployment with public access

---

## Project Structure
backend-collab-fastapi/
│
├── main.py
├── requirements.txt
├── README.md
└── .env.example

## How to Run Locally

pip install -r requirements.txt
uvicorn main:app --reload
Access:

API: http://127.0.0.1:8000

Swagger Docs: http://127.0.0.1:8000/docs

Live Deployment
Live URL:
https://backend-collab-workspace.onrender.com
Design Decisions & Trade-offs
FastAPI was chosen for its performance, async support, and built-in OpenAPI documentation.

WebSocket support demonstrates real-time collaboration capability.
Background jobs and message queues are conceptually designed but not fully implemented due to serverless deployment constraints.
The system is designed to be horizontally scalable in a containerized or VM-based environment.

Scalability Considerations

Stateless API design allows horizontal scaling.
WebSocket connections can be distributed using a message broker (Redis/Kafka) in production.
Database and background workers can be added as separate services.

Future Improvements

JWT authentication & role-based access control
Project/workspace management APIs
Background job processing with Redis/Celery
Database integration (PostgreSQL + Redis)

Author
Harsh Kharje
GitHub: https://github.com/harshhhh03
