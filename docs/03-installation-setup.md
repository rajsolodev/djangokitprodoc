# Installation & Local Setup

## Requirements

- Python 3.10+
- PostgreSQL / MySQL / SQLite
- Virtualenv recommended

## Steps

1. Clone the repository
2. Create virtual environment
3. Install dependencies

pip install -r requirements.txt

4. Create .env file (see environment variables doc)
5. Run migrations

python manage.py migrate

6. Create superuser

python manage.py createsuperuser

7. Start server

python manage.py runserver
