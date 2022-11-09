# Final Project Information (Fall 2022)

## Schedule & Requirements

### Requirements

The goal of the final project is for you to build a complete system that accomplishes a realistic task while ensuring differential privacy. Final projects will be completed in groups of 1-3. The deliverables for the project will be as follows:

- A *project proposal* of 1 paragraph, describing:
  - Who is in your group
  - What problem you're trying to solve
  - A brief description of the approach you plan to use (e.g. what data; what algorithms)
- A *project writeup* of 1-3 pages, containing:
  - A problem statement
  - A technical description of your solution, with emphasis on anything that makes your solution unique; your description should be sufficient to enable the reader to *reproduce your implementation*
  - A description of the results - if you've evaluated your implementation on real data, describe how well it works
  - If your project is a critique of an existing system, a **longer writeup of at least 4-5 pages is expected** instead of an implementation
- A *project presentation video* of about 5 minutes
  - Your presentation should include slides or a demo
  - All group members should present some part of the project
  - Your presentation should cover the same material as your writeup, and be understandable to anyone who has taken this class (i.e. related work that was not covered in class should be explained in your presentation)
- Your *implementation*, in whatever form you choose
  - You can use any language or libraries you prefer, but a Python notebook will make grading easier
  - If your project is a critique of an existing system, no implementation is required (unless it helps support your conclusions)

### Schedule & Grading

The final project is worth 10% of your final grade. The schedule for final project deliverables, and the contribution of each one to the grade you receive for the final project, are as follows:

| Deliverable                | Due Date                      | Grade Percent | Turn In    |
| ---------------------:     | ----------------------------- | ------------- | ---------- |
| Project Proposal           | 11/18/22 by 11:59pm           | 10%           | Blackboard |
| Project Presentation Video | 12/12/22 by 11:59pm           | 30%           | Blackboard |
| Implementation + Writeup   | 12/12/22 at 11:59pm           | 60%           | Blackboard |


### Graduate Students

Graduate students (and undergraduates taking the course for graduate credit) will be expected to develop a more ambitious final project (a more sophisticated algorithm or approach; a larger or more challenging dataset; or a more detailed analysis of experimental results).

## Project Ideas

You're welcome to work on any project interesting to you, as long as it's related to data privacy. Suggested examples are below.

### Summary and critique of a differential privacy guarantee (suggested option)

  - Consider [Damien Desfontaines' list of real-world differential privacy deployments](https://desfontain.es/privacy/real-world-differential-privacy.html)
  - Consider the privacy guarantee given by the system
    - Privacy parameters
    - Unit of privacy
    - Possible failures of the guarantee
    - Possible attacks on the system
  - Consider the way the guarantee is communicated
    - Is there missing information?
    - Is the communication misleading?

### Analysis of a *new* dataset, with differential privacy (suggested option)

#### Sources of data

  - [Kaggle datasets](https://www.kaggle.com/datasets)
  - [COMPAS dataset](https://www.kaggle.com/danofer/compass)
  - [Census data](https://data.census.gov/cedsci/advanced)
  - [NIST Diverse Communities Data Excerpts](https://github.com/usnistgov/SDNist/tree/main/nist%20diverse%20communities%20data%20excerpts)
  - [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets.php)

#### Analysis ideas
  - For a workload of queries on several columns, compare the Laplace and Gaussian mechanisms
  - Analyze clipping parameters for some of the columns (e.g. for summation)
  - Try to predict one column using the rest of them using differentially private gradient descent
  - Generate synthetic data using private marginals
  - Try to answer clearly important questions about the data, with differential privacy
    - Census: populations; average incomes; use Laplace and/or Gaussian mechanisms
    - COMPAS: connection between race and score (e.g. following [Propublica's analysis](https://github.com/propublica/compas-analysis/blob/master/Compas%20Analysis.ipynb)); use Laplace and/or Gaussian mechanisms
    - Kaggle datasets: differentially private gradient descent
    - UCI ML datasets: differentially private gradient descent (look for larger datasets, > 1000 samples)

### Implementation of a *new* differentially private algorithm (challenging)

  - Multi-column synthetic data using private marginals
  - Hierarchical solutions for answering range queries (e.g. Census "top-down" algorithm)
  - Variants of differentially private gradient descent (e.g. minibatching)
  - Iterative algorithms for synthetic representations (e.g. [MWEM](https://arxiv.org/pdf/1012.4763.pdf))


