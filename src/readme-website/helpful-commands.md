# Helpful Commands

Django comes with a lot of functionality.
[Here](https://www.djangoproject.com/) is the full django documentation, but here is a list of helpful commands.

`python manage.py runserver` : starts the website

`python manage.py makemigrations` : creates the migration files necessary for changing the database schema

`python manage.py migrate` : applies the newly created migrations

Every time you change the database schema you need to run the above two commands in order.

*A note about `python`: some systems will allow you to run python by typing `python` others require `python3` and others require `python3.13`*