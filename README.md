# ANDA Day 2 State Space Analysis

## Staff

 - **Lead Trainer**: 
    - Michael Denker, Forchungszentrum Jülich, Germany
 - **Lecturers**: 
   - Hideaki Shimazaki, Graduate School of Informatics, Kyoto University
 - **Teaching Assistants**: 
    - Atle E. Rimehaug, Uni Bonn, Germany
    - Julio Rodino, Forchungszentrum Jülich, Germany
 

## Session Overview

Session Overview


How can we characterise the statistical structure of a neural population beyond
the firing rate of individual neurons?

In this hands-on session, we will use the pairwise maximum-entropy (Ising) model
to describe the joint activity of small neural populations represented as binary
spike patterns. We will work with simulated data where the ground-truth
parameters are known. We will begin by exploring the model's natural parameters:
neuron biases and pairwise couplings. We learn how they shape the distribution over spike
patterns. We will then fit the model using an EM algorithm and assess how well
pairwise interactions account for population variability using thermodynamic
quantities such as the entropy ratio and KL divergence.

In the second part, we extend the model to non-stationary data. A state-space
formulation treats the parameters as a hidden process evolving over time and
estimates them with a Kalman filter and backward smoother. We will track dynamic
correlations, quantify posterior uncertainty, and examine how thermodynamic
signatures change when neural interactions fluctuate.

The aim is to build intuition for what the model parameters represent, when
pairwise interactions matter, and what the algorithm can and cannot resolve given
limited data.

## Tools
- [SSLL](https://github.com/tomxsharp/ssll): state-space log-linear model for estimating time-varying spike-train correlations