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
    ```
    python manage.py runserver
    ``` 
    ```
    python manage.py makemigrations
    ```

    ```
    python manage.py migrate
    ```
* setting.py – It is the most important file in Django projects. It holds all the configuration values of your web project, i.e. pre-installed apps, middleware, default database, API keys, and a bunch of other stuff. 
* views.py – View is user interface. In views.py file we create python functions that takes http requests and returns http response.
* urls.py – It is a universal resource locator which contains all the endpoints, we store all links of the project and functions to call it.  
* models.py – All the database logic and tables are created by the model.py file django.
* wsgi.py – WSGI stands for Web Server Gateway Interface, This file is used for deploying the project in WSGI.
* admin.py – It is used to create a superuser Registering model, login, and use the web application.
* app.py – It is a file that helps the user to include the application configuration for their app.

## How do we start our development server?
```
python manage.py runserver
```

## Importance of virtual environment setup for Django.
* A virtual environment allows you to establish separate dependencies of the different projects 

## What are the sessions?
* Session is technique to keep track of site's and browser data. During the session, the user data is stored in sessions, which are server side files.The session ends when the user closes the browser or logs out of the program. Within a session, we can keep as much data as we want, We must use the session start() method to start the session. There is one advantage of using a session is that the data is stored in an encrypted format.

## What is Django ORM?
* ORM stand object relation model enables us to interact with our database. It allows us to add, delete, change, and query objects (Object Relational Mapper). Django uses a database abstraction API called ORM to interface Viewed with its database models, to use Django object relation Models, we must first have a project and an app running. Models can be created in app/models.py after an app has been started. The Django ORM may be accessed by running the following command in our project directory.

```
python manage.py shell
```

## What do you mean by the csrf_token?
* Cross-Site Request Forgery (CSRF) is used to prevent malecius attack. When generating the page on the server, it generates a token and ensures that any requests coming back in are cross-checked against this token.

## Explain the use of Middlewares in Django.
* Middleware is a lightweight plugin in Django that is used to keep the application secure during request and response processing

## What is Media Root?
* Media root is used to upload user-generated content. We can serve user-uploaded media files locally, using the MEDIA_ROOT and MEDIA_URL settings.

## How you can include and inherit files in your application?
Using the extends tag in Templates, we can inherit our files in Django, The extends tag is used to inherit these templates.
```
{% extends 'template_name.html' %}
```
## What is Django Rest Frameworkcont
* The REST Framework is an HTTP-based standard for listing, generating, modifying, and deleting data on your server.

## What are Django cookies?
* A cookie is a piece of information stored in the client’s browser. To set and fetch cookies, Django provides built-in methods to use the set_cookie() method for setting a cookie and the get() method for getting the cookie. we can also use the request.COOKIES[‘key’] array to get cookie values.

## What is serialization in Django?
* Serializers in the Django REST Framework are responsible for transforming objects into data types that javascript and front-end frameworks can understand.
