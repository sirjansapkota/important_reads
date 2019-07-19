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

Assuming that the estimated _h<sup>2</sup>_ is a true reflection of the population parameter, then ___h<sup>2</sup>_ is the upper limit of the phenotypic variance explained by a linear predictor (_R<sup>2</sup>_) based on DNA markers__ such as SNPs, and a genetic predictor can thus never fully account for all phenotypic variation.

In practice, not all environmental factors are identified (and some factors that are classified as ‘environment’ may simply be __stochastic events__ like _population structure_).

In agriculture, genetic risk prediction is mostly geared towards selection of breeding stock on the basis of estimates of additive genetic values (that is, estimated breeding values) in the parent generation; _the aim is to elicit average changes in the phenotype of the offspring generation_. That is, the impact of __genetic prediction is naturally at the level of a group rather than an individual__.

__2.  Variance explainable by markers:__

SNPs are are typically not the causal variants for a phenotype, they are __just in LD with the causal variant__.

_If a genetic variant is associated with fitness, _election will drive one allele to low frequency_.
The __larger the effect__ of a SNP on fitness, the __lower the frequencies of the causal alleles__ are expected to be. [Maintaining evolvability](https://www.ncbi.nlm.nih.gov/pubmed/19147924)

The difference between the variance explained by genome-wide-significant SNPs (_h<sub>GWS</sub>_) and heritability estimates from family studies (_h<sup>2</sup>_) has been called the __‘missing heritability’__, and the difference between _h<sub>GWS</sub>_ and _h<sup>2</sup><sub>M</sub>_ has been described as the  __‘hidden heritability’__.
___h<sub>GWS</sub> < h<sup>2</sup><sub>M</sub> < h<sup>2</sup>___

In livestock populations, _smaller effective population size leads to long range LD_, and as a result causal variant explain a large proportion of heritability, and hence even rare alleles can be predicted by a linear combination of SNPs that are in LD with the causal variant.

when the SNPs are fitted together with a pedigree, __as much as half of the genetic variance is explained by the pedigree__ and not by the SNPs.

With WGS, since causative mutations will be present in data, _proportion of variance explained by SNPs will approach h<sup>2</sup>_.

__3. errors in the estimated effects of the markers:__

Sample of finite size, and so the effects are estimated with some __sampling error__.

Complex traits are controlled by a large number of largely unknown loci.
The _true effects of most SNPs are small_, and so the _accuracy_ with which these effects are estimated _is low_ unless a large discovery sample is used.

Correlation (prediction accuracy) is a function of effective population size (effective chrom. seg.), heritability, and sample size. So, it is __difficult to estimate the effect of rare variants__.

__4. statistical methods in the discovery sample:__

use of arbitary p-value threshold for selection of predictors, and estimating effect of one SNP at a time is not optimal.

Methods that model the distribution of SNP effects and the correlation between SNPs in the presence of single as well as multiple causal variants will be more accurate.

### Pitfalls of the analysis

__Pitfall 1: validation and discovery sample overlap.__
Lack of independence of validation and discovery sample.

When the number of SNPs in the predictor is large and the sample size is small, the discovery R2 can be very high by chance and can be a gross overestimation of the true variance explained by the predictor when applied in an independent sample.

Applying the incorrect validation procedure results in over-estimation of the accuracy of the prediction (or over-fitting).

The remedy to this pitfall is to use external validation. It is important to avoid the pitfall of updating the predictor on the basis of results derived from the validation sample.

__Pitfall 2: the validation sample.__

If validation sample is closely related to discovery population (training) then the prediction accuracy is overestimated.

_cryptic relatedness_ can inflate prediction accuracy, even when known close relatives are excluded. 

Remedy is to use _conventionally unrelated_ individuals in discovery and validation stages. Relatedness can be estimated using SNP data, so close relatives can be excluded.

In populations with small effective population size, such as some breeds of livestock, all individuals are related. This does not invalidate the prediction, but it does mean that the same prediction accuracy cannot be expected when the prediction equation is applied to another population that is less closely related to the discovery population.

A prediction equation may work well in a genetically diverse population but less well in an application population that is less diverse, such as in commercial strains of a crop.

__Pitfall 3: population stratification similarity.__

Another way in which prediction accuracy can be inflated is if the discovery and validation samples contain similar patterns of population stratification and if the eventual target population is not similarly stratified.

The question of whether this inflation should be viewed as a pitfall depends on the ultimate goal of the analysis.

A practical remedy to problems associated with population stratification is to fit _ancestry principal components_ in the analysis of discovery samples.

A remedy for differential bias is to carry out stringent quality control and/or to validate predictors in a completely independent sample in lieu of tenfold cross-validation.

If the application sample is an outlier on the PCA, then the prediction accuracy in the target may be less than expected from the validation procedure.

__Pitfall 4: expectation of equality of R<sup>2</sup> and h<sup>2</sup><sub>M</sub>.__

SNP or chip heritability: an unbiased estimate of the variance explained by markers h<sup>2</sup><sub>M</sub> is achieved by correlating phenotypic similarity between pairs of individuals with their SNP-based genotypic similarity.

With ever-larger sample sizes, the size of the error terms in the SNP effect estimates will be reduced, and the two statistics will converge to the same value.

Improvement in trait prediction as sample size increases depends on the genetic architecture of the trait, in particular how many variants there are with tiny effect sizes.




