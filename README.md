To-Do List Application
Overview
This is a Django-based to-do list application developed as part of the ALX Back-End Capstone Project. It allows users to create, view, update, and delete tasks, add comments, and track task completion with due dates and priorities. The application includes user authentication to associate tasks and comments with users.
Features

Create, read, update, and delete tasks (CRUD operations).
Add comments to tasks.
Set task priority (Low, Medium, High) and due dates.
Track overdue tasks and completion status.
Responsive UI with Bootstrap and custom CSS (sidebar, gradient background).

Technologies

Back-End: Python 3.13, Django 5.1.6
Database: SQLite
Front-End: Bootstrap 5.3, Custom CSS
Version Control: Git, GitHub

Setup Instructions

Clone the Repository:
git clone https://github.com/mukeshimanafrank/todo_app.git
cd todo_app


Set Up Virtual Environment:
python -m venv venv
.\venv\Scripts\activate  # Windows


Install Dependencies:
pip install django


Apply Migrations:
python manage.py makemigrations
python manage.py migrate


Create a Superuser (for authentication):
python manage.py createsuperuser


Run the Server:
python manage.py runserver

Access at http://127.0.0.1:8000/.


Usage

Login: Log in with a user account to create and manage tasks.
Task Management: Create tasks with titles, descriptions, due dates, and priorities. Toggle completion or delete tasks.
Comments: View task details and add comments.
Admin Panel: Access http://127.0.0.1:8000/admin/ to manage tasks and users.

Project Structure
todo_app/
├── manage.py
├── todo/
│   ├── migrations/
│   ├── static/
│   │   └── todo/
│   │       └── styles.css
│   ├── templates/
│   │   └── todo/
│   │       ├── task_list.html
│   │       ├── task_form.html
│   │       └── task_detail.html
│   ├── templatetags/
│   │   ├── __init__.py
│   │   └── form_filters.py
│   ├── __init__.py
│   ├── admin.py
│   ├── apps.py
│   ├── forms.py
│   ├── models.py
│   ├── urls.py
│   └── views.py
├── todo_project/
│   ├── __init__.py
│   ├── asgi.py
│   ├── settings.py
│   ├── urls.py
│   └── wsgi.py
└── README.md

Future Improvements

Add task categories.
Implement REST API endpoints for integration with front-end frameworks.
Enhance UI with JavaScript interactivity.

License
MIT License
