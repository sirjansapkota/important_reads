## Breeding and genetic data analysis platforms

### [BrAPI](https://brapi.org) : [Github](https://github.com/plantbreeding/API)
The Breeding API (BrAPI) Project is an effort to create a RESTful specification to enable interoperability among plant breeding databases.
WHAT ARE THE ADVANTAGES OF USING BRAPI?
The Breeding API specifies a standard interface for plant phenotype/genotype databases to serve their data to crop breeding applications. It is a shared, open API, to be used by all data providers and data consumers who wish to participate.

Main features:
 Genotype visualization using [Flapjack](https://ics.hutton.ac.uk/flapjack/) [Citation](https://www.ncbi.nlm.nih.gov/pubmed/20956241)
 Field Data Collection
[BrAPI R module] (https://github.com/CIP-RIU/brapi)
 Data Transfer
 Geographic Visualization
 
### [TASSEL](https://www.maizegenetics.net/tassel) : Trait Analysis by aSSociation, Evolution and Linkage
TASSEL is a software package used to evaluate traits associations, evolutionary patterns, and linkage disequilibrium. Strengths of this software include:
 1. The opportunity for a number of new and powerful statistical approaches to association mapping such as a General Linear Model (GLM) and Mixed Linear Model (MLM). MLM is an implementation of the technique which our recently published Nature Genetics paper - Unified Mixed-Model Method for Association Mapping - which reduces Type I error in association mapping with complex pedigrees, families, founding effects and population structure.
2. An ability to handle a wide range of indels (insertion & deletions). Most software ignore this type of polymorphism; however, in some species (like maize), this is the most common type of polymorphism.

Read more at: [Bradbury et. al. 2007](https://academic.oup.com/bioinformatics/article/23/19/2633/185151)

### [PLINK](http://zzz.bwh.harvard.edu/plink/): Whole genome association analysis toolset

## R packages used for statistics, genetics, breeding and data science
[BreedingSchemeLanguage]:(https://cran.r-project.org/web/packages/BreedingSchemeLanguage/index.html)  [original paper](https://dl.sciencesocieties.org/publications/cs/pdfs/57/3/1347)  Describe and Simulate Breeding Schemes
Users can simulate their planned breeding schemes by using functions that do standard breeding tasks. 

[lme4](https://cran.r-project.org/web/packages/lme4/lme4.pdf): Linear Mixed-Effects Models using 'Eigen' and S4 objects. Useful for variance component analysis like calculation of ANOVA, BLUE/BLUP, broad-sense heritability.

[rrBLUP](https://cran.r-project.org/web/packages/rrBLUP/rrBLUP.pdf): ridge regression Best Linear Unbiased Predictor
Used for marker effects estimation and implementation of genomic prediction and cross validation.

[BGLR](https://cran.r-project.org/web/packages/BGLR/index.html): Bayesian Genomic Linear Regression
Useful for implementing bayesian inference in whole genome regression models for variable selection, marker-effects estimation and genomic prediction using parameteric and semi-parametric approaches.
[Github](https://github.com/gdlc/BGLR-R)

[pegas](https://cran.r-project.org/web/packages/pegas/pegas.pdf): Population and Evolutionary Genetics Analysis System
Functions for reading, writing, plotting, analysing, and manipulating allelic and haplo-typic data, including from VCF files, and for the analysis of population nucleotide se-quences and micro-satellites including coalescent analyses, linkage disequilibrium, popula-tion structure (Fst, Amova) and equilibrium (HWE), haplotype networks, minimum span-ning tree and network, and median-joining networks.

[heritability](https://cran.r-project.org/web/packages/heritability/heritability.pdf): Marker based heritability estimation

[GAPIT](http://www.zzlab.net/GAPIT/gapit_help_document.pdf): Genomic Association and Prediction Integrated Tool
Useful for mixed-effects models for association analysis and prediction.
Common Models: MLM, CMLM, P3D, SUPER

GAPIT  uses R  libraries:  multtest,  gplots,  LDheatmap,  genetics,  EMMREML, scatterplot3d, and  a modified  version  of  the  EMMA  R  package.

[qtl](https://cran.r-project.org/web/packages/qtl/index.html): Tools for Analyzing QTL experiments

[PhenotypeSimulator](https://cran.r-project.org/web/packages/PhenotypeSimulator/index.html): Flexible Phenotype Simulation from Different Genetic and Noise Models
Simulation is a critical part of method development and assessment in quantitative genetics. 'PhenotypeSimulator' allows for the flexible simulation of phenotypes under different models, including genetic variant and infinitesimal genetic effects (reflecting population structure) as well as non-genetic covariate effects, observational noise and additional correlation effects. The different phenotype components are combined into a final phenotype while controlling for the proportion of variance explained by each of the components. For each effect component, the number of variables, their distribution and the design of their effect across traits can be customised. For the simulation of the genetic effects, external genotype data from a number of standard software ('plink', 'hapgen2'/ 'impute2', 'genome', 'bimbam', simple text files) can be imported. The final simulated phenotypes and its components can be automatically saved into .rds or .csv files. In addition, they can be saved in formats compatible with commonly used genetic association software ('gemma', 'bimbam', 'plink', 'snptest', 'LiMMBo'). 

[Genetics](https://cran.r-project.org/web/packages/genetics/index.html): Population Genetics 
Classes and methods for handling genetic data. Includes classes to represent genotypes and haplotypes at single markers up to multiple markers on multiple chromosomes. Function include allele frequencies, flagging homo/heterozygotes, flagging carriers of certain alleles, estimating and testing for Hardy-Weinberg disequilibrium, estimating and testing for linkage disequilibrium, ...

### [TIDYVERSE](https://cran.r-project.org/web/packages/tidyverse/index.html):
Suite of R packages for Data Wrangling and Visualization

### Views
[Statistical Genetics](https://cran.r-project.org/web/views/Genetics.html): Views on R packages for statistical analysis of genetic data.

