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



output: .............................................................

<img width="1360" height="723" alt="Image" src="https://github.com/user-attachments/assets/a0f2029f-d036-412e-a0b3-f96fdb7f0e02" />

<img width="1176" height="589" alt="Image" src="https://github.com/user-attachments/assets/8165e090-ead7-4218-9aea-e187dc736a9a" />

<img width="1179" height="488" alt="Image" src="https://github.com/user-attachments/assets/0341c492-2854-4f17-ba5b-8fb0bb4325e2" />

<img width="1355" height="656" alt="Image" src="https://github.com/user-attachments/assets/fe3da8ae-e54e-4ffd-bbbd-29d0047e40f1" />

<img width="1355" height="639" alt="Image" src="https://github.com/user-attachments/assets/1c321fc5-76a8-4f7f-8f28-e8c010be9928" />

<img width="1338" height="561" alt="Image" src="https://github.com/user-attachments/assets/a78f4fc5-cc24-47a3-b7f3-4a6a24f0a6b8" />

<img width="1287" height="623" alt="Image" src="https://github.com/user-attachments/assets/79e7866a-6eab-417b-a6a3-c34939124fba" />

<img width="1287" height="623" alt="Image" src="https://github.com/user-attachments/assets/be312743-6466-4f44-8193-32d855410ba9" />

<img width="942" height="272" alt="Image" src="https://github.com/user-attachments/assets/989e9681-b4f0-4423-a6a3-f5c05732d041" />

<img width="1360" height="317" alt="Image" src="https://github.com/user-attachments/assets/608883eb-22eb-4ebd-aebe-8ffc2cb4e9a6" />

<img width="1354" height="525" alt="Image" src="https://github.com/user-attachments/assets/b9621342-0dbb-4b35-b72d-e62107833c91" />

<img width="1360" height="611" alt="Image" src="https://github.com/user-attachments/assets/efa19cec-a502-4a6f-a9cc-84e7ff5b98b6" />

<img width="1339" height="619" alt="Image" src="https://github.com/user-attachments/assets/d4490f87-62c9-4c3e-af00-bf1f046e464b" />

<img width="1360" height="629" alt="Image" src="https://github.com/user-attachments/assets/872b7e24-e7b9-4a5f-b79f-2a89e14abc68" />
