# Flask Form Submission Application

This repository contains a Flask-based web application for submitting forms. Users can fill out and submit forms, and receive email notifications upon submission. The application stores submitted form data in a SQLite database.

## Features

- User-friendly form for data submission
- Email notifications for form submissions
- Data storage using SQLite
- Flash messages for user feedback

## Prerequisites

- Python 3.x
- Flask
- Flask-SQLAlchemy
- Flask-Mail

## Setup

### Clone the repository

```sh
git clone https://github.com/Dishaa01423/job_application_form-flask-.git
cd job_application_form-flask-
```

## Create and activate a virtual environment
```sh
python -m venv env
source env/bin/activate  # On Windows use `env\Scripts\activate`
```

## Install dependencies
```sh
pip install -r requirements.txt
```

## Configuration

Update the email configuration in app.py with your email credentials:

app.config["MAIL_USERNAME"] = "disha01423@gmail.com"
app.config["MAIL_PASSWORD"] = "your-email-password"

## Run the application
```sh
python app.py
```
The application will be accessible at http://127.0.0.1:5001/.

## Usage
**Access the application**
Open your web browser and go to http://127.0.0.1:5001/.

**Submitting Forms**
Fill out the form with your details and submit it. You will receive an email notification with your submitted data.

**Viewing Submitted Data**
Submitted data is stored in a SQLite database (data.db). You can view and manage the data using any SQLite database viewer.

## Deployment
**Prepare for deployment**
1. Collect static files:

2. Ensure all static files (CSS, JS, etc.) are in the appropriate directories.

3. Set up a production server: Use a web server like Gunicorn with Nginx or Apache for deployment.

4. Environment variables: Ensure you set the necessary environment variables for Flask settings, such as SECRET_KEY, MAIL_USERNAME, and MAIL_PASSWORD.
