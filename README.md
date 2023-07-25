# NEU-365P-385L-Spring-2024
Programming and Data Analysis for Modern Neuroscience

- [Setup your Python environment](setup-your-python-environment.md)
- [Keep up-to-date with the course GitHub repository](#keep-up-to-date-with-the-course-github-repository)
- [Python environment overview](#python-environment-overview)
- [Python Basics](#python-basics)
- [Data Toolkit](#data-toolkit)
- [Data Visualization](#data-visualization)
- [Statistical Inference](#statistical-inference)

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
