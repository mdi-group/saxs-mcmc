[![DOI](https://zenodo.org/badge/818885526.svg)](https://zenodo.org/doi/10.5281/zenodo.13321720)
## Introduction
This is a Python script using Markov Chain Monte Carlo (MCMC) sampling with a neural network surrogate model to predict colloidal interaction parameters (effective charge and Debye length) from a Small Angle X-ray Scattering (SAXS) profile. 

If you use this code in your work, please consider citing the following article:

>Wong K, Runzhang Q, Ye Y, Zhi L, Guldin S, Butler K. Predicting Colloidal Interaction Parameters from Small Angle X-Ray Scattering Curves using Artificial Neural Networks and Markov Chain Monte Carlo Sampling . ChemRxiv. 2024; doi:10.26434/chemrxiv-2024-swz2p-v2

## Contents
- MCMC.ipynb: Code to perform MCMC sampling
- Experimental_Data.dat: Experimentally obtained SAXS data of a gold nanoparticle solution

In order to run the code, you will also need to download the following files from this link: https://www.dropbox.com/scl/fo/xmixk0groja42gd3l2bkc/ANGG2Au59XLZZWhgHAnmElU?rlkey=i6dik3cd6w2tuam7jtwcs6f08&dl=0 
- SAXS_Data.pickle: Contains 250,000 SAXS profiles which were used in training the neural network surrogate
- 2Param_Inverse_Model.h5 - Contains the weights of the trained neural network surrogate for the MCMC sampling

## Citing

```
@misc{saxs-mcmc,
title  = {Predicting Colloidal Interaction Parameters from Small Angle X-Ray Scattering Curves using Artificial Neural Networks and Markov Chain Monte Carlo Sampling},
author = {Wong K, Runzhang Q, Ye Y, Zhi L, Guldin S, Butler K. T.},
url    = {https://github.com/mdi-group/saxs-mcmc/},
doi    = {10.5281/zenodo.13321720},
year   = {2024}
 }
```

## Requirements
The main language is Python 3.9.17.
* Tensorflow: 2.12.0
* EMCEE: 3.1.4
* Corner: 2.2.2
* Seaborn: 0.12.2
* Scikit learn: 1.3.0 
