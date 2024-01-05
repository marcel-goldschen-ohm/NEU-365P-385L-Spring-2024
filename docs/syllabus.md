# 🚧 Syllabus
NEU 365P/385P - Spring 2024 - Programming and Data Analysis for Modern Neuroscience

⚠️ *The syllabus is subject to change as the course progresses depending on my judgement.* This is because I modify my course every year to make it that much better for you. That said, the current syllabus is at least a reasonable approximation of what the final course will look like.

Python intro
---
1. <details><summary>Jan 16 T - Course intro and python intro</summary>
  
     - You will get a brief overview of the course.
     - You will be able to use `conda` to manage python environments.
     - You will be able to use `conda` and `pip` to manage python packages within each environment.
     - You will be able to run python code in a Jupyter notebook.
     - You will understand some basic python code:
       - Variables
       - Types
       - Basic operations
       - Logical comparisons
       - Comments

   </details>
2. <details><summary>Jan 18 R - Python basics</summary>
  
     - You will understand some basic python code:
       - `if` code blocks
       - Nested code blocks
       - `list` and index/slice
       - `dict` (key,value) pairs
       - `for` and `while` loops
       - Functions (optional named and default arguments)
       - Assignment vs mutation

   </details>
3. <details><summary>Jan 23 T - Classes and modules</summary>
  
     - You will understand how to compartmentalize python code beyond simple functions:
       - `class` code blocks
       - Class `__init__` method
       - Class instance (`self`) vs class template
       - Class inheritance
       - Modules

   </details>

Working with data
---
4. <details><summary>Jan 25 R - Numpy N-dimensional arrays and matplotlib</summary>
  
     - You will appreciate that many types of data can be represented as N-dimensional arrays.
     - You will understand how to work with `numpy` N-dimensional arrays.
       - Array initialization (e.g., `zeros`, `ones`, `random`) and `shape`
       - Element-wise array math
       - Index and slice
       - Logical masks
       - Reductions (e.g., `min`, `max`, `mean`, `var`)
       - Broadcasting
     - You will appreciate that `numpy` can be *much much* faster than raw python.
     - You will appreciate that without `numpy` we would not use python for most data analysis.
     - You will be able to visualize data with simple plots using `matplotlib`.

   </details>
5. Jan 30 T - Pandas tables and hvplot

Probability and random variables
---
6. Feb 01 R - Probability distributions

Resampling
---
7. Feb 06 T - Bootstrap confidence interval and permutation test

Model optimization
---
8. Feb 08 R - Curve fitting and maximum likelihood estimation (MLE)

Review
---
9. Feb 13 T - Review

Linear model
---
10. Feb 15 R - Linear regression

Generalized linear model (GLM)
---
11. Feb 20 T - Poisson and logistic regression

Nonlinear model
---
12. Feb 22 R - Polynomial and k-nearest neighbors (KNN) regression

Model selection
---
13. Feb 27 T - Bias/Variance tradeoff and cross validation

Regularization
---
14. Feb 29 R - Ridge and lasso regression

Classification
---
15. Mar 05 T - Confusion matrix, ROC curve, support vector machine (SVM)

Ensemble model
---
16. Mar 07 R - Random forest classifier and extreme gradient boosting (XGBoost)

🏖️ Spring break
---
- Mar 12 T - SPRING BREAK
- Mar 14 R - SPRING BREAK

Time series (i.e., sequences)
---
17. Mar 19 T - Time series and convolution

Simulating a neuron
---
18. Mar 21 R - Leaky integrate and fire (LIF) neuron
19. Mar 26 T - LIF neuron with synaptic input

Hidden Markov model
---
20. Mar 28 R - Hidden Markov model (HMM) for an ion channel
21. Apr 02 T - HMM for a DNA sequence

Clustering
---
22. Apr 04 R - K-means, gaussian mixture model (GMM), DBSCAN, etc.

Dimensionality reduction
---
23. Apr 09 T - Principal component analysis (PCA)
24. Apr 11 R - RNAseq lab with PCA (or UMAP or t-SNE) and clustering

Neural network
---
25. Apr 16 T - Feedforward neural network (FNN)
26. Apr 18 R - Feedforward neural network (FNN)
27. Apr 23 T - Recurrent neural network (RNN)
28. Apr 25 R - Long/Short term memory (LSTM) neural network
