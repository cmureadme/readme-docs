# Setup
We have venv and docker development setups for local development.
When you deploy the website locally you will run with `Debug=True`.
Our actual production websites run with `Debug=False`.

Windows is not supported. If you are on Windows, you need to [have WSL installed](https://learn.microsoft.com/en-us/windows/wsl/install).

## Venv
This is the preferred development environment as it is more lightweight. 

Clone the repo:
```
git clone https://github.com/cmureadme/readme-website.git
```
Run the setup script:
```
chmod +x setup.sh
./setup.sh
```
A new blank `.env` file will be created, add a secret key of your choosing.

Make sure that you have the venv activated: 
```source ./.venv/bin/activate```

Download the [sample db](https://cmureadme.com/sample_dbs/vol1to5/) and place `db.sqlite3` and the uncompressed `media` in the `readme-website` directory (NOT `readme_website`).

To start the website, run
```
python manage.py runserver
```
You should be then able to access your local website at https://localhost:8000

To create an admin account for developing the admin panel locally, run
```python manage.py createsuperuser```

*Some systems will allow you to run python by typing `python`. Others require `python3`, and others require `python3.13`*

## Docker
If you don't have experience with Docker, you can use Docker Desktop. Instructions can be found [here](https://docs.docker.com/desktop/).

If you are on Windows with WSL, [this page](https://docs.docker.com/desktop/features/wsl/) contains the information needed to make sure that Docker is running using WSL.

Run 
```git clone https://github.com/cmureadme/website-docker-local.git```

Download the [sample db](https://cmureadme.com/sample_dbs/vol1to5/) and place `db.sqlite3` and the uncompressed `media` in the `sample_dbs` directory.

From there, follow the instructions on the [repo's readme](https://github.com/cmureadme/website-docker-local/blob/main/README.md)




