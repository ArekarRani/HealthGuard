# HealthGuard

HealthGuard is an AI-powered early disease detection and patient support system built with Flask. It combines X-ray analysis, medical reporting, dashboards for different user roles, and chatbot-style assistance to help support early screening workflows.

## Features
- AI-based X-ray prediction with heatmap generation for explainability
- Patient, doctor, admin, and Asha worker role-based dashboards
- Secure login, registration, and profile management
- Medical report generation in PDF format
- Medicine recommendation and chatbot support
- SQLite-ready setup for local development

## Tech Stack
- Backend: Python, Flask, Flask-SQLAlchemy
- Frontend: HTML, CSS, JavaScript
- AI/ML: TensorFlow, NumPy, OpenCV, Pillow
- Database: SQLite by default, MySQL-compatible options available
- Reports: FPDF

## Project Structure
- `app/` - Flask application package, routes, models, templates, and utilities
- `Accuracy_model/` - Model assets and training-related files
- `static/` - Static assets such as CSS, JavaScript, and images
- `uploads/` - Uploaded images and generated files
- `run.py` - Application entry point
- `requirements.txt` - Full dependency list

## Setup
### 1. Clone the repository
```powershell
git clone https://github.com/<your-username>/healthguard.git
cd healthguard
```

### 2. Create and activate a virtual environment
```powershell
py -3.11 -m venv .venv
.venv\Scripts\Activate.ps1
```

### 3. Install dependencies
```powershell
python -m pip install --upgrade pip
pip install -r requirements.txt
```

If you want a lighter local install for basic testing, use `requirements-minimal.txt` instead.

### 4. Run the app
```powershell
python run.py
```

Then open:

```text
http://localhost:3000
```

## Demo Accounts
These credentials are defined in `app/config.py` for development:
- Admin: `admin` / `admin123`
- Doctor: `doctor` / `doctor123`
- Asha worker: create through the signup page or project-specific setup

## Notes
- Python 3.11 is recommended for best compatibility with the current dependency set.
- The project uses a SQLite database by default, so it runs locally without extra database setup.
- If ML model loading is disabled during development, the UI can still be explored without the full TensorFlow workflow.

## Disclaimer
HealthGuard is a decision-support project and is not a substitute for professional medical advice, diagnosis, or treatment.
 
