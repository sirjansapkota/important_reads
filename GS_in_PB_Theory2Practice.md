# Genomic selection in plant breeding: from theory to practice  [Jannink et. al. 2010](https://www.ncbi.nlm.nih.gov/pubmed/20156985)

The weaknesses of traditional MAS come from the way MAS splits the task into two components, first identifying QTL and then estimating their effects.

QTL identification methods can make MAS poorly suited to crop improvement: 

__(i)__ biparental populations may be used that are not representative and in any event do not have the same level of allelic diversity and phase as the breeding program as a whole;

__(ii)__ the necessity of generating such populations is costly such that the populations may be small and therefore underpowered;

__(iii)__ validation of discoveries is then warranted, requiring additionaleffort;

__(iv)__ the separation of QTL identification from estimation means that estimated effects will be biased, and small-effect QTL will be missed entirely as a result of using stringent significance thresholds.

_The GEBVs say nothing of the function of the underlying genes but they are the ideal selection criterion._

### GS METHODS

At high marker densities:

=> it was assumed that linkage phase between markers or haplotype blocks of markers and causal polymorphisms would be consistent across families so that population-wide estimates of marker effects would be meaningful.

=> But there may be a high degree of correlation or multicollinearity between the predictors/markers.

=> In so-called ‘large p, small n’ problems, standard multiple linear regression cannot be used without __variable selection__, which __conflicts with the original goal of avoiding marker selection__.

=> An important __danger in__ the development of a __prediction__ model __is overfitting__: an overfitted __model can exaggerate minor fluctuations__ in the data and will generally have poor predictive ability. That's why RR, BLUP, BayesR, KernelR, and ML methods are used.

=> This parameterization, where all effects are assumed to have equal variance, is also called ridge regression. [Whittaker et. al.], Note that assuming all marker effects are drawn from the same distribution does not mean the effects are all equal but that they are all equally shrunken toward zero.

__BayesA__: each effect _i_ is normally distributed with its own variance, whereas variance parameters are drawn from scaled inverted chi-squared distribution.

__BayesB__: A further probability _pi_ is given that the marker has no effect at all.

_Further accounts of Bayesian alphabet in_ Gianola _et al_. 2009: Additive genetic variability and the Bayesian alphabet.

__Random Forest__ is an ensemble predictor consisting of a collection of tree-structured predictors, where each tree in the ensemble is ‘grown’ on the basis of a bootstrapped sample of the training dataset. Each tree individually predicts the target response and the ‘forest’ (i.e. the ensembles of ‘trees’) predicts the target response as an average of individual tree predictions.





