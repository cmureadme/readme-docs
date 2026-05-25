# Linting

We use `ruff` for linting and formatting of our Python code. It should install along with the rest of the dependencies if you install `requirements-local.txt`.

To use the linter, run `./lint.sh` from the project root directory. This is currently equivalent to `ruff check && ruff format`. 

(This is done in the [Setup](../setup.md) script) To automate this, you can run `./install-lint-hook.sh` from the project root directory. This will symlink `.git/hooks/pre-commit` to `lint.sh`, causing it to run before every commit. Note that you can only have one pre-commit hook per local repository, so if you're using another piece of software like `pre-commit`, you'll need to make them play nice.
