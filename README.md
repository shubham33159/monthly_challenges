# Monthly Challenges

Small Django project that serves a list of monthly challenges and detail pages for each month.

## Features
- Simple views and templates for an index and per-month challenge page
- Static assets under `challenges/static/`
- Template inheritance via `templates/base.html`
- Example project structure for learning Django

## Requirements
- Python 3.8+
- Django 3.x/4.x (use the version in `requirements.txt` if present)

## Quick setup (Windows)
1. Create and activate a venv
   - Command Prompt:
     ```
     python -m venv .venv
     .venv\Scripts\activate
     ```
   - PowerShell:
     ```
     python -m venv .venv
     .\.venv\Scripts\Activate.ps1
     ```
2. Install dependencies
   ```
   pip install -r requirements.txt
   ```
   If `requirements.txt` is missing:
   ```
   pip install django
   ```
3. Apply migrations
   ```
   python manage.py migrate
   ```
4. (Optional) Create superuser
   ```
   python manage.py createsuperuser
   ```
5. Run dev server
   ```
   python manage.py runserver
   ```
6. Open http://127.0.0.1:8000/

## Running tests
```
python manage.py test
```

## Project layout (important files)
- manage.py
- monthly_challenges/ (project settings, urls)
- challenges/ (app: views, urls, templates, static)
- templates/
- static/

## Suggestions / Next steps
- Add `requirements.txt` and `README` (this file)
- Move challenge data into a model and register in admin
- Add unit tests for views and templates
- Add linting/formatting (black, flake8) and CI
- Remove `db.sqlite3` from repo and add to `.gitignore`

## License
MIT (or choose your preferred license)
