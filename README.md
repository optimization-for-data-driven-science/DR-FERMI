# Distributionally Robust Fair Empirical Risk Minimization (DR-FERMI)
DR-FERMI is a distributionally robust stochastic optimization framework for handling distribution shifts in fair empirical risk minimization tasks. The distribution shift happens when the distribution of the test data (target domain) is different from the distribution of the training data (source domain). The main advantage of DR-FERMI over the previous methods is that it does not assume the availability of the causal graph describing the interaction of non-sensitive predictors, sensitive attributes, and the target variable. Further, we do not consider specific types of distribution shifts such as demographic shifts, covariate shifts, or label shifts in formulating the problem and developing algorithms.

## Issues with Conventional Algorithmic Fairness Approaches 
A common assumption of algorithmic fairness approaches is that the training data has the same distribution as the test data. However, such an assumption might not hold in many practical problems. For instance, ACS PUMS Data is a collection of new datasets distributed over different states. Learning a fair model (demographic parity of equalized odds) in one US state, such as California, does not guarantee that the model remains fair in other states. In other words, fairness is not transferable from the source domain (training data) to the target domain (test data) when the distribution of the data shifts in the test phase. 

## Distribtuionally Robust Formulation of Fair Empirical Risk Minimization
The Fair Empirical Risk Minimization with Exponential Renyi Mutual Information (ERMI) as the measure of fairness violation seeks to optimize the following problem:

To handle distribution shifts with respect to the fairness measure, we define the uncertainty set over the matrix Q using Lp norms:

## Experiments on ACS Data
The implementation of DR-FERMI on the ACS Data for L1 and L2 norms are avalable at **DR-FERMI_ACS Data.ipynb** notebook.
