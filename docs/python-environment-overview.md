# Python environment overview

## Python files
There are two basic file types for working with Python code:
- Plain text file with extension `*.py`
- [Jupyter notebook](https://jupyter.org) file with extension `*.ipynb`

## Integrated Development Environment (IDE)
Although it is entirely possbile to edit and run Python code using only a simple text editor and your command line, an IDE can make coding a more pleasent experience.

A few recommended IDEs:
- [Jupyter Lab](https://jupyter.org)
- [Visual Studio Code (VSCode)](https://code.visualstudio.com)
- [PyCharm](https://www.jetbrains.com/pycharm/)
- [Spyder](https://www.spyder-ide.org)
- [Google Colab](https://colab.research.google.com)

## Package managers
I suggest using `conda` because it allows you to manage `python` as a package, and for each `python` version that you install you can still use `pip` as well if you want.

- `conda` (e.g., [miniconda](https://docs.conda.io/en/main/miniconda.html)) <-- Also manages `python` and `pip` as packages in conda.
- `pip`: [Python Package Index (PyPI)](https://pypi.org) <-- Tied to a particular installation of `python`.

## Virtual Environments
- conda environments (e.g., neu365 as in the [setup instructions](setup-your-python-environment.md))
- [venv](https://python.land/virtual-environments/virtualenv)
