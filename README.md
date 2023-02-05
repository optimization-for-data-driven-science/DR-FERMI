# Distributionally Robust Fair Empirical Risk Minimization

## Issues with Conventional Algorithmic Fairness Approaches 
A common assumption of algorithmic fariness approaches is that the training data has exactly the same distribution as test data. Such assumption might not hold
in many practical problems. For instance, ACS PUMS Data is a collection of new datasets distributed over different states. Learning a fair model (demographic parity of equalized odds) in one state such as California does not guarantee that the model remains fair in other states. In other words, the fairness is not transferable from the source domain (training data) to the target domain (test data) when the distribution of the data shifts in the test phase. 

## Distribtuionally Robust Formulation of Fair Empirical Risk Minimization
The Fair Empirical Risk Minimization with Exponential Renyi Mutual Information (ERMI) as the measure of fairness violation seeks to optimize the following problem:

To handle distribution shifts with respect to the fairness measure, we define the uncertainty set over the matrix Q using Lp norms:

## Experiments on ACS Data
The implementation of DR-FERMI on the ACS Data for L1 and L2 norms are avalable at DR-FERMI_ACS **Data.ipynb** notebook.
