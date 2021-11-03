# SVM-Optimization

Support Vector Machines (SVMs) are a well established technique for the solution of classification problems in machine learning. A mathematical description of Support Vector Classifiers (SVCs) is provided in the SMO notebook.

Two methods are implemented to optimize SVCs (to solve non-linear classification problems):

- Sequential Minimal Optimization (SMO),
- Primal Estimated Sub-GrAdient SOlver for SVM (PEGASOS).

# SMO

SMO is a popular method for optimizing SVCs. It solves the quadratic programming (QP) problem (expressed in the dual form) by breaking it down into a series of smallest possible subproblems. The implementation is based on [John Platt's original paper](https://www.microsoft.com/en-us/research/wp-content/uploads/2016/02/tr-98-14.pdf). 

# PEGASOS

PEGASOS is an effective stochastic sub-gradient descent algorithm for solving the primal objective function. The implementation is based on the kernelized PEGASOS algorithm from [original paper](https://link.springer.com/article/10.1007/s10107-010-0420-4).

# Evaluation

The implementations are tested on the moons dataset from ```Scikit-learn```. For both methods, we plot the decision boundary and a confusion matrix showing the classification results.
