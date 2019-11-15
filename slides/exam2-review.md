# Exam 2 Topic List

## Variants of Differential Privacy

- Advantages compared to ε, (ε,δ)-DP
- Rényi DP
- Zero-concentrated DP
- Conversion from variants to (ε,δ)-DP

## Algorithm Design

- Exponential mechanism
- Sparse vector technique
- Clipping (methods; information loss vs sensitivity)
- Adaptive clipping
- Splitting the privacy budget

## Differentially Private Machine Learning

- Types:
  - Input perturbation
  - Output perturbation
  - Gradient perturbation
  - Objective perturbation

- Gradient perturbation (noisy gradient descent)
  - What is gradient descent
  - What is the format of a linear model
  - How to bound the sensitivity of the gradient (clipping the gradient vs clipping the samples)
  - Composition issues

## Local Differential privacy

- Tradeoffs of LDP
- Randomized response
- Unary encoding

## Synthetic Data

- Range queries
- Synthetic representations vs synthetic data
- The histogram representation for range queries
- Tradeoffs in the histogram representation (e.g. large vs small bins)
- Using histograms as probability distributions to generate synthetic data
- 1-way vs 2-way vs n-way marginal distributions
  - Advantage: n-way preserves correlation
  - Disadvantage: as n grows, counts shrink, and noise becomes overwhelming

