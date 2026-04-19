# OTT Platform - Django Project

## Setup Instructions

1. **Install MySQL** and create a database:
   ```sql
   CREATE DATABASE ott CHARACTER SET utf8mb4 COLLATE utf8mb4_unicode_ci;
   ```

2. **Import seed data** (optional):
   ```bash
   mysql -u root -p ott < ott.sql
   ```

3. **Install Python dependencies**:
   ```bash
   pip install -r requirements.txt
   ```

4. **Update database credentials** in `ott_project/settings.py` (DATABASES section).

5. **Run migrations**:
   ```bash
   python manage.py makemigrations
   python manage.py migrate
   ```

6. **Load initial data** (if you didn't import ott.sql):
   ```bash
   python manage.py loaddata initial_data
   ```

7. **Run the server**:
   ```bash
   python manage.py runserver
   ```

8. **Access the app**:
   - User site: http://127.0.0.1:8000/
   - Admin login: username `admin`, password `admin123`
   - User login: username `aditi`, password `user123`
