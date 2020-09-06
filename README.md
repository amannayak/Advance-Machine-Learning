# Advance-Machine-Learning
New and advance machine learning algorithms are used as part of implementation

## Task 1

**Graphical Model**

A [graphical model](https://en.wikipedia.org/wiki/Graphical_model#:~:text=Bayesian%20network,-Main%20article%3A%20Bayesian&text=In%20general%2C%20any%20two%20sets,separation%20holds%20in%20the%20graph.&text=This%20type%20of%20graphical%20model,Bayesian%20network%2C%20or%20belief%20network.) or probabilistic graphical model (PGM) or structured probabilistic model is a probabilistic model for which a graph expresses the conditional dependence structure between random variables.


**Data Set and why Graphical Model**

Data : [Asia](https://www.bnlearn.com/documentation/man/asia.html) (synthetic) data set by Lauritzen and Spiegelhalter. 

“Shortness-of-breath (dyspnoea) may be due to tuberculosis, lung cancer or bronchitis, or none of them, or more than one of them. A recent visit to Asia increases the chances of tuberculosis, while smoking is known to be a risk factor for both lung cancer and bronchitis. The results of a single chest X-ray do not discriminate between lung cancer and tuberculosis, as neither does the presence or absence of dyspnoea.”

**Standard learning algorithms are not able to recover the true structure of the network because of the presence of a node (E) with conditional probabilities equal to both 0 and 1. Monte Carlo tests seems to behave better than their parametric counterparts.**


**Format**

The asia data set contains the following variables:

* D (dyspnoea), a two-level factor with levels yes and no.

* T (tuberculosis), a two-level factor with levels yes and no.

* L (lung cancer), a two-level factor with levels yes and no.

* B (bronchitis), a two-level factor with levels yes and no.

* A (visit to Asia), a two-level factor with levels yes and no.

* S (smoking), a two-level factor with levels yes and no.

* X (chest X-ray), a two-level factor with levels yes and no.

* E (tuberculosis versus lung cancer/bronchitis), a two-level factor with levels yes and no.
