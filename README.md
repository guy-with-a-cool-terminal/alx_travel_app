
# alx_travel_app

A Django-based travel application backend project with REST API support, Swagger documentation, and MySQL database integration.

---

## Project Overview

`alx_travel_app` is a Django project designed to provide a RESTful API for travel-related listings. The project includes:

- Django REST Framework for API creation.
- MySQL database configured via environment variables.
- CORS headers support for cross-origin requests.
- Celery with RabbitMQ for asynchronous task management.
- Swagger documentation (via drf-yasg) available at `/swagger/`.

---

## Features

- **Django REST Framework:** Robust API development.
- **MySQL Database:** Configured with secure environment variables.
- **CORS Headers:** Handle cross-origin HTTP requests.
- **Celery + RabbitMQ:** Support for background task processing.
- **Swagger API Documentation:** Automatically generated docs accessible at `/swagger/`.

---

## Installation and Setup

### Prerequisites

- Python 3.8+
- MySQL Server
- RabbitMQ Server
- Virtual environment tool (e.g., `venv` or `virtualenv`)

### Getting Started

1. **Clone the repository**

   ```bash
   git clone https://github.com/yourusername/alx_travel_app.git
   cd alx_travel_app
````

2. **Create and activate a virtual environment**

   ```bash
   python -m venv venv
   source venv/bin/activate   # On Windows: venv\Scripts\activate
   ```

3. **Install dependencies**

   ```bash
   pip install -r requirements.txt
   ```

4. **Configure environment variables**

   Create a `.env` file in the `alx_travel_app` directory with your database and RabbitMQ credentials:

   ```env
   MYSQL_DB_NAME=your_db_name
   MYSQL_USER=your_db_user
   MYSQL_PASSWORD=your_db_password
   MYSQL_HOST=localhost
   MYSQL_PORT=3306

   RABBITMQ_USER=your_rabbitmq_user
   RABBITMQ_PASSWORD=your_rabbitmq_password
   RABBITMQ_HOST=localhost
   RABBITMQ_PORT=5672
   ```

5. **Run migrations**

   ```bash
   python manage.py migrate
   ```

6. **Start the development server**

   ```bash
   python manage.py runserver
   ```

7. **Access Swagger API docs**

   Navigate to [http://localhost:8000/swagger/](http://localhost:8000/swagger/) to view the API documentation.

---

## Project Structure

```
alx_travel_app/
├── alx_travel_app/
│   ├── __init__.py
│   ├── settings.py
│   ├── urls.py
│   ├── wsgi.py
│   └── ...
├── listings/
│   ├── migrations/
│   ├── __init__.py
│   ├── admin.py
│   ├── apps.py
│   ├── models.py
│   ├── serializers.py
│   ├── views.py
│   └── ...
├── requirements.txt
├── manage.py
└── .env.example
```

---

## Technologies Used

* Django
* Django REST Framework
* MySQL
* Celery
* RabbitMQ
* django-cors-headers
* drf-yasg (Swagger documentation)
* django-environ (environment variables management)

---

## Git

This project is under version control with Git. The initial commit includes the base project setup with configurations for REST, CORS, MySQL, Celery, RabbitMQ, and Swagger.

---

## License

Specify your license here if applicable.

---

Feel free to open issues or submit pull requests for improvements!

