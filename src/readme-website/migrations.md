# Migrations

To change the database:

1. make changes to `models.py`. 
  - you may need to update `admin.py` or `forms.py`
2. run `python manage.py makemigrations` to generate a migrations file (in `/[app]/migrations`). This is how django is able to update the database consistently
3. run `python manage.py migrate` to apply the migration to the db. 

~~~admonish note
Make sure to `git add` the migration file in `/[app]/migrations`.
If you `git pull` a migration file, you also need to run `python manage.py migrate` to apply it.
~~~

~~~admonish warning
If something breaks during the command line steps, you may have corrupted your database file. If this is a concern, follow these steps to restore it:
1. delete the new migration file
2. redownload the database file from [here](cmureadme.com/sample_dbs/)
~~~

