# Pitfalls of predicting complex traits from SNPs [Wray et. al. 2013, Nature](https://www.nature.com/articles/nrg3457)

There is increasing interest in making prediction of complex traits using simple genetic variants (SNPs).
Incorrect conclusions at validation stage may lead to poor to no prediction accuracy.

### Limitations of prediction analyses:

__1.  Prediction of phenotypes from genetic markers:__

Assuming that the estimated h<sup>2</sup> is a true reflection of the population parameter, then h2 is the upper limit of the phenotypic variance explained by a linear predictor (R2) based on DNA markers such as SNPs, and a genetic predictor can thus never fully account for all phenotypic variation.

In practice, not all environmental factors are identified (and some factors that are classified as ‘environment’ may simply be stochastic events).

In agriculture, genetic risk prediction is mostly geared towards selection of breeding stock on the basis of estimates of additive genetic values (that is, estimated breeding values) in the parent generation; the aim is to elicit average changes in the phenotype of the offspring generation. That is, the impact of genetic prediction is naturally at the level of a group rather than an individual.

__2.  Variance explainable by markers:__

SNPs are are typically not the causal variants for a phenotype, they are just in LD with the causal variant.

If a genetic variant is associated with fitness, selection will drive one allele to low frequency. 

The larger the effect of a SNP on fitness, the lower the frequencies of the causal alleles are expected to be.

The difference between the variance explained by genome-wide-significant SNPs (hGWS) and heritability estimates from family studies (h2) has been called the ‘missing heritability’, and the difference between hGWS and h2M has been described as the  ‘hidden heritability’.
h<sub>GWS</sub> < h<sup>2</sup><sub>M</sub> < h<sup>2</sup>

In livestock populations, smaller effective population size leads to long range LD, and as a result causal variant explain a large proportion of heritability, and hence even rare alleles can be predicted by a linear combination of SNPs that are in LD with the causal variant.

when the SNPs are fitted together with a pedigree, as much as half of the genetic variance is explained by the pedigree and not by the SNPs.

With WGS, since causative mutations will be present in data, proportion of variance explained by SNPs will approach h<sup>2</sup>.

__3. errors in the estimated effects of the markers:__



