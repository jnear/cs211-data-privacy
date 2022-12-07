# Exam 2 Topic List

## Local Sensitivity

- Definition & difference from global sensitivity
- Challenges (e.g. leaks information about the data)
- Propose-test-release
- Smooth sensitivity

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

- Why do we need privacy in machine learning?
  - Machine learning models can memorize sensitive training data
- Gradient perturbation (noisy gradient descent)
  - What is gradient descent
  - What is the format of a linear model
  - How to bound the sensitivity of the gradient (clipping the gradient's L2 norm)
  - Composition issues and best privacy variants

## Local Differential privacy

- Tradeoffs of local differential privacy
  - Huge benefit: threat model
  - Huge drawback: accuracy
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
- Challenge of dimensionality

## Units of Privacy

- Definition (in terms of neighboring datasets)
- Evaluating a unit of privacy: "user-level" vs others
- Transforming the unit of privacy
  - Bounding user contribution & adjusting sensitivity

## Tradeoffs and Lessons Learned

- Utility vs. Privacy
  - Still challenging to navigate
  - Still unclear what ε is "good"
- Clipping
  - Noise scale vs information loss
  - Prefer to avoid information loss
- Mechanism Choice
  - For small number of queries, Laplace mechanism has the best accuracy
  - For many queries at once, use the vector-valued Gaussian mechanism and L2 sensitivity
- Composition
  - Advanced composition is *worse* below ~70 queries
  - RDP and zCDP are always good, but don't offer much benefit for just a few queries
  - When composition matters, prefer RDP or zCDP
- Special tricks to use whenever possible:
  - Sparse Vector Technique (AboveThreshold)
  - Report Noisy Max
- Dimensionality
  - High-dimensional things are hard!
  - Contingency tables
  - Large workloads of queries
  - High-dimensional machine learning (e.g. deep learning)
  - High-dimensional synthetic data (e.g. k-way marginals for large k)
