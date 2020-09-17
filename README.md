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



##Task 2

**Hidden Markov Model**

Hidden Markov Model (HMM) is a statistical Markov model in which the system being modeled is assumed to be a Markov process – call it {\displaystyle X}X – with unobservable ("hidden") states. HMM assumes that there is another process {\displaystyle Y}Y whose behavior "depends" on {\displaystyle X}X. The goal is to learn about {\displaystyle X}X by observing {\displaystyle Y}Y. HMM stipulates that, for each time instance {\displaystyle n_{0}}n_{0}, the conditional probability distribution of {\displaystyle Y_{n_{0}}}{\displaystyle Y_{n_{0}}} given the history {\displaystyle \{X_{n}=x_{n}\}_{n\leq n_{0}}}{\displaystyle \{X_{n}=x_{n}\}_{n\leq n_{0}}} must not depend on {\displaystyle \{x_{n}\}_{n<n_{0}}}{\displaystyle \{x_{n}\}_{n<n_{0}}}.

Hidden Markov models are known for their applications to reinforcement learning and temporal pattern recognition such as speech, handwriting, gesture recognition, part-of-speech tagging, musical score following, partial discharges and bioinformatics.

Let {\displaystyle X_{n}}X_{n} and {\displaystyle Y_{n}}Y_{n} be discrete-time stochastic processes and {\displaystyle n\geq 1}n\geq 1. The pair {\displaystyle (X_{n},Y_{n})}{\displaystyle (X_{n},Y_{n})} is a hidden markov model if

* {\displaystyle X_{n}}X_{n} is a Markov process and is not directly observable ("hidden");
* {\displaystyle \operatorname {\mathbf {P} } {\bigl (}Y_{n}\in A\ {\bigl |}\ X_{1}=x_{1},\ldots ,X_{n}=x_{n}{\bigr )}=\operatorname {\mathbf {P} } {\bigl (}Y_{n}\in A\ {\bigl |}\ X_{n}=x_{n}{\bigr )},}{\displaystyle \operatorname {\mathbf {P} } {\bigl (}Y_{n}\in A\ {\bigl |}\ X_{1}=x_{1},\ldots ,X_{n}=x_{n}{\bigr )}=\operatorname {\mathbf {P} } {\bigl (}Y_{n}\in A\ {\bigl |}\ X_{n}=x_{n}{\bigr )},}
for every {\displaystyle n\geq 1,}{\displaystyle n\geq 1,} {\displaystyle x_{1},\ldots ,x_{n},}{\displaystyle x_{1},\ldots ,x_{n},} and an arbitrary (measurable) set {\displaystyle A}A.

Terminology
The states of the process {\displaystyle X_{n}}X_{n} are called hidden states, and {\displaystyle \operatorname {\mathbf {P} } {\bigl (}Y_{n}\in A\ {\bigl |}\ X_{n}=x_{n}{\bigr )}}{\displaystyle \operatorname {\mathbf {P} } {\bigl (}Y_{n}\in A\ {\bigl |}\ X_{n}=x_{n}{\bigr )}} is called emission probability or output probability.

