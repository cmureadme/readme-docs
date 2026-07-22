# Requirements

In the `readme-website` directory, there are two requirements files:

- `requirements-local.txt`: This requirements file specifies the bare minimum requirements and uses `~=` to match the latest patch of the library.
- `requirements-host.txt`: This requirements file is what's used in the production Docker build, and should contain a full `pip freeze` of a working environment.

Currently the following dependencies are in `requirements-local.txt`:

| Dependency | Purpose |
|-|-|
| Django | web framework |
| gunicorn | WSGI server |
| Markdown | formatting |
| Pillow | image serving |
| python-dotenv | env creation |
| ruff | linting |
|django-markdownx | admin panel preview content |

When in your virtual environment for local development, run `pip freeze | diff requirements-host.txt -` from time to time. If any differences are printed, this indicates staging and prod are now using an out-of-date version of some library. Confirm that your local copy is working fine with the latest version, and if so, update `requirements-host.txt` to match your `pip freeze`.

## Note about `~=`, `>=`, and `==`for local requirements
- `~=`, for compatible releases, is generally preferred. 
- `>=` is used for any version that is the version specified or future releases, which may break things.
Only use this if you have a good reason to.
- `==` prevents you from receiving critical security updates.