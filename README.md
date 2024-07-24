# python base

### Direnv

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

### Python package management CLI ([uv](https://pypi.org/project/uv/))

Fast python package installer and resolver. Used to manage dependencies within a virtual
environment. Create the virtual environment using the `uv venv` command. Activate the
virtual environment using `source .venv/bin/activate`.