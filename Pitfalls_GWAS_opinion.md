# Pitfalls of predicting complex traits from SNPs
[Wray et. al. 2013, Nature](https://www.nature.com/articles/nrg3457)

There is increasing interest in making prediction of complex traits using simple genetic variants (SNPs).
Incorrect conclusions at validation stage may lead to poor to no prediction accuracy.

#### Selective Citations:
[Heritability in the genomics era—concepts and misconceptions](https://www.nature.com/articles/nrg2322)

[The genetic interpretation of area under the ROC curve in genomic profiling](http://dx.plos.org/10.1371/journal.pgen.1000864)

[Predicting mutation outcome from early stochastic variation in genetic interaction partners](https://www.nature.com/articles/nature10665)

[Five years of GWAS discovery](https://www.sciencedirect.com/science/article/pii/S0002929711005337?via%3Dihub)

[Comparison of statistical tests for association between rare variants and binary traits.](https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0042530)

[Bayesian statistical methods for genetic association studies.](https://www.nature.com/articles/nrg2615)


### Limitations of prediction analyses:

__1.  Prediction of phenotypes from genetic markers:__

Assuming that the estimated h<sup>2</sup> is a true reflection of the population parameter, then __h<sup>2</sup> is the upper limit of the phenotypic variance explained by a linear predictor (R<sup>2</sup>) based on DNA markers__ such as SNPs, and a genetic predictor can thus never fully account for all phenotypic variation.

In practice, not all environmental factors are identified (and some factors that are classified as ‘environment’ may simply be __stochastic events__ like _population structure_).

In agriculture, genetic risk prediction is mostly geared towards selection of breeding stock on the basis of estimates of additive genetic values (that is, estimated breeding values) in the parent generation; _the aim is to elicit average changes in the phenotype of the offspring generation_. That is, the impact of __genetic prediction is naturally at the level of a group rather than an individual__.

__2.  Variance explainable by markers:__

SNPs are are typically not the causal variants for a phenotype, they are __just in LD with the causal variant__.

_If a genetic variant is associated with fitness, _election will drive one allele to low frequency_.
The __larger the effect__ of a SNP on fitness, the __lower the frequencies of the causal alleles__ are expected to be. [Maintaining evolvability](https://www.ncbi.nlm.nih.gov/pubmed/19147924)

The difference between the variance explained by genome-wide-significant SNPs (h<sub>GWS</sub>) and heritability estimates from family studies (h<sup>2</sup>) has been called the __‘missing heritability’__, and the difference between h<sub>GWS</sub> and h<sup>2</sup><sub>M</sub> has been described as the  __‘hidden heritability’__.
__h<sub>GWS</sub> < h<sup>2</sup><sub>M</sub> < h<sup>2</sup>__

In livestock populations, _smaller effective population size leads to long range LD_, and as a result causal variant explain a large proportion of heritability, and hence even rare alleles can be predicted by a linear combination of SNPs that are in LD with the causal variant.

when the SNPs are fitted together with a pedigree, __as much as half of the genetic variance is explained by the pedigree__ and not by the SNPs.

With WGS, since causative mutations will be present in data, _proportion of variance explained by SNPs will approach h<sup>2</sup>_.

__3. errors in the estimated effects of the markers:__

Sample of finite size, and so the effects are estimated with some __sampling error__.

Complex traits are controlled by a large number of largely unknown loci.
The _true effects of most SNPs are small_, and so the _accuracy_ with which these effects are estimated _is low_ unless a large discovery sample is used.

correlation (prediction accuracy) is a function of effective population size (effective chrom. seg.), heritability, and sample size. So, it is __difficult to estimate the effect of rare variants__.





