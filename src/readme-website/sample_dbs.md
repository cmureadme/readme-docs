# Sample Databases

We have sample databases that can be downloaded and used for development.
The databases can be found at [cmureadme.com/sample_dbs/](cmureadme.com/sample_dbs/).

## Creating sample databases
There is a script called `make_sample_db.sh` inside of the `website-docker-prod` folder in the Readme account on the KGB server.
The script removes all sensitive information from the database.
When running the script the first argument is the name of the folder these will be stored in.
The next arguments are the volumes that are to be kept.

```bash
./make_sample_db.sh vol1to3 1 2 3
```

This will create a folder `sample_dbs/vol1to3` inside it there will be two files `sample_db.sqlite3` and `media.tar.gz`.

The database will only contain data in volumes 1, 2, and 3.
The media folder will also only contain the images associated with these volumes.

This folder will be immediately available on the web at `cmureadme.com/sample_dbs/vol1to3` and anyone can download the two files in it.

### Small Note
When you want to use the newly downloaded database on your local setup of the website rename the file from `sample_db.sqlite3` to `db.sqlite3`.
The website is configured to look for a file named `db.sqlite3`.