# NITC

Collection of NIT Calicut projects including the **NITC Physical Reporting Queue System**.

## NITC-Physical-Reporting

A Flask-based queue management system for physical document reporting at NIT Calicut. Handles student token booking, admin verification, and fee payment tracking.

### Features

- **Student Portal** — Register, login, book slots, upload documents (Class 10/12, category, payment receipt)
- **Admin Dashboard** — Two-tier admin verification, token management, Chanakya integration
- **Queue System** — Token generation with time slots, fee status tracking
- **Document Upload** — Secure file upload with per-student document management

### Tech Stack

- **Framework:** Flask (Python)
- **Database:** SQLite via Flask-SQLAlchemy
- **Frontend:** Jinja2 templates + static assets
- **Auth:** Session-based with role separation (student/admin)

### Setup

```bash
cd NITC-Physical-Reporting/queue-system
pip install flask flask-sqlalchemy
python app.py
```

### Default Routes

| Route | Description |
|---|---|
| `/` | Student login |
| `/register` | Student registration |
| `/admin/login` | Admin login |
| `/dashboard` | Student dashboard |
| `/admin/dashboard` | Admin management panel |
| `/book-slot` | Book a reporting slot |
| `/verify-docs` | Admin document verification |
