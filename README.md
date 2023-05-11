# odoogpt-docs

Documentation of OdooGPT available at [odoogpt.thespino.dev](https://odoogpt.thespino.dev)

Built with 

- [mkdocs](https://www.mkdocs.org)
- [mkdocs-material](https://squidfunk.github.io/mkdocs-material)



## Environment setup

If needed, use or create pyenv virtual env:

```sh
# Create
pyenv virtualenv 3.9.16 venv-odoogpt-docs
pyenv activate venv-odoogpt-docs

# Use
pyenv shell venv-odoogpt-docs
```

Then, install requirements: 
```sh
pip install -r ./requirements.txt
```

## Start mkdocs locally
```sh
mkdocs serve
```

## Build static site
```sh
mkdocs build
```

## Deploy to Github pages
```sh
mkdocs gh-deploy
```