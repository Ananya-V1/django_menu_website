# Little Lemon

A Django website for Little Lemon, a fictional family-owned Mediterranean restaurant in Chicago. Built as a learning project while following the Meta Back-End Developer course on Coursera.

## Features

- Home, About, Menu and Book pages sharing one base template with a header and navigation bar
- Menu page listing dishes from the database, each linking to its own detail page
- Booking form that saves reservations to the database
- Django admin for managing menu items and bookings

## What I practised

- Django models and migrations (`Menu`, `Booking`)
- Function-based views and URL routing, including URL parameters (`menu_item/<int:pk>`)
- Template inheritance with `{% extends %}` and `{% block %}`, loops, and the `{% url %}` tag
- Model forms and the Django admin
- Serving static files (CSS and images)

## Running it locally

```bash
python -m venv venv
source venv/bin/activate        # Windows: venv\Scripts\activate
pip install -r requirements.txt
python manage.py migrate
python manage.py createsuperuser
python manage.py runserver
```

Open http://127.0.0.1:8000/. Add menu items at http://127.0.0.1:8000/admin/.
