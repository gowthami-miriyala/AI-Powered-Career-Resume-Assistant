# AI-Powered Career & Resume Assistant

A realistic final-year B.Tech project built with Flask, SQLite/SQLAlchemy, Bootstrap, JavaScript and practical NLP.

## Features
- Registration/login with password hashing
- Secure PDF/DOCX/TXT uploads
- Resume and JD text extraction
- TF-IDF cosine similarity
- Skill/keyword matching
- Explainable 0-100 ATS-style score
- Suggestions and learning roadmap
- Interview question generation
- Career chatbot with deterministic answers
- Analysis history
- Professional PDF report download
- Responsive Bootstrap UI
- Automated tests

## Windows + VS Code setup
```powershell
cd AI_Career_Resume_Assistant
py -m venv .venv
.venv\Scripts\activate
pip install -r requirements.txt
copy .env.example .env
python run.py
```
Open http://127.0.0.1:5000

Linux/macOS:
```bash
python3 -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
cp .env.example .env
python run.py
```

## Demo
The application includes a **Load Demo** option on the login page. It creates a demo account:
- Email: `demo@example.com`
- Password: `Demo@12345`

## ATS scoring
- Skills match: 40%
- Semantic TF-IDF similarity: 25%
- Important keyword coverage: 15%
- Education/qualification: 8%
- Experience: 7%
- Resume structure: 5%

The score is deliberately presented as an ATS-style heuristic, not a prediction of hiring.

## Testing
```powershell
pytest -q
```

## GitHub
```powershell
git init
git add .
git commit -m "Initial AI Career Resume Assistant"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/AI_Career_Resume_Assistant.git
git push -u origin main
```
Do not commit `.env`, uploaded resumes, generated reports or the local database.

## Deployment
For Render/Railway-like services, install dependencies from requirements.txt and run with a production WSGI server such as Gunicorn after adding it to requirements:
`gunicorn -w 2 run:app`
For production, use PostgreSQL, persistent object storage, HTTPS, CSRF protection and a strong secret.

## Architecture
Browser -> Flask routes -> services (parsing/NLP/reporting) -> SQLAlchemy/SQLite.

## Viva topics
Explain TF-IDF, cosine similarity, skill extraction, score weighting, password hashing, file validation, SQLAlchemy ORM, PDF parsing, Flask routing, and limitations of heuristic ATS scoring.
