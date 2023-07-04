# Liverpool FC web project - README
## liverpool-fc-web-project
Liverpool FC website project produced as part of University of Edinburgh/ 
HyperionDev Software Engineering Bootcamp. The website contains two standalone 
pages ('Home' and 'Honours'), a members' area which makes use of a custom
Django user/ authentication solution and a competition area which allows an
admin use to load competition 'posts' and makes use of Django authentication
routines.

## Table of contents
1. Installation
2. Usage
3. Credits

## 1. Installation
* Clone the GitHub repo locally in a folder called 'LiverpoolFC'.
* Ensure you have python3 installed on your machine (details can be found
  [here](https://www.python.org)).
* Set up a virtual environment for the project by running the following commands:
  * python -m pip install pip
  * pip install virtualenv
  * pip install virtualenvwrapper
* For MacOS users, place the following code in your ~/.zshrc file:

```bash
# Setting PATH for Python 3 installed by brew if it is not present
export PATH=/usr/local/share/python:$PATH
# Configuration for virtualenv
export WORKON_HOME=$HOME/.virtualenvs
export VIRTUALENVWRAPPER_PYTHON=/usr/local/bin/python3 export 
VIRTUALENVWRAPPER_VIRTUALENV=/usr/local/bin/virtualenv source
/usr/local/bin/virtualenvwrapper.sh
```

* Open a command line window and type the following to set up your virtual
* environment and install Django:

```bash
mkvirtualenv my_django
workon my_django
pip install django
```

## 2. Usage
To run the website locally, navigate to the top level LiverpoolFC folder you 
created during installation and type the following commands:

```bash
workon my_django
python manage.py runserver
```

The website can be accessed at ```http://127.0.0.1:8000/website```.

To access the admin functionality, you need to create a superuser account by
entering ```python manage.py createsuperuser``` at the command line.  The 
admin access is available at ```http://127.0.0.1:8000/admin```.


## 3. Credits
Developed by Andrew Baker (GitHub: andrewjbaker) as part of the University of 
Edinburgh and HyperionDev Software Engineering Online Bootcamp (2023).

## 4. URL
You can access the repository for this project 
[here](https://github.com/andrewjbaker/liverpool-fc-web-project)
