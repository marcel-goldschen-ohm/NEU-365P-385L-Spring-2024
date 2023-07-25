# NEU-365P-385L-Spring-2024
Programming and Data Analysis for Modern Neuroscience

# Setup your Python environment
You are free to setup your python environment however you like. The following is my recommended approach and what I will assume you have done for the purposes of this course.

### 1. Install Conda
Download and install the latest version of [Miniconda3](https://docs.conda.io/en/latest/miniconda.html).

*On macOS I suggest using the **pkg** installer as it is the simplest.*

### 2. Configure Conda
Conda groups collections of packages into [channels](https://docs.conda.io/projects/conda/en/latest/user-guide/concepts/channels.html). Most of the packages that you will install for this course will come from either the defaults or [conda-forge](https://conda-forge.org/docs/user/introduction.html) channels. Conda only searches channels that you tell it to. To setup conda so that it automatically searches the [conda-forge](https://conda-forge.org/docs/user/introduction.html) channel before searching the defaults channel, open a command shell or terminal and run:
```
conda config --add channels conda-forge
```
To see a list of all of the channels that conda will search (top = highest priority, bottom = lowest priority):
```
conda config --show channels
```
Note that you can always specify the channel to search when installing packages on a per package basis. An example of this is shown in the next step.

### 3. Create a sandboxed Python environment for this course
First, create a new conda environemnt named "neu365p". In a command shell or terminal run:
```
conda create --name neu365p
```
Next, set "neu365p" as the active environment for all conda commands. Run:
```
conda activate neu365p
```
Now install the latest version of the `python` package (from the defaults channel) into the active ("neu365p") environment.
```
conda install python
```
Finally, install the latest version of the `jupyterlab` package (from the conda-forge channel) into the active ("neu365p") environment.
```
conda install jupyterlab -c conda-forge
```
*Note that if you configured conda to automatically search the conda-forge channel as described above, then you could omit the `-c conda-forge` portion of the last command.*

⚠️ Note that each time you open a new command shell or terminal, you will need to activate the conda environment that you want to use:
```
conda activate neu365p
```
The currently active environment should be displayed in your command prompt, e.g. `(neu365p)`.

You can see a list of all your conda environments with:
```
conda env list
```
You can see a list of all installed packages in your active environment with:
```
conda list
```

### 4. Run JupyterLab
[JupyterLab](https://jupyter.org) is a complete Python integrated development environment (IDE) that supports Jupyter notebooks (which we will use in this course). It runs in a tab in your browser. You should already have installed JupyterLab in the previous step.

To run JupyterLab first make sure your "neu365p" environment is active:
```
conda activate neu365p
```
Then, simply run the command:
```
jupyter-lab
```
This will start **JupyterLab which will open up a tab in your browser with a complete user interface** for writing and running Python code.

When you are done using JupyterLab, from within the JupyterLab browser interface select `File->Shutdown`.

### 5. `OPTIONAL:` Install Visual Studio Code (VSCode)
There are a variety of user interfaces for Python coding from the most basic text editor and cmd shell to more complex user interfaces with more features such as JupyterLab. One alternative to JupyterLab that is compatible with Jupyter notebooks is VSCode.
1. Download [Visual Studio Code (VSCode)](https://code.visualstudio.com/)
2. Open VSCode and install the **Python** and **Jupyter** extensions.
3. In VSCode, Select `View->Command Palette...` and search for and select `Python: Select Interpreter`, then select the Python version associated with your neu365p environment (e.g., `Python 3.11.0 ('neu365p')`).
4. In VSCode you can also set the Python interpreter for each individual file. When you open a Python file the interpreter will be displayed in one of the corners. Make sure it is set to the Python version associated with neu365p, otherwise click the displayed interpreter and select from the dropdown the one for neu365p.

*It does NOT matter which user interface you use.* Both JupyterLab and VSCode will give you a pretty similar experience, as will several others.

# Keep up-to-date with the course GitHub repository
1. Create a [GitHub](https://github.com) account for yourself (it's free). 
2. Download the [GitHub Desktop](https://desktop.github.com) application.
3. Sign into to GitHub Desktop using your GitHub account credentials.
4. Go to [the course GitHub repo](https://github.com/marcel-goldschen-ohm/NEU-365P-385L-Spring-2024), click the `<> Code` button in the upper right and choose `Open with GitHub Desktop`. This will open GitHub Desktop on your computer and ask you to choose a location in which to clone (copy) all of the course repo files. When it is done you will have a local copy of the course GitHub repo in a folder on your computer.
5. Whenever you want to make sure your local copy is an up-to-date reflection of the current online course repo, all you have to do is launch GitHub Desktop, select the repo for this course and click the `Fetch Origin` button in the upper right. If this button changes to `Pull Origin`, that means that there are changes in the online repo that you do not have locally. Just click the `Pull Origin` button and all of the changes including new files in the online repo will be downloaded so that your local repo is an exact copy of the current online course repo.
6. ⚠️ Whenever you execute Step #5 above, your local repo will become an EXACT COPY of the online course repo. *THIS INCLUDES RESETTING ANY HOMEWORK FILES YOU COMPLETED WITH THE ONLINE BLANK HOMEWORK FILES!* To avoid this, make sure **YOU MOVE YOUR HOMEWORK FILES OUTSIDE OF YOUR LOCAL REPO FOLDER BEFORE YOU WORK ON THEM!**

# Python environment overview
- Python Files
  - Text file: `*.py`
  - [Jupyter notebook](https://jupyter.org) file: `*.ipynb`
- A few recommended Integrated Development Environments (IDEs)
  - [Jupyter Lab](https://jupyter.org)
  - [Visual Studio Code (VSCode)](https://code.visualstudio.com)
  - [PyCharm](https://www.jetbrains.com/pycharm/)
  - [Spyder](https://www.spyder-ide.org)
  - [Google Colab](https://colab.research.google.com)
- Package managers
  - `conda` (e.g., [miniconda](https://docs.conda.io/en/main/miniconda.html)) <-- Also manages Python itself!
  - `pip`: [Python Package Index (PyPI)](https://pypi.org)
- Virtual Environments
  - conda environments (e.g., neu365p in the setup instructions above)
  - [venv](https://python.land/virtual-environments/virtualenv)

# Python Basics
Familiarizing yourself with the concepts listed below is in my opinion sufficient for a very reasonable level of mastery in Python.

1. Variables and the importance of choosing good names for them.
2. Basic data types: `int`, `float`, `bool`, `str` and `type` function
3. Comments and multi-line strings: `#`, `"""`
4. Basic operations: `+`, `-`, `*`, `/`, `**`
5. Logical comparisons: `==`, `!=`, `<`, `>`, `<=`, `>=`, `and`, `or`, `not`
6. `if`, `elif`, `else` blocks
7. Nested blocks
8. `list` and `tuple`
9. `sorted` and `reversed` functions
10. List unpacking: `*`
11. List zipping: `zip`
12. List comprehensions
13. List indexing and slicing: `[start]`, `[start:stop]`, `[start:stop:step]` <-- *stupid 0-based indexing*
14. Dictionary (key, value) pairs: `dict`
15. Dictionary indexing: `[key] = value`
16. `for` and `while` loop blocks
17. `range` and `len` functions
18. `def` function blocks
19. Default and named function arguments
20. Assignment vs. Mutation
21. Variable scope
22. `class` blocks
23. Module files: `import`

Other more advanced topics:

- Procedural Programming vs. Functional Programming vs. Object Oriented Programming (OOP)
- Function `args` and `kwargs`
- Generators: `yield`
- Package file hierarchy
- [poetry](https://python-poetry.org)

# Data Toolkit
If you cannot manipulate data, everything else in this course is moot. Familiarizing yourself with the tools listed below (I highly recommend going in the order presented) will prepare you to work with almost any data at any level in the Python environment. The most essential learning goals are listed along with each tool.

1. [list](https://docs.python.org/3/tutorial/introduction.html#lists): You will be able to work with lists of arbitrary items and use indexing/slicing to manipulate a subset of items from the list.
2. [dict](https://docs.python.org/3/tutorial/datastructures.html#dictionaries): You will be able to work with (key, value) pairs.
3. [numpy](https://numpy.org): You will be able to work with N-dimensional arrays (e.g., initialization, indexing/slicing, views, math, aggregation, logical masks, matrix multiplication). You will appreciate the power of N-D arrays for many types of data, and the speed and clarity of numpy vs. pure python.
4. [pandas](https://pandas.pydata.org): You will be able to work with dataframes (i.e., tables; indexing/slicing, to/from numpy, groupby, plot). You will appreciate the power of pandas dataframes for exploratory data analysis and see that pandas far exceeds the ability of programs like Excel to manage large tabular datasets.
5. [xarray](https://xarray.dev): You will appreciate the usefulness of N-D arrays with labeled dimensions. This is numpy + pandas to the next level.
6. [zarr](https://zarr.dev): You will be able to store data in a self-describing hierarchical format with chunked arrays either locally or in the cloud.
7. [dask](https://www.dask.org): You will be able to perform computations on datasets too large to fit into your local computer memory.

Other resources of interest:

- [pydata](https://pydata.org): Community leveraging python to work with many types of data.
- [parquet](https://parquet.apache.org): A modern and vastly superior format for storing large tabular datasets as compared to comma separated values (.csv).

# Data Visualization
Before jumping into making your own plots, it is imperative to understand that how you present your data can greatly influence what conclusions viewers draw from it. Thus, it is incredibly important that you do not present your data in a way that is misleading. To avoid such pitfalls, you need to be aware of some common ways in which graphs can be misleading as well as some good practices.

- :bangbang: [Misleading graphs](https://en.wikipedia.org/wiki/Misleading_graph)

Familiarizing yourself with the tools listed below (I highly recommend going in the order presented) will enable you to generate quality graphics to visualize your data.

1. [matplotlib](https://matplotlib.org): The most used plotting package in Python. Bonus: It's almost identical to plotting in MATLAB. This is probably the most customizable plotting package out there, so you can get your plots to look exactly how you want them. The downside is that the default plots don't look all that nice, and customizing them requires a lot of code :(
2. [seaborn](https://seaborn.pydata.org): Shortcuts for creating nice looking matplotlib plots from pandas dataframes (i.e., tables).
3. [hvplot](https://hvplot.holoviz.org): Easily create nice looking interactive plots from pandas dataframes (i.e., tables).
4. [napari](https://napari.org/stable/#): Awesome drag-n-drop app for N-dimensional image viewing and analysis. *I recommend creating a new environment in which to install this as it has a lot of dependencies.*

Other resources of interest:

- [plotly](https://plotly.com): Interactive plots. Note that hvplot can be configured to use plotly if you want.
- [bokeh](https://bokeh.org): Interactive plots. Note that hvplot uses bokeh by default.
- [panel](https://panel.holoviz.org): Create dashboard apps in your browser with interactive graphs. I don't have much experience with this, but it looks like it could be a nice option.
- [PySide/PyQt](https://wiki.qt.io/Qt_for_Python): Create graphical user interface (GUI) apps. I personally love Qt, but be warned that this may require a large investment to become reasonably familiar with.

# Statistical Inference
1. [random variables]()
2. [probability]()
3. [joint and conditional probability]()
4. [Bayes Theorem]()
5. [probability distributions]()
6. [maximum likelihood]()
7. [sampling distribution]()
8. [Central Limit Theorem]()
9. [hypothesis testing]()
10. [pitfalls of p-values]()
11. [permutation test]()
12. [confidence interval]()
13. [bootstrap]()

Other resources of interest:

- :bangbang: [Misuse of statistics](https://en.wikipedia.org/wiki/Misuse_of_statistics)

# Linear Models

# Regression

# Classification

# Clustering

# Dimensionality Reduction

# Neural Networks
