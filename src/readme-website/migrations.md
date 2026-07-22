# Migrations

Every time you change the database schema you need to run the following two commands.

`python manage.py makemigrations` : creates the migration files necessary for changing the database schema

`python manage.py migrate` : applies the newly created migrations

Make sure to `git add` the migration file in `/magazine/migrations`.
