# Django Important Questions

## What is Django?
* Django is a Full-stack web development framework
* Django is high level, open source and python based web framework and was created in 2003. It follows the model view template (MVT) architechture pattern. Netflix, Instagramm, Mozilla, Nextdoor, and Amazon.

## What is the difference between a Project and an App?
* The main difference between a project and an app is that a project is defined as the entire application whereas, an app is part of the project

## Explain Django’s architecture.
* Django follow MVT(model, view, template) architechture. All the database logic and tables are created by the model.py file django. View is user interface and it accept request by the user and reponse. While in template folder we define our HTML, CSS, and JavaScript files.

## What are the Features of using Django?
* Open Source 
* Secure and Versatile 
* Vast and Supported Community
* Web templating system
* Middleware class support
* Admin Interface
* Django is SEO optimized

## How do you create a Django project?

```
django-admin startproject ProjectName
```

## How do you create a Django app?

```
python manage.py startapp AppName
```

## Explain the Django project directory structure
* init.py – It’s an empty Python file. This file tells the Python interpreter that this directory is a package and that the presence of the __init.py_ file makes it a Python project.
* manage.py – This file is used to interact with your project from the command line utility.
    ```python manage.py runserver``` 
    ```python manage.py makemigrations```
    ```python manage.py migrate```