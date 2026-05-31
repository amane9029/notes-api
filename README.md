# Notes API

A simple CRUD Notes API built with FastAPI + MySQL.

## Endpoints

| Method | Endpoint | Description |
|--------|----------|-------------|
| GET | / | Health check |
| GET | /notes | Get all notes |
| POST | /notes | Create a note |
| GET | /notes/{id} | Get a note by ID |
| PUT | /notes/{id} | Update a note |
| DELETE | /notes/{id} | Delete a note |

## Setup on CloudPanel

1. Clone the repo into your site directory
2. Create a virtual environment:
   ```bash
   python3 -m venv venv
   source venv/bin/activate
   ```
3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
4. Copy `.env.example` to `.env` and fill in your DB credentials:
   ```bash
   cp .env.example .env
   ```
5. Run with uvicorn:
   ```bash
   uvicorn main:app --host 0.0.0.0 --port 8000
   ```

## Docs
Visit `/docs` for the auto-generated Swagger UI.
