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
2. delete the `db.sqlite3`
3. run from the command line `python manage.py migrate  # create the blank database file`
4. run from the command dline `python manage.py loaddata db_sample.json  # populate it with sample data`
~~~

### database data to/from json
This command dumps all data to a json file, except admin logs such as editing articles, etc.
```
python manage.py dumpdata --natural-foreign --natural-primary -e contenttypes -e auth.Permission --indent 2 > dump.json
```
If you're on Windows, you may need to add the `-Xutf8` flag after `python`.

A corresponding `loaddata` command exists. See https://docs.djangoproject.com/en/5.1/ref/django-admin/. For comprehensive docs.
