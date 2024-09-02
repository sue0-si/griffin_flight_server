# Project Description
This project is a Django Web application whose main purpose is to provide RESTful API servers for the Flutter project.

This API server is integrated with the database to provide user management, data query and update.

This release distributes an initial version of the API server. Further functional development and performance improvements are expected in the future. Any suggestions or improvements to the project are welcome.

### Flutter GitLink
[Flight reservation application (Front-end)](https://github.com/sc2bat/griffin_flight)

[Admin Webpage](https://github.com/sc2bat/griffin_admin_web)

## Skills
Language: Python 3.8

Database: MySQL 8.0 

Server: Ubuntu 22.04.4 LTS

Framework: Django 5.0.2

## Functionality
- User Signup and Login

- Database(MySql 8.0) CRUD


## How to install and run this project 
To run this project, follow these steps:

### Settings and Installation
Install MySQL 8.0.
```
sudo apt update
sudo apt install mysql-server
```

### Project setting
Clone this repository and set the virtual environment.
```
git clone https://github.com/your_username/your_project.git
cd your_project
python -m venv venv
source venv/bin/activate (For Window user - venv\Scripts\activate)
pip install -r requirements.txt
```

### Django setting
Change the settings for the MySQL database in the `settings.py` file inside the project.
```
DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.mysql',
        'NAME': 'your_database_name',
        'USER': 'your_database_user',
        'PASSWORD': 'your_database_password',
        'HOST': 'localhost',
        'PORT': '3306',
    }
}
```

### Perform database migration:
```
python manage.py migrate
```

#### Run the server: 
```
python manage.py runserver
```

From your browser, go to http://localhost:8000 and check the application.
