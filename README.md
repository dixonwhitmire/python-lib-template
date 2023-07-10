# python-lib-template

A template project for Python >= 3.9 library projects which includes:

- [pytest](https://docs.pytest.org/)
- [black](https://pypi.org/project/black/)
- [isort](https://pypi.org/project/isort/)
- [PEP 517 metadata build](https://setuptools.pypa.io/en/latest/userguide/declarative_config.html)

## Quickstart

```shell
# create virtual environment and execute tests
python3 -m venv venv && \
        source venv/bin/activate && \
        python3 -m pip install --upgrade pip setuptools
        
python3 -m pip install -e .[dev]

python3 -m pytest
```

## Using the Template

* clone the repository for your specific project `git clone <url> <your project name>`
* rename the toplevel namespace and package directories
* update setup.cfg to reflect project naming as appropriate
* update logging.yml to utilize the project's namespace/packaging as appropriate
* review [setup.cfg]([PEP 517 metadata build](https://setuptools.pypa.io/en/latest/userguide/declarative_config.html)) for additional settings