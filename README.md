# Campus Connect

**Name:** Zyril Ryle R. Restauro  
**Section:** G1

Campus Connect is a Django application with account registration, login, a dashboard, and a profile page where signed-in users can update their own details.

## Requirements

- Python 3.10 or newer
- Django (the project was created with Django 6.1.2)

## Run locally

1. Clone the repository and open a terminal in the project folder.
2. Create and activate a virtual environment:

   ```powershell
   python -m venv .venv
   .\.venv\Scripts\activate
   ```

   On macOS or Linux, use `python3 -m venv .venv` and `source .venv/bin/activate`.

3. Install Django and confirm:

   ```shell
   pip install django
   python -m django --version
   ```

4. Apply database migrations. This is needed for a fresh database or after model changes; if your existing database is already migrated, you can skip this step:

   ```shell
   python manage.py migrate
   ```

5. (Optional) Create an administrator account if you want to use Django admin at `/admin/`:

   ```shell
   python manage.py createsuperuser
   ```

6. Start the development server and open the URL shown in the terminal (usually <http://127.0.0.1:8000/>):

   ```shell
   python manage.py runserver
   ```

Bootstrap 5 is loaded from its CDN by the shared base template, so an internet connection is needed to load its styles.
