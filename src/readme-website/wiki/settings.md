# Settings
Django supports having multiple different settings files for different contexts.
All of the settings files are python files placed in `settings/`.
In general you should not need to edit any of the settings files.

---
**NOTE**

Django expects you to have a variable in settings named `SECRET_KEY`.
This is used for things like hashing passwords.
It is bad to have a secret key tracked in settings.
We have seprate secret keys that we use for the production and staging servers.
When you are running the website locally you need to make a secret key for yourself.
Since the passwords and other sensative data you are storing locally dosen't matter you can make your secret key anything.
Create a file called `.env` and put in it `SECRET_KEY = "whateveryouwant"`.

---

# Base
`base.py` contains the base settings that apply to every instance of the website.
No matter if you are running the website locally, or in a production context these settings apply.
The bulk of our settings live in this file, because there are not many settings that are dependent on the hosting context.

# Host
`host.py` contains the settings that are needed when running on a server, and not your local machine.
It extends `base.py` meaning it has all of the settings defined in `base.py` and all of the settings defined in `host.py`.

# Production
`prod.py` contains the settings that are needed for running on our main production website.
It builds off of `host.py`.

# Staging
`staging.py` contains the settings that are needed for running our staging website.
It builds off of `host.py`.

# Local
`local.py` contains the settings that are needed for running the website on your local machine.
It builds off of `base.py`.