# Graveyard
This is a graveyard of many of our past mistakes.
Read this file and DONT repeat these mistakes please.
Please it has taken years off of my life to fix some of these.

This website is so cursed.

The old repo for our website has been archived, but you can witness the horrors [here](https://github.com/cmureadme/readme-website-old)

## Hosting our production server inside of a student dorm
Before we moved the Readme website to be hosted on the KGB cclub server the website was hosted off of a student owned server running in a dorm.

This server also hosted other personal projects for students.
Many of our tech people also did not have ssh permissions into this server and pushing any updates was extreamly inconsistant.

Since this was hosted in a dorm and not a dedicated server room the server would also sometimes randomly go down if the dorm lost power.

It was also in the living room of this dorm where at least 8 people had physical access to it.

## Production server was run with Debug=True
I should not have to explain why this is an issue.
Don't do this lol.

## Primary keys for core models in our database where set to be strings
This means that every time you want to update certain fields it creates a whole new object.
This is so so so so awful.
Django by default has increminting numbers as primary keys.
This is how it is suppost to be done.
DO NOT manually set primary keys ever.

This is also basicly impossible to undo when it is done, so we have to create a new repo and remake our database schema.

## API key stored in plain text on the git repo
I should not have to explain why this is an issue.
Don't do this lol.

Another reason why we have to make a new repo.

## Large media files hosted on the git repo
I should not have to explain why this is an issue.
Don't do this lol.

This made the `.git` file massive.
It was larger than the entire Linux repo.

Another reason why we have to make a new repo.

## requirements.txt
This entire file was cursed.

There were multiple libraries in there that where just completely unused.

Also requirments where set with `==` not `~=` so we never got security updates leading to 14 different security vulnrabilities.

Also `psycopg2-binary` which is a library for PostgreSQL when we use sqlite3.
This library gave so many dependancy issues and hours of debugging when it was completely unused and beyond useless for our uses.
Also the precompiled binary should not be used in production mode as there are security issues.

## User accounts
There were many shared user accounts on the Django website that an unknown amount of people had the login information to.
There should be one account per user and one user per account for security purposes, and loging purposes.