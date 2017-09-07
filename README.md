# Integrated Business Management System

This project consists of the Integrated Business Management System
(IBMS) corporate application, used by the Department of Biodiversity
 Conservation and Attractions.

# Installation

Create a new virtualenv and install required libraries using `pip`:

    pip install -r requirements.txt

# Environment variables

This project uses confy to set environment
variables (in a `.env` file). Required settings are as follows:

    DJANGO_SETTINGS_MODULE="ibms_project.settings"
    DEBUG=True
    DATABASE_URL="postgis://USER:PASSWORD@HOST:PORT/DATABASE_NAME"
    SECRET_KEY="ThisIsASecretKey"
    CONFLUENCE_URL="https://confluence.dpaw.wa.gov.au"

# Running

Use `runserver` to run a local copy of the application:

    python manage.py runserver 0.0.0.0:8080

Run console commands manually:

    python manage.py shell_plus
