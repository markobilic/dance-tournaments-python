# Dance Tournaments (Flask)

Flask application for running dance tournaments: events, federations, disciplines, levels, age groups and categories, dancers and choreographies, start order, live judging and grades.

UI is based on the Datta Able Flask dashboard template by AppSeed (see `LICENSE.md`).

## Stack

- Flask, Flask-Login, Flask-SQLAlchemy, Flask-Migrate
- MySQL (SQLite fallback when DB settings are not provided)
- Gunicorn, Docker / nginx config included

## Setup

```bash
python -m venv env
env\Scripts\activate          # Linux/macOS: source env/bin/activate
pip install -r requirements.txt
cp env.sample .env            # set DB_* values for MySQL
flask run
```

Docker: `docker-compose up --build`
