# Setup

This page covers setting our developmental Docker image on your local machine and getting started. 

## Docker
An important note is that we have stopped supporting Windows development. If you are on windows you need to have WSL installed.
[Here](https://learn.microsoft.com/en-us/windows/wsl/install) is the offical Microsoft page on how to install WSL.

Docker desktop is really easy and intuative to use. If you don't already have Docker experance I would recommend installing Docker desktop.
Instructions can be found [here](https://docs.docker.com/desktop/).

If you are on Windows with WSL [this page](https://docs.docker.com/desktop/features/wsl/) contains the information needed to make sure that Docker is running using WSL.

Now that you have Docker installed we want to make a clone of our [developmental Docker repo](https://github.com/cmureadme/readme-website-dev-docker).
If you are on Windows with WSL open a new terminal with WSL.
If you are on Mac or Linux just open your normal terminal.

Then run `git clone https://github.com/cmureadme/readme-website-dev-docker.git`

From there follow the instructions on the [repo's readme](https://github.com/cmureadme/readme-website-dev-docker/blob/main/README.md)

Note that when you deploy the website locally you will run with `Debug=True`.
Our actual production websites run with `Debug=False`.

