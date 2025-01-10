# Docs
## Deploying
Read the docs for like, everything.

Currently domain names cmureadme.com and staging.cmureadme.com is hosted on the following server:
```
madison.lan.cmu.edu (128.237.64.84)
```

The command 
```
/usr/bin/sudo -u www-data /var/www/readme-deploy.sh
```
deploys the main branch. Similar commands exist for the staging and dev branches. The user that runs this command on the `madison` server must be in the `www-data` group (I think).

## Developing
### changing the database
The general flowchart for database changes is

1. something will change in a `models.py` to specify the model/table you create/update. 
  - you may need to update the corresponding `admin.py` and or `forms.py` to let django know what's up (what to show in admin dashboard and what forms to show in that dashboard, respectively)
2. run on the command line `python manage.py makemigrations` to generate a migrations file (saved in the migrations folder). This is how django is able to update the database file from the old schema to the new. Take a look at what it looks like!
3. run on the command line `python manage.py migrate` to apply that migration file to the db. 

Hopefully, your changes worked!

~~~admonish warning
If something breaks during the command line steps, you may have corrupted your database file. If this is a concern, follow these steps to restore it:
1. delete the new migration file
2. delete the `db.sqlite3`
3. run from the command line `python manage.py migrate  # create the blank database file`
4. run from the command dline `python manage.py loaddata db_sample.json  # populate it with sample data`
~~~
