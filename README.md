#Steps to get the app running

1. Install mysql

```$sudo apt-get install mysql-server-5.6```

2. Create database in mysql

```$create database mwproject;```

In mySQL, change password of root user


3. Install pythons package management system

```$sudo apt-get install python-pip```

4. Install dependencies

```sudo apt-get install build-essential python-dev libmysqlclient-dev```

5. Install virtual environment 

```$sudo pip install virtualenv```

```$virtualenv mendeleyenv```

```$cd mendeleyenv```


6. Clone the git repository

```$git clone https://github.com/sjain-umd/mendeleyRepo.git```
```$cd mendeleyRepo```

7. Install dependencies in virtual environment from requirements.txt
```$pip install -r requirements.txt```

8. Add settings.py in folder parallel with urls.py (mendeleyapp/settings.py)

9. Update database credentials in settings.py

10. Sync the database
```$python manage.py syncdb```

11. Run server
```$python manage.py runserver 0.0.0.0:8000```

Once the server is started, type the following url in browser.
http://localhost:8000/logout/ (this is to force logout once)
Next use the front end to enter id of WorldCat record.
http://localhost:8000/static/client-base.html




