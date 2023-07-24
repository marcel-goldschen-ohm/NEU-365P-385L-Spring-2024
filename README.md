# NEU-365P-385L-Spring-2024
Programming and Data Analysis for Modern Neuroscience

# Python Environment
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
  - `conda` (e.g., [miniconda](https://docs.conda.io/en/main/miniconda.html)) <-- Also manages Python!
  - `pip`: [Python Package Index (PyPI)](https://pypi.org)
- Python Virtual Environments
  - conda environments
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

- Functional Programming vs. Object Oriented Programming (OOP)
- Function `args` and `kwargs`
- Generators: `yield`
- Package file hierarchy
- [poetry](https://python-poetry.org)

# Data Toolkit
Familiarizing yourself with the tools listed below (I highly recommend going in the order presented) will prepare you to work with almost any data at any level in the Python environment. The most essential learning goals are listed along with each tool.

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
1. [matplotlib](https://matplotlib.org)
2. [seaborn](https://seaborn.pydata.org)
3. [hvplot](https://hvplot.holoviz.org)
4. [napari](https://napari.org/stable/#)

Other resources of interest:

- :bangbang: [Misleading graphs](https://en.wikipedia.org/wiki/Misleading_graph)
- [panel](https://panel.holoviz.org)
- [PySide/PyQt](https://wiki.qt.io/Qt_for_Python)

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
