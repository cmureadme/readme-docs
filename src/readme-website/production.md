# Hosting

KGB has a server hosted by computer club.
We run two instances of the readme website on this server: [cmureadme.com](cmureadme.com) and [dev.cmureadme.com](dev.cmureadme.com).
Each website runs in its own Docker container.

## Production Website
Our production website is [cmureadme.com](cmureadme.com), and runs off the `main` branch of [the readme-website git repo](https://github.com/cmureadme/readme-website).
We use [website-docker-prod](https://github.com/cmureadme/website-docker-prod) repo for our Docker image and scripts to build and redeploy the website.

To redeploy, run `.\redeploy.sh`.

## Development Website
Our development website is [dev.cmureadme.com](dev.cmureadme.com), and runs off the `dev` branch of [the readme-website git repo](https://github.com/cmureadme/readme-website).
We use [website-docker-staging](https://github.com/cmureadme/website-docker-staging) repo for our Docker image and scripts to build and redeploy the website.
On every redeploy, we make a copy of the production database and media folder.
This ensures that any changes we make on the development website don't affect anything on the production database.
It also ensures that any changes that we are about to implement work with our production dataset.

We have a webhook listener that redeploys upon pushes to `dev`. If this goes offline, someone with sudo on the KGB server should run ```~readme/webhookd/deploy_webhook.sh```

If you don't have a superuser/user account on our actual production website, you will not have a superuser/user account on the development website.
This means you need to test any admin changes you make on your local deployment extensively.
