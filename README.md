# odoogpt-docs

Documentation of OdooGPT available at [odoogpt.thespino.dev](https://odoogpt.thespino.dev)

Built with 

- [mkdocs](https://www.mkdocs.org)
- [mkdocs-material](https://squidfunk.github.io/mkdocs-material)



## Environment setup

```sh
pip install -r ./requirements.txt
```

## Start mkdocs locally
```sh
mkdocs serve
```

## Build stati csit
```sh
mkdocs build
```

## Deploy with `mike`
Use [mike](https://github.com/jimporter/mike) plugin to deploy into `gh-pages` branch and get live 
build into github pages. 

The documentation *should have new versions only on notable or breaking changes*, otherwise simply 
update it in the corresponding version. That's why this docs use a `major.minor` format only. 

That should cover all supported Odoo versions, so for example version "1.0" should contain all 
documentation for versions "\*.\*.1.0.\*" (i.e. 16.0.**1.0**.0, 16.0.**1.0**.1, 15.0.**1.0**.0, ...)

```sh
mike deploy --push --update-aliases <major.minor> latest
```
