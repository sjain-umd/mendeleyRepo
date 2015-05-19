#Steps to get the app running

* Install mysql

```$sudo apt-get install mysql-server-5.6```

* Create database in mysql

```$create database mwproject;```

In mySQL, change password of root user


* Install pythons package management system

```$sudo apt-get install python-pip```

* Install dependencies

```sudo apt-get install build-essential python-dev libmysqlclient-dev```

* Install virtual environment 

```$sudo pip install virtualenv```

```$virtualenv mendeleyenv```

```$cd mendeleyenv```


* Clone the git repository

```$git clone https://github.com/sjain-umd/mendeleyRepo.git```

```$cd mendeleyRepo```

* Install dependencies in virtual environment from requirements.txt

```$pip install -r requirements.txt```

* Add settings.py in folder parallel with urls.py (mendeleyapp/settings.py)

* Update database credentials in settings.py

* Sync the database

```$python manage.py syncdb```

* Run server

```$python manage.py runserver 0.0.0.0:8000```

Once the server is started, type the following url in browser.

(http://localhost:8000/logout/) (this is to force logout once)

Next use the front end to enter id of WorldCat record.

(http://localhost:8000/static/client-base.html)




