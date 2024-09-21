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
skull emoji