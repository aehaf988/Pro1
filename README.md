# Project 1
Ann-Elise Hafvenström & Linn Isberg

The paper: Alexandrov et al. 2013, "Signatures of mutational processes in human cancer" introduced Signature 3 (SBS3), associated with defective homologous-recombination repair and BRCA1/2 loss. 

This project aims to model the number of SBS3-shaped mutations in a cohort of 119 breast cancer genomes. The 96-trinucleotide spectrum is modelled as a mixture of signature mutations and fits the mixture weight for one cancer type. A simple Poisson model is used to describe the data from our chosen paper. SBS3 is strongly enhanced BRCA1/BRCA2 associated breast tumours (P = 1.6 × 10⁻⁸ for breast cancer). The generative model proposed is K∼Poisson(N⋅θ) where N = the total mutation count in the cohort, and θ = the SBS3 rate per mutation. 

The forward simulation: We simulated(theta, N_total, rng) and drew one Poisson observation. A histogram over 10,000 drew at θ^ visualizes the sampling distribution.

The backward validation: We picked a known θtrue, simulated K from the model and refit θ^ on each simulation. We then checked across 1,000 trials that the estimator was unbiased (bias≈0)and that the exact 95% CI covered θtrue about 95% of the time.

