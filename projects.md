# NOTE: This information is outdated, and has NOT yet been updated for Fall 2020

# Final Project Information (Fall 2019)

## Schedule & Requirements

### Requirements

The goal of the final project is for you to build a complete system that accomplishes a realistic task while ensuring differential privacy. Final projects will be completed in groups of 1-3. The deliverables for the project will be as follows:

- A *project proposal* of 1 page or less, describing:
  - Who is in your group
  - What problem you're trying to solve
  - A brief description of the approach you plan to use, including references to the underlying techniques you plan to leverage (e.g. privacy definitions, basic mechanisms, and existing algorithms)
  - A brief description of how your idea relates or compares to previous solutions to the same problem
- A *project writeup* of 3-5 pages, and containing:
  - A problem statement and comparison to related work (as in the proposal)
  - A technical description of your solution, with emphasis on anything that makes your solution unique; your description should be sufficient to enable the reader to *reproduce your implementation*
  - A description of the results - if you've evaluated your implementation on real data, describe how well it works
- A *project presentation* of about 15 minutes
  - Your presentation should include slides
  - All group members should present some part of the project
  - Your presentation should cover the same material as your writeup, and be understandable to anyone who has taken this class (i.e. related work that was not covered in class should be explained in your presentation)
- Your *implementation*, in whatever form you choose
  - You can use any language or libraries you prefer

### Schedule & Grading

The final project is worth 20% of your final grade. The schedule for final project deliverables, and the contribution of each one to the grade you receive for the final project, are as follows:

| Deliverable           | Due Date                      | Grade Percent | Turn In    |
| ---------------------:| ----------------------------- | ------------- | ---------- |
| Project Proposal      | 11/8/19 at 5:00pm             | 10%           | Gradescope |
| Project Presentations | 12/4/19 and 12/6/19 in class  | 30%           | In class   |
| Implementation        | 12/9/19 at 5:00pm             | 20%           | TBD        |
| Project Writeup       | 12/9/19 at 5:00pm             | 40%           | Gradescope |

- After the initial proposal phase, I'll respond with feedback and suggestions on Gradescope by Friday, 11/15/19.
- Each group member will receive the same project grade.
- The proposal grade will focus on how likely your proposed solution is to solve the problem. Most proposals are likely to receive full credit (i.e. don't worry about making it perfect).
- The implementation grade will focus on whether or not your code actually satisfies differential privacy; your implementation does not need to be particularly efficient or polished.
- The project writeup should be similar to a research paper in computer science, and is intended to give you experience with this kind of writing. In addition to a grade, I will provide you with feedback of the form you would receive from a conference reviewer, if you were to submit your writeup for publication at a computer science conference. Your grade will focus on the following points:
  - How well your writeup motivates the problem you have solved
  - The clarity of your technical description of your solution
  - Completeness of the comparison of your result to previous work
  - Your presentation of any evaluation results
- The presentation is intended to be similar to a conference presentation at a research conference; in addition to a grade, I will provide you with written feedback and suggestions from the perspective of preparing to make research presentations at conferences. Your presentation grade will focus on:
  - The clarity of your slides (i.e. use diagrams, and don't put a wall of text on your slides)
  - The extent to which your presentation covers the material in your writeup
  - The ability of audience members to follow your presentation and understand the key contribution of your project

As a paper reviewer, I try to answer the following questions. Your writeup should seek to address each one clearly.
- Is the paper answering the “right” question?
- Does it make reasonable assumptions?
- How novel is the solution?
- Is the solution technically sound?
- Is the solution difficult or easy?
- How well is the solution evaluated?
- Expected impact (hard to guess)
- Writing level: is the paper clearly written? Is it self-contained?

### Graduate Students

Graduate students (and undergraduates taking the course for graduate credit) will be expected to develop a more ambitious final project. In particular, your project writeup should be written in the style of a conference paper, and clearly describe the motivation for your work, your results, and what those results teach us that wasn't previously known. The goal is to give you practice in writing up a technical result in the style of a conference publication.

## Examples & Opportunities

You're welcome to work on any project interesting to you, as long as it's related to data privacy. If your idea is very different from the kinds of examples listed below, please email me in advance of the proposal deadline so we can discuss it.

### Project Ideas

- Use one of the systems we discussed in class to generate differentially private synthetic data, and run experiments to test its utility against the original data.

- Build a system to answer [WikiSQL](https://github.com/salesforce/WikiSQL) queries with differential privacy, and experiment with strategies for improving overall privacy budget behavior for a large workload of queries (e.g. better composition theorems).

- Implement an algorithm for estimating the scale of data, like the private quantile algorithm in [this paper](http://www.cse.psu.edu/~ads22/pubs/2011/stoc194-smith.pdf). Evaluate your algorithm on real data - either queries like WikiSQL or [TPC-H](http://www.tpc.org/tpch/), or machine learning data (as applied to the convex learning methods we saw in class).

- Reproduce statistics from real investigations of big data like [this one](https://dailydatablog.wordpress.com/2018/01/27/where-ya-headed-analyzing-over-400-million-taxi-trips-using-hadoop-and-pyspark/)([code](https://github.com/am2786/NYC-taxi-data-analysis)). Analyze the effect of data scale on the accuracy of your results.

- Solve a [Kaggle competition](https://www.kaggle.com/competitions) challenge with differential privacy, either with deep learning (if you have expertise) or using the convex machine learning solutions we saw in class.

- Participate in a research project on formally verifying differentially private algorithms, which builds on [Duet](https://plaid.w3.uvm.edu/duet/) (more in class).

### Specific Algorithms of Interest

Workloads of linear queries / synthetic data:
- [Matrix mechanism](https://people.cs.umass.edu/~mcgregor/papers/15-vldbj.pdf)
- [HDMM](https://arxiv.org/abs/1808.03537)
- [MWEM](https://arxiv.org/pdf/1012.4763.pdf)
- [Dual Query](https://arxiv.org/abs/1402.1526)

Graph queries:
- [Recursive mechanism](https://arxiv.org/abs/1304.4795)
- Lipschitz extensions: [paper 1](http://www.cse.psu.edu/~sxr48/pubs/nodeprivacy-TCC.pdf), [paper 2](https://cs-people.bu.edu/sofya/pubs/Lipschitz-deg-ext-FOCS16.pdf)
- [Weighted PINQ](https://arxiv.org/abs/1203.3453)

Algorithms for streaming data:
- [PeGaSus](https://people.cs.umass.edu/~miklau/assets/pubs/dp/Chen17PeGaSus.pdf)


### CS Fair

I *highly encourage* everyone to submit their projects to the [CS Fair](https://csfair.w3.uvm.edu/). The materials you prepare for the course should be all you need for a compelling entry, and there are cash prizes for the first three places. If you register by November 9, you get a free t-shirt!

### Projects Overlapping with CS295A: Software Verification

If you're also in David Darais's CS295A: Software Verification, I *highly encourage* projects that satisfy the requirements for both classes. It's very likely that you can submit the same writeup and presentation for both courses (though the bar may be a little higher). If you're interested in this, please let me know and we'll discuss it. Some interesting ideas include:

- Verify an algorithm for computing sensitivity of queries in relational algebra
- Verify that a clipping + averaging algorithm has bounded sensitivity
- Verify that sample & aggregate yields bounded local sensitivity
