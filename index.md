---
title: CS 295 Data Privacy
layout: default
---

# UVM CS 295: Data Privacy (Fall 2019)

## Announcements

**11/3/19**: [Homework 6](https://github.com/jnear/cs295-data-privacy/blob/master/homework/Homework%206.ipynb) has been posted. It is due on Friday, November 8, at 5:00pm.

**10/28/19**: [Notes on final projects](https://jnear.github.io/cs295-data-privacy/projects) have been posted.

**10/21/19**: [Notes from today's lecture](https://github.com/jnear/cs295-data-privacy/blob/master/notes/11%20-%20Algorithm%20Design.ipynb) have been posted.

**10/18/19**: [Homework 5](https://github.com/jnear/cs295-data-privacy/blob/master/homework/Homework%205.ipynb) has been posted. It is due on Friday, October 25, at 5:00pm.

**10/14/19**: [Homework 4](https://github.com/jnear/cs295-data-privacy/blob/master/homework/Homework%204.ipynb) has been posted. It is due on Friday, October 18, at 5:00pm.

**9/27/19**: [Homework 3](https://github.com/jnear/cs295-data-privacy/blob/master/homework/Homework%203.ipynb) has been posted. It is due on Friday, October 4, at 5:00pm.

**9/17/19**: [Homework 2](https://github.com/jnear/cs295-data-privacy/blob/master/homework/Homework%202.ipynb) has been posted. It is due on Friday, September 27, at 5:00pm.

**9/13/19**: Due to a travel delay, there will be no class today (9/13). I have delayed the submission deadline for Homework 1 to next Tuesday.

**9/9/19**: I have posted the first three sets of [course notes](https://github.com/jnear/cs295-data-privacy/tree/master/notes), which may be helpful in completing the first homework assignment.

**9/6/19**: [Homework 1](https://github.com/jnear/cs295-data-privacy/blob/master/homework/Homework%201.ipynb) has been posted. It is due on Friday, September 13, at 5:00pm.

## Course Description

How can we learn from sensitive data collected from individuals, while protecting the privacy of those individuals? 

This question is central to the study of data privacy,
and is increasingly relevant with the widespread collection of our personal data.
Analysis of this data can lead to important benefits for society,
including advances in medicine and public infrastructure,
but can also result in privacy breaches that expose our most closely-held secrets.

This course will explore both threats to privacy and solutions to the data privacy problem.
We will demonstrate that traditional approaches to protecting privacy, such as anonymization,
are subject to powerful attacks that reveal individuals' sensitive data.
We will see that while more recent approaches for protecting privacy, including k-anonymity and l-diversity,
are more resistant to these attacks, they are not immune.

Then, we will explore recent formal notions of privacy, including differential privacy.
Differential privacy provides a rigorous formal definition of individual privacy that enables a wide range of
statistical analyses while protecting privacy.
We will explore a number of differentially private algorithms for analytics and machine learning,
and learn about the algorithmic building blocks and proof techniques used to develop them.

In addition to learning about the mathematical foundations of differential privacy,
we will explore its practical implications.
We will learn about existing practical systems for enforcing differential privacy and examine the challenges of building such systems.
This course will include programming assignments and an end-of-semester project,
in which students are expected to demonstrate both mastery of the concepts we explore and understanding of
their practical implications by building their own systems that perform privacy-preserving analyses on real data.

## Administrative

- **Lecture**: Monday, Wednesday, Friday, 1:10pm - 2:00pm, Votey 254
- **Instructor**: Joe Near (jnear at uvm dot edu)
- **Office hours**: Thursdays, 2:00pm - 4:00pm, Innovation E458

## Resources

- **Course notes** are available as Python notebooks [here](https://github.com/jnear/cs295-data-privacy/tree/master/notes)
- **Homework assignments** will be turned in via [Gradescope](https://www.gradescope.com/)
- **Discussions** will take place on the course [Piazza](https://piazza.com/class/jzjwvewkdri4yk)
- **Slides** from lecture are available [here](https://github.com/jnear/cs295-data-privacy/tree/master/slides)
- **Blackboard** for the course is available [here](https://bb.uvm.edu/webapps/blackboard/execute/courseMain?course_id=_135289_1)
- **Review Sheets** for exams:
  - [Exam 1](https://github.com/jnear/cs295-data-privacy/blob/master/slides/exam1-review.md)

## Textbook & Other References

Please **do not** buy any books for this course. All required reference material is available online for free.

The primary textbook we will use for this course is:

- [D&R] [The Algorithmic Foundations of Differential Privacy](https://www.cis.upenn.edu/~aaroth/Papers/privacybook.pdf)  
  Cynthia Dwork and Aaron Roth.

The textbook is available in PDF form for free; buying a paper copy is difficult and not needed for this course.
We will also use the following non-technical primer on differential privacy, also available for free:

- [Nissim] [Differential Privacy: A Primer for a Non-technical Audience](https://privacytools.seas.harvard.edu/files/privacytools/files/pedagogical-document-dp_new.pdf)  
   Kobbi Nissim, Thomas Steinke, Alexandra Wood, Micah Altman, Aaron Bembenek, Mark Bun, Marco Gaboardi, David R. O’Brien, and Salil Vadhan.

In addition to these, we will reference a number of academic papers throughout the semester (especially for the section on privacy-preserving machine learning).

### Links and Helpful Resources

 - [Definitions and formulas](https://github.com/jnear/cs295-data-privacy/blob/master/slides/formulas.pdf) that may be helpful on quizzes and exams
 - [Notes on probability distributions](https://www3.nd.edu/~rwilliam/stats1/x11.pdf)
 - [Intro to differentially private machine learning](https://github.com/jnear/cs295-data-privacy/blob/master/slides/Intro%20to%20machine%20learning.ipynb)
 - [Variants of differential privacy](https://github.com/jnear/cs295-data-privacy/blob/master/slides/privacy_definitions.pdf)
 - Vincent Bindschaedler's [Synthetic Data Generation Framework](https://vbinds.ch/node/69)

## Policies

### Grading

Your grade for the course will be determined as follows:

- 8 homework assignments (5% each; 40% total)
- 2 in-class exams (20% each; 40% total)
- final project (20%)

### Exams & Quizzes

There will be two exams during class on October 11 and November 22.
You will be allowed one physical page (8 1/2" x 11") of notes for each exam.
There is no final exam, and this course will conclude before the University's exam period.

### Homework Assignments

This course will use Python for examples and for programming assignments.
Students are expected to be proficient in Python programming.
Programming assignments will be distributed and turned in as Jupyter notebooks.
See [this page](http://jupyter.org/install) for information on installing Jupyter; the Anaconda method is recommended,
since it also installs the other libraries we will use in the course.

**Assignment Submission*: Homework will be turned in and graded via Gradescope. You should receive an email with a link to activate your account after the semester begins. If you don't receive such a link, or if you have trouble logging in to Gradescope, let me know.

To submit an assignment:

1. Complete the released Jupyter Notebook by filling in answers to all the questions
2. Export your Notebook to a Python (.py) file. In the Notebook interface, click on "File" -> "Download as..." -> "Python (.py)"
3. Log into Gradesceope and submit the exported .py file as your assignment solution

Please let me know if you have any questions about the submission process, or trouble with Gradescope.

 - [Homework 1](https://github.com/jnear/cs295-data-privacy/blob/master/homework/Homework%201.ipynb) (due Tuesday, September 17, 5:00pm)
 - [Homework 2](https://github.com/jnear/cs295-data-privacy/blob/master/homework/Homework%202.ipynb) (due Friday, September 27, 5:00pm)
 - [Homework 3](https://github.com/jnear/cs295-data-privacy/blob/master/homework/Homework%203.ipynb) (due Friday, October 4, 5:00pm)
 - [Homework 4](https://github.com/jnear/cs295-data-privacy/blob/master/homework/Homework%204.ipynb) (due Friday, October 18, 5:00pm)
 - [Homework 5](https://github.com/jnear/cs295-data-privacy/blob/master/homework/Homework%205.ipynb) (due Friday, October 25, 5:00pm)
 - [Homework 6](https://github.com/jnear/cs295-data-privacy/blob/master/homework/Homework%206.ipynb) (due Friday, November 8, 5:00pm)

### Late Work

Homework assignments may be turned in late for a penalty of 10% per day after the deadline.
Homework more than 10 days late will not be accepted.

### Collaboration & Allowed References

Collaboration on the high-level ideas and approach on assignments is encouraged.
Copying someone else's work is not allowed.
Any collaboration, even at a high level, must be declared when you submit your assignment.
Every assignment must include a collaboration statement.
E.g., "I discussed high-level strategies for solving problem 2 and 5 with Alex."

The official references for the course are listed in the schedule below.
Copying from references other than these is not allowed.
In particular, code and proofs should not be copied from other sources,
including Stack Overflow and other public sources.

Students caught copying work are eligible for immediate failure of the course and disciplinary action by the University.
All academic integrity misconduct will be treated according to [UVM's Code of Academic Integrity](https://www.uvm.edu/policies/student/acadintegrity.pdf).

## Final Projects

The course will include a final project, completed in groups of 1-3 students.
The final project will demonstrate your mastery of the concepts covered in this course
by implementing a practical system to perform privacy-preserving analysis of realistic data.

Click [here](https://jnear.github.io/cs295-data-privacy/projects) for more complete information.

## Schedule

Note that class will **not** be held on the following dates:

- Monday, Sep. 2 (labor day)
- Monday, Sep. 9
- Wednesday, Sep. 11
- Monday, Oct. 14 (fall recess)
- Wednesday, Oct. 23
- Friday, Oct. 25
- Week of Nov. 25 (Thanksgiving break)

Important dates:

- Exam #1: Friday, October 11
- Exam #2: Friday, November 22
- Project presentations: December 4 & 6
- Final projects due: December 9

Important links:

- [Course notes](https://github.com/jnear/cs295-data-privacy/tree/master/notes)
- [PDFs of course notes](https://github.com/jnear/cs295-data-privacy/tree/master/notes/pdfs)

| Week of...| Topics                                                                               | Reference | Homework (tentative)   |
| ---------:| ------------------------------------------------------------------------------------ | --------- | ---------------------- |
| 8/26/19   | Intro to data privacy; de-identification; re-identification                          | [Notes #1](https://github.com/jnear/cs295-data-privacy/blob/master/notes/1%20-%20De-identification%20and%20Re-identification.ipynb)  |                        |
| 9/2/19    | k-Anonymity and l-Diversity (no class Monday)                                        | [Notes #2](https://github.com/jnear/cs295-data-privacy/blob/master/notes/2%20-%20k-Anonymity.ipynb)  | HW1 Released           |
| 9/9/19    | Intro to differential privacy (no class Monday & Wednesday)                          | [Notes #3](https://github.com/jnear/cs295-data-privacy/blob/master/notes/3%20-%20Introduction%20to%20Differential%20Privacy.ipynb)  | HW1 Due                |
| 9/16/19   | Sensitivity; Laplace mechanism; post-processing; composition & privacy budget        | [Notes #4](https://github.com/jnear/cs295-data-privacy/blob/master/notes/4%20-%20Properties%20of%20Differential%20Privacy.ipynb), [Notes #5](https://github.com/jnear/cs295-data-privacy/blob/master/notes/5%20-%20Sensitivity.ipynb)          | HW2 Released           |
| 9/23/19   | Relaxations of DP; Gaussian mech.; advanced composition                              | [Notes #6](https://github.com/jnear/cs295-data-privacy/blob/master/notes/6%20-%20Approximate%20Differential%20Privacy.ipynb)          | HW2 Due; HW3 Released  |
| 9/30/19   | Local sensitivity; propose-test-release, smooth sensitivity, sample-and-aggregate    | [Notes #7](https://github.com/jnear/cs295-data-privacy/blob/master/notes/7%20-%20Local%20Sensitivity.ipynb)          | HW3 Due                |
| 10/7/19   |  Recent variants of differential privacy; exam #1                              | [Notes #8](https://github.com/jnear/cs295-data-privacy/blob/master/notes/8%20-%20Variants%20of%20Differential%20Privacy.ipynb)          | HW4 Released           |
| 10/14/19  | Exponential mechanism; sparse vector technique (no class Monday)          | [Notes #9](https://github.com/jnear/cs295-data-privacy/blob/master/notes/9%20-%20Exponential%20Mechanism.ipynb), [Notes #10](https://github.com/jnear/cs295-data-privacy/blob/master/notes/10%20-%20Sparse%20Vector%20Technique.ipynb)          | HW4 Due; HW5 Released  |
| 10/21/19  | Algorithm design (no class Wednesday, Friday)                                        | [Notes #11](https://github.com/jnear/cs295-data-privacy/blob/master/notes/11%20-%20Algorithm%20Design.ipynb)          | HW5 Due                |
| 10/28/19  | Privacy-preserving machine learning; differentially private SGD                      |           | HW6 Released           |
| 11/4/19   | Differentially private synthetic data                                                |           | HW6 Due; HW7 Released  |
| 11/11/19  | Local differential privacy                                                           |           | HW7 Due; HW8 Released  |
| 11/18/19  | Privacy in deep learning; practical systems for privacy; exam #2                     |           | HW8 Due                |
| 11/25/19  | No class Monday, Wednesday, Friday                                                   |           |                        |
| 12/2/19   | Open challenges; project presentations                                               |           | Final projects due     |

