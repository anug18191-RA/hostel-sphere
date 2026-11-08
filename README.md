# HostelSphere - Integrated Smart Hostel Management System

A web-based hostel management system for students, wardens, administrators and maintenance staff.

**Live demo:** https://hostelsphere.pythonanywhere.com

## About

HostelSphere replaces paper registers with one system for room allocation, fees, complaints, visitors, leave and the mess menu. Each role gets its own portal.

BCA college project, MLA Academy of Higher Learning, Bengaluru City University.

- **Team:** Annapurna L, Chithra TS
- **Guide:** Ms. Kamala

## Features

- Four role-based portals: Student, Warden, Admin and Maintenance
- Student registration, login and forgot password
- Room allocation and room management
- Fee tracking with paid and due amounts, and fee receipts
- Complaints with picture attachment
- Leave requests and visitor entry with approval
- Student ID card with QR code
- Mess menu
- Dashboards with charts and reports
- Settings and restore of deleted data

## Tech Stack

- Frontend: HTML, CSS, JavaScript
- Backend: Python, Django 5.2
- Database: SQLite (default), MySQL supported through PyMySQL
- Image uploads: Pillow

## Run Locally

Install Python 3.12 and Git first, then run:

```
git clone https://github.com/anug18191-RA/hostel-sphere.git
cd hostel-sphere
python -m venv venv
venv\Scripts\activate
pip install -r requirements.txt
python manage.py migrate
python manage.py runserver
```

Open http://127.0.0.1:8000 in your browser.

## Demo Accounts (fresh local install only)

| Role | Username | Password |
|---|---|---|
| Admin | admin | admin123 |
| Warden | warden | warden123 |
| Maintenance | maint | maint123 |

Students can register from the login page. Change these passwords before hosting the project anywhere public.

## Project Structure

```
hostel/            main app (models, views, templates, static files)
hostel_sphere/     Django project settings and URLs
manage.py          Django management script
requirements.txt   Python dependencies
setup.sql          optional MySQL schema
```

## Deployment

The live demo runs on PythonAnywhere (free plan) with SQLite.