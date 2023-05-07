# Python

Python is a programming language that is easy to learn and use. It is interpreted, instead of compiled, so you run your programs through the python interpreter or executable. Follow the instructions below to start using Python.


## Installing Python

1. Open a browser and navigate to: https://www.python.org/downloads/
2. Download a version of Python for your operating system.
3. Run the installer.
4. Update your path environment variable.
5. To validate your installation, open a command prompt and type `python`.
6. You should see a message about the version of python installed and the python prompt: `>>>`.


## Virtual Environments

Python virtual environments are a good way to isolate the versions of python and django you use for your projects from your main installation. They are not required but are a good idea if you want to try different versions of python and django on different projects. Follow the instructions below to create a python virtual environment on Windows:

1. Open a command window and navigate to your project directory.
2. To create a virtual environment run `python -m venv <virtual_environment_name>`
3. To activate the virtual environment, make sure you are in the virtual enviornment directory then run `Scripts\activate`
4. It's a good idea to update pip after creating a virtual environment. To do that, run `python -m pip install --upgrade pip`
5. To deactivate the virtual environment run `Scripts\deactivate` or just close the command window.


## Django

Django is a python web framework that is robust, easy to use and secure. Many popular websites use django like Instagram, Spotify, and Youtube. Follow the instructions below to install it:

1. Navigate to your virtual environment directory and activate it.
2. To install django run `pip install django`
3. To start a django project run `django-admin startproject <project_name>`
4. To start the development server, navigate to the `<project_name>` directory then run `python manage.py runserver`
5. Open a web browser and navigate to `http://localhost:8000/`
6. To start an app run `django-admin startapp <app_name>`.
7. Afer creating the app, navigate to the app directory and create folders for `templates` and for `static` files.




