# Python environment overview

## Python files
There are two basic file types for working with python code:
- Plain text file with extension `*.py`
- [Jupyter notebook](https://jupyter.org) file with extension `*.ipynb`

## Integrated Development Environment (IDE)
Although it is entirely possbile to edit and run python code using only a simple text editor and your command line, an IDE can make coding a more pleasent experience.

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

## Python Environments
You can think of a python environment as a folder that contains a particular version of python and a set of python packages that you installed into the environment. The key point is that you can have multiple python environments on your computer and each environment is completely separate from all other environments. Thus, each environment can have a different set of installed packages and even a completely different version of python.

Why should you almost always use a separate python environment for each project?
1. Different projects may require packages that are incompatible with each other.
2. The more packages you install into a single environment, the more you risk having a package dependency error. It is not a question of *if* this will happen, it is a question of *when*. Thus, you are asking for trouble if you keep installing all of the packages that you need for all of your projects into the same environment. If dependencies in an environment become sufficiently convoluted, you may need to simply delete the environemnt and remake it from scratch. If you have a separate environemnt for each project, this won't affect all your other projects.

Two methods for managing python environments (we'll use conda environments in this course):
- conda environments (e.g., neu365 as in the [setup instructions](setup-your-python-environment.md))
- [venv](https://python.land/virtual-environments/virtualenv)
