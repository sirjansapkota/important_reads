## Excerpts from Likelihood, Bayesian and MCMC Methods

By Daniel Sorenson and Daniel Gianola, 2002

### Introduction to Bayesian Inference

Two types of data encountered in breeding:

1. field data/records : phenotypic observations taken in field/farm, available in massive amount.

2. data from genetic selection experiments: limited in amount, data from carefully conducted controlled experiments.

[Asymptotic theory](https://en.wikipedia.org/w/index.php?title=Asymptotic_theory_(statistics)&gettingStartedReturn=true): In statistics, asymptotic theory, or large sample theory, is a framework for assessing properties of estimators and statistical tests. Within this framework, it is typically assumed that the sample size n grows indefinitely; the properties of estimators and tests are then evaluated in the limit as n → ∞. In practice, a limit evaluation is treated as being approximately valid for large finite sample sizes, as well.

Assuming joint normality of additive genetic effects and phenotypic values is maintained. Quanititative geneticists in the light of the question: “How much genetic change has taken place in the course of
selection?” would:

First, estimate components of variance (or covariance) in the base population using either full or marginal likelihood (for marginal would lead to REML estimates of parameters).

Second, conditionally on those estimates, they would obtain best linear unbiased predictions (BLUP) of additive genetic effects (In current case, probably as genomic estimated breeding values).


=> __What is a BLUP?__

Theoretically, BLUP is the linear combination of the observations that minimizes prediction error variance in the class of linear functions whose expected value is equal to the expected value of the predictand (the genetic effects).

BLUP can be derived only if the dispersion parameters (variance and covariance components) are known, at least to proportionality. In case of estimates values from data like REML, the resulting empirical BLUP is no linear or best, and only unbiased when random sampling and absence of selection or assortative mating.
__This problem is often ignored by Quantitative geneticists, and they proceed to predict genetic means for different generations or cohorts using the empirical BLUP.__

Complications caused by nonrandom sampling mechanisms are encountered, as parents of a subsequent generation are not chosen at random. Unless selection is ignorable, in some sense, inferences are liable to be distorted.

__Important questions in quantiative genetcs__: Should one use the conditional distribution of the random effects, given the data, ignoring selection and the error of estimation of the parameters for inferring genetic change?

##### Reasoning for Bayesian analysis:
If one wishes to know what to expect, at least in the frequentist sense of hypothetical repeated sampling, the only answer would seem to reside in simulating all conceivable selection schemes and designs, for all possible values of the parameters. Clearly, this is not feasible. Simulations would need to be sensibly restricted to experimental settings and to parameter values that are likely to reflect reality. This implies that at least something must be known about the state of nature, before experimentation. However, there is always uncertainty, ranging from mild to large. An alternative is to adopt the Bayesian point of view.

In Bayesian point of view:
- all unknown quantities in a statistical system are tread as random variables.

- reflecting subjective uncertainty measured by a proabability distribution.

- unknown may include parameters, random effects, unobserved data, sampling distributions, or entire model itself.

- combined previously known information in statistical ensemble with the information data (prior probability distribution) to obtain posterior distribution.

- inferences are made using standard probability calculus techniques.

- The result is interpreted probabilistically,  example: to infer the mean one would say “the posterior probability that μ is between aand b is so much”.

##### [Bayes' theorem](https://en.wikipedia.org/wiki/Bayes%27_theorem):

The standard result of conditional probability is Bayes theorem when applied to specific problem of inferring "causes" from "effects". Also called __"inverse probability"__.

It states that the probability of a cause or hypothesis Hi, given evidence Ej , is proportional to the product of the prior probability assigned to the hypothesis, p(Hi), times the conditional probability of observing the effect Ej under hypothesis Hi.

The distribution is called posterior probability distribution and the demoninator in the equation is called normalizing constant.








