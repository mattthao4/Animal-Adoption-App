# Animal Adoption App

## Overview
This is a Django-based Animal Adoption App for managing animal shelters, adoptions, donations, medical records, and staff/adopter accounts. The project includes a custom user model, staff/adopter dashboards, animal and shelter management, donation tracking, and medical record management. The frontend uses Django templates and static assets (CSS, images).

## Project Structure
- `shelter_project/` - Main Django project folder.
  - `shelterapp/` - Main application with models, views, forms, templates, and admin configuration.
  - `shelter/` - Project settings, URLs, and WSGI/ASGI entry points.
  - `static/` - Static files (CSS, images).
  - `db.sqlite3` - SQLite database (default for development).
  - `manage.py` - Django management script.
- `venv/` - Python virtual environment (not included in deployment).

## Key Features
- User authentication with custom user model (staff and adopters).
- Staff dashboard for managing animals, adoptions, medical records, paychecks, and donations.
- Adopter dashboard for viewing animals, submitting adoption requests, and tracking status.
- CRUD operations for animals, shelters, donations, and medical records.
- Search and filter functionality for medical records.
- Responsive HTML templates and custom CSS.

## Setup Instructions

1. **Clone the repository:**
   ```sh
   git clone <your-repo-url>
   cd Animal-Adoption-App
   ```

2. **Create and activate a virtual environment:**
   ```sh
   python -m venv venv
   # On Windows:
   venv\Scripts\activate
   # On macOS/Linux:
   source venv/bin/activate
   ```

3. **Install dependencies:**
   - If you have a `requirements.txt`, run:
     ```sh
     pip install -r requirements.txt
     ```
   - If not, install Django (and any other dependencies you use):
     ```sh
     pip install django
     ```

4. **Apply migrations:**
   ```sh
   python shelter_project/manage.py migrate
   ```

5. **Create a superuser (for admin access):**
   ```sh
   python shelter_project/manage.py createsuperuser
   ```

6. **Run the development server:**
   ```sh
   python shelter_project/manage.py runserver
   ```

7. **Access the app:**
   - Open your browser and go to: [http://127.0.0.1:8000/](http://127.0.0.1:8000/)

## Notes
- Static files are located in `shelter_project/shelter/static/`.
- HTML templates are in `shelter_project/shelterapp/templates/`.
- The default database is SQLite (`db.sqlite3`), suitable for development.

## How to Stop the Server
- Press `Ctrl+C` in the terminal.

## How to Deactivate the Virtual Environment
- Run `deactivate` in the terminal.
