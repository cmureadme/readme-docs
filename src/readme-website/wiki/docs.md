# Docs
## Deploying
Read the docs for like, everything.

Currently domain names cmureadme.com and staging.cmureadme.com is hosted on the following server:
```
madison.lan.cmu.edu (128.237.64.84)
```

The command used to deploy the server is:
```
/var/www/readme-staging/venv/bin/python3 -m gunicorn readme.wsgi -b 127.0.0.1:7777 --log-level debug
```

Uhhhhh this next paragraph is dogwater and you should just ask Lee about it. It's being wrapped in a code block so you don't accidentally read it.
```
a deployment script does not yet exist. Upon pulling the repo, one must chmod the directory to saffron:www-data. 
```

## Developing
skull emoji