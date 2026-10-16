# Bayesian weighted one inflated beta regression models for AMR probability outcomes

Example code accompanying Stanton et al. (2026) (Modelling trends in phenotypic 
*Escherichia coli* antimicrobial resistance in ruminant livestock populations), 
demonstrating a weighted zero inflated beta regression modelling approach that can be
used to model sample level *E. coli* antimicrobial resistance probability. To 
adjust for changing test sensitivity associated with variation in *E. coli*
abundance, the nonlinear Poisson regression described in Vass et al. (2026) 
was adapted to incorporate censored count data. Posterior estimates of the
proportion of AMR within each sample are extracted and a threshold is applied to 
estimate the probability of antimicrobial resistance being present but 
unobserved in AMR negative samples. Log transformed inverse variance weighting 
is applied to weight probabilities in AMR negative samples. 

An example application of this modelling approach in which the effect of changing 
temperature preceding sampling of the probability of observing resistance is 
included.

## Contents

- `Bayesian_beta_regression_for_AMR_likelihood.Rproj` — RStudio project file
- `model_example_code.Rmd` — model fitting and plotting example
- `data_for_poisson.rds` — example data for modified Vass et al. (2026) Poisson model
- `zi_model_data.Rds` — example data for weighted one inflated beta regression model

## Requirements

- R 
- [RStudio]

### R packages

- `brms`
- `tidyverse`
- `lubridate`
- `naniar`
- `tidybayes`
- `viridis`
- `cowplot`
