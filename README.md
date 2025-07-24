# Django CV Generator 📝

A simple web application built with Django that allows users to input their personal and professional information, generate a formatted CV (resume), and download it as a PDF.

---

## 🚀 Features

- Collect user information through a styled form
- Dynamically generate a resume from the submitted data
- Clean and modern HTML template for the resume
- Downloadable CV in PDF format
- Admin interface to manage user profiles
- Responsive and printable resume layout

---

## 🛠️ Technologies Used

- Python 3.13+
- Django 5.2+
- Bootstrap 4 (for styling)
- HTML, CSS
- Git & GitHub

---

## 📂 Project Structure

cv-generator/
├── mysite/ # Django project folder
│ └── settings.py # Configured with environment variables
├── pdf/ # Core app for CV generation
│ ├── models.py # Profile model
│ ├── views.py # Accepts form data & renders resume
│ └── templates/pdf/ # HTML templates (form, list, resume)
├── db.sqlite3 # Local database (ignored in repo)
├── .env # Environment variables (ignored)
├── .gitignore
├── manage.py
└── README.md


---

## ⚙️ Setup Instructions

# 1. Clone the repository
git clone https://github.com/yourusername/cv-generator.git
cd cv-generator

# 2. Create and activate a virtual environment
python -m venv env
# On macOS/Linux:
source env/bin/activate
# On Windows:
env\Scripts\activate

# 3. Install dependencies (adjust if no requirements.txt)
pip install django python-decouple

# 4. Create a .env file in the root directory and add your secret key
echo "SECRET_KEY=your-django-secret-key" > .env
echo "DEBUG=True" >> .env

# 5. Apply migrations
python manage.py migrate

# 6. Run the development server
python manage.py runserver

# Visit the app in your browser:
# http://127.0.0.1:8000/
