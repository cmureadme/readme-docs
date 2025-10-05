# Production

KGB has a server hosted by computer club.
We use this to run all of our websites.
We run two readme websites on this server [cmureadme.com](cmureadme.com) and [dev.cmureadme.com](dev.cmureadme.com).
Each website runs in it's own Docker container, as it's own Docker image.

## Actual Production Website
Our actual production website is [cmureadme.com](cmureadme.com).
We use [this](https://github.com/cmureadme/readme-website-docker) repo for our Docker image, and scripts to build and redeploy the website.
Notably our database + media is backed up on every redeploy.
This Docker image runs of of the [`main` branch of the readme-website git repo](https://github.com/cmureadme/readme-website).

All of the media is hosted on the nginx server.
The django code itself is run using gunicorn.

We also have our sample development databases hosted at [https://cmureadme.com/sample_dbs/](https://cmureadme.com/sample_dbs/).

Everytime we push to `main` we run `.\redeploy.sh`.

## Development Website
Our development website is [dev.cmureadme.com](dev.cmureadme.com).
We use [this](https://github.com/cmureadme/dev-readme-website-docker) repo for our Docker image, and scripts to build and redeploy the website.
Notably we make a copy of the production database and media folder on every redeploy.
This ensures that any changes we make on the development website don't affect anything on the production database.
It also ensures that any changes that we are about to implement work with our actual dataset.

Note that if you don't have a superuser/user account on our actual production website you will not have a superuser/user account on the development website.
This means you need to test any admin changes you make on your local deployment extensivly.

Anyone can rebuild the dev website by going to [dev.cmureadme.cmu/rebuild](dev.cmureadme.cmu/rebuild).
This means that even if you don't have server access, you can still test any changes you make on the `dev` branch.

All of the media is hosted on the nginx server.
The django code itself is run using gunicorn.
Everything about the deployment is the same as the production deployment except for what git branch it pulls from.