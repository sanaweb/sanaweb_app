sanaweb_app
===========

System Requirements:
-------------------

Python2.7
http://www.python.org/download/releases/2.7.6/

MySQL
http://dev.mysql.com/downloads/mysql/


Python Setup:
------------

Install Python setuptools
> sudo wget https://bitbucket.org/pypa/setuptools/raw/bootstrap/ez_setup.py -O - | python
 
Install Pip
> easy_install pip

Create virtualenv
> virtualenv sanaenv

Activate virtualenv
> . sanaenv/bin/activate

Install Python packages
> pip install Django==1.6
> pip install mysql-python


Django Setup:
------------

Create Sana project
> django-admin.py startproject sana

Sync database
> python manage.py syncdb

Create Sana web app (inside project directory)
> python manage.py startapp <app_name>


Database setup:
--------------

Edit settings.py
See https://docs.djangoproject.com/en/1.6/ref/settings/#databases for database specific details

