# python base

### (1) Direnv

To create environment variables isolated to the scope of your directory, 
the `direnv` CLI provides a convenient mechanism for doing so. Start by following the
[documentation](https://direnv.net/) and then running the following command(s).

**Create container for environment variables isolated to directory scope:**
```zsh
touch ./ .envrc
```

**Enables `direnv` to load environment variables into shell:**
```zsh
direnv allow
```

### (2) Python package management CLI ([uv](https://pypi.org/project/uv/))

Fast python package installer and resolver used to manage dependencies within a virtual
environment.

**Create and activate a virtual environment using the following command(s):**

```zsh
uv venv & source .venv/bin/activate
```

### (3) Additional Notes

**Useful aliases:**

```text
alias uvfreeze="uv pip freeze | uv pip compile - -o requirements.txt"
alias uvsync="uv pip sync requirements.txt"
alias djrun="python manage.py runserver"
```