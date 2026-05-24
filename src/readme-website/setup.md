# Setup
This page covers setting up eaither our developmental Docker image or venv on your local machine and getting started. 
An important note is that we have stopped supporting Windows development. If you are on windows you need to have WSL installed.
[Here](https://learn.microsoft.com/en-us/windows/wsl/install) is the offical Microsoft page on how to install WSL.

## Venv
Note that this is the prefered method for development as it is much lighterweight.
Before using the venv make sure that you have python3.13 installed.

*A note about python3.13: some systems will allow you to run python by typing `python` others require `python3` and others require `python3.13`*
To run the setup script:
```
chmod +x setup.sh
./setup.sh
```
After running this a new `.env` file will be created.
Fill in the `SECRET_KEY` field with whatever you would like.

Whenever you are running the website locally make sure that you have activated the venv: `source ./.venv/bin/activate`
## Docker
Docker desktop is really easy and intuative to use. If you don't already have Docker experance I would recommend installing Docker desktop.
Instructions can be found [here](https://docs.docker.com/desktop/).

If you are on Windows with WSL [this page](https://docs.docker.com/desktop/features/wsl/) contains the information needed to make sure that Docker is running using WSL.

Now that you have Docker installed we want to make a clone of our [developmental Docker repo](https://github.com/cmureadme/website-docker-local).
If you are on Windows with WSL open a new terminal with WSL.
If you are on Mac or Linux just open your normal terminal.

Then run `git clone https://github.com/cmureadme/website-docker-local.git`

From there follow the instructions on the [repo's readme](https://github.com/cmureadme/website-docker-local/blob/main/README.md)

Note that when you deploy the website locally you will run with `Debug=True`.
Our actual production websites run with `Debug=False`.

