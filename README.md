# Project 1
Ann-Elise Hafvenström & Linn Isberg

The paper: Alexandrov et al. 2013, "Signatures of mutational processes in human cancer" introduced Signature 3 (SBS3), associated with defective homologous-recombination repair and BRCA1/2 loss. 

This project aims to model the number of SBS3-shaped mutations in a cohort of 119 breast cancer genomes. A simple Poisson model is used to describe the data from our chosen paper. The project also investigates to what extent the model can reproduce the observed data and analyzes the uncertainty of the estimated parameter.

A Poisson distribution is used to model the total number of SBS3-shaped mutations i the cohort. This was chosen because each of the N mutations independently has a small probability θ of being SBS3 shaped, which is a typical setup for a Poisson count. Our chosen random variable K = the mutational signature count in breast cancer sample. 

The generative model proposed is K∼Poisson(N⋅θ). 

The parameter: θ [dimensionless, [0,1]]: the fraction of all mutations in the cohort that are SBS3-shaped. A larger θ means more mutations are attributable to defective homologous-recombination repair. 
N is fixed to the cohort's own total mutation count. 





Model a 96-trinucleotide spectrum as a mixture of signature mutations and fits the mixture weight for one cancer type. 
Each signature is a probability distribution over 96-mutation types
observed mutation-counts in a sample = sum over signatures of(weight * signature spectrum)
xi - N Ek ((wk)*(sk,i))

BRCA1 and BRCA2 observed probably in signature 3 which is controlled in the breast cancer type samples. (P = 1.6 × 10⁻⁸ for breast cancer)") One-parameter model using Poisson
