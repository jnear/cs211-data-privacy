---
title: CS 211 Data Privacy
layout: default
---

# UVM CS 211: Data Privacy (Fall 2022)

  * [Course Description](#course-description)
  * [Administrative](#administrative)
  * [Resources](#resources)
  * [Textbook & Other References](#textbook---other-references)
  * [Policies](#policies)
    + [Grading](#grading)
    + [Exams & Quizzes](#exams---quizzes)
    + [Homework Assignments and In-class Exercises](#homework-assignments-and-in-class-exercises)
    + [Late Work](#late-work)
    + [Collaboration & Allowed References](#collaboration--allowed-references)
  * [Final Projects](#final-projects)
  * [CS Student Research Day & Extra Credit](#cs-student-research-day--extra-credit)
  * [Schedule](#schedule)

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

## Learning Objectives

By the end of this course, you will be able to:

- Describe the problem and challenges of data privacy
- Conduct a privacy attack on de-identified data
- Define and apply formal notions of privacy, including k-Anonymity and differential privacy
- Design differentially private algorithms and argue that they are correct
- Evaluate the accuracy and efficiency properties of differentially private algorithms

## Administrative

- **Lecture**: Monday, Wednesday, Friday, 1:10pm - 2:00pm, at Dewey Hall 314
- **Instructor**: Joe Near (jnear at uvm dot edu)
- **Graduate Teaching Assistant**: Protiva Sen
- **Office hours**: 
  - **Joe Near** (instructor): Mondays and Fridays, 9:30am-10:30am, and by appointment; Innovation Hall E458 (or MS Teams)

## Resources

- **Course textbook** is available [online](https://programming-dp.com) or as a [PDF](https://github.com/uvm-plaid/programming-dp/blob/master/book.pdf)
- **Blackboard** for the course is available [here](https://bb.uvm.edu/webapps/blackboard/execute/launcher?type=Course&id=_171840_1)
- **Course Github Repo** [is available here](https://github.com/jnear/cs211-data-privacy)
- **Weekly exercises**
  - [Download exercises here](https://github.com/jnear/cs211-data-privacy/tree/master/exercises)
  - Turn in notebook files on Blackboard
- **Homework assignments** 
  - [Download notebooks here](https://github.com/jnear/cs211-data-privacy/tree/master/homework)
  - Turn in notebook files on Blackboard
- **Discussions** will take place on MS Teams
- **Slides** from lecture are available [here](https://github.com/jnear/cs211-data-privacy/tree/master/slides)
- **Review Sheets** for exams:
  - [Exam 1](https://github.com/jnear/cs211-data-privacy/blob/master/slides/exam1-review.md)
  - [Exam 2](https://github.com/jnear/cs211-data-privacy/blob/master/slides/exam2-review.md) (not yet updated for 2022)

## Textbook & Other References

Please **do not** buy any books for this course. All required reference material is available online for free.

The primary textbook we will use for this course is:

- [Programming Differential Privacy](https://programming-dp.com)  
  Joseph P. Near and Chiké Abuah.  
  Also available as a [PDF](https://github.com/uvm-plaid/programming-dp/blob/master/book.pdf)

The following resources may also be useful for additional reading:

- [D&R] [The Algorithmic Foundations of Differential Privacy](https://www.cis.upenn.edu/~aaroth/Papers/privacybook.pdf)  
  Cynthia Dwork and Aaron Roth.
  
- [Nissim] [Differential Privacy: A Primer for a Non-technical Audience](https://privacytools.seas.harvard.edu/files/privacytools/files/pedagogical-document-dp_new.pdf)  
   Kobbi Nissim, Thomas Steinke, Alexandra Wood, Micah Altman, Aaron Bembenek, Mark Bun, Marco Gaboardi, David R. O’Brien, and Salil Vadhan.

In addition to these, we will reference a number of academic papers throughout the semester (especially for the section on privacy-preserving machine learning).

### Links and Helpful Resources

 - [How to set up Jupyter Notebooks](https://jnear.github.io/cs211-data-privacy/jupyter)
 - [Definitions and formulas](https://github.com/jnear/cs211-data-privacy/blob/master/slides/formulas.pdf) that may be helpful on quizzes and exams
 - [Notes on probability distributions](https://www3.nd.edu/~rwilliam/stats1/x11.pdf)
 - [Intro to differentially private machine learning](https://github.com/jnear/cs211-data-privacy/blob/master/slides/Intro%20to%20machine%20learning.ipynb)
 - [Variants of differential privacy](https://github.com/jnear/cs211-data-privacy/blob/master/slides/privacy_definitions.pdf)

## Policies

### Grading

Your grade for the course will be determined as follows:

- 10 homework assignments (5% each; 50% total)
- in-class weekly exercises (20% total)
- midterm exam (10%)
- final exam (10%)
- final project (10%)

Your final grade will be determined by summing the total number of
points awarded and calculating the percentage of the total possible
points. This percentage is translated into a letter grade as follows:

#### Undergraduate Students

| Percent | Letter Grade |
| ------: | ------------ |
| 98-100  | A+           |
| 93-97   | A            |
| 90-92   | A-           |
| 87-89   | B+           |
| 83-86   | B            |
| 80-82   | B-           |
| 77-79   | C+           |
| 73-76   | C            |
| 70-72   | C-           |
| 67-69   | D+           |
| 63-66   | D            |
| 60-62   | D-           |
| <60     | F            |

#### Graduate Students

| Percent | Letter Grade |
| ------: | ------------ |
| 98-100  | A+           |
| 93-97   | A            |
| 90-92   | A-           |
| 87-89   | B+           |
| 83-86   | B            |
| 80-82   | B-           |
| 77-79   | C+           |
| 73-76   | C            |
| 70-72   | C-           |
| <70     | F            |

### Exams & Quizzes

There will be two exams: a midterm and a final. You will be allowed one page of notes for each exam. See the schedule below for the dates.

### Homework Assignments and In-class Exercises

This course will use Python for examples and for programming
assignments.  Students are expected to be proficient in Python
programming.  Programming assignments will be distributed and turned
in as Jupyter notebooks. [Click
here](https://jnear.github.io/cs211-data-privacy/jupyter) for
instructions on installing Jupyter Notebook.

**Assignment Submission**: Homework and in-class exercises will be
turned in via Blackboard.

To submit an assignment:

1. Complete the released Jupyter Notebook by filling in answers to all the questions
2. Submit the notebook file (the .ipynb file) as your solution on Blackboard

*Please* do not change the name of the .ipynb file. This makes the
grading process more difficult.

Please let me know if you have any questions about the submission process.

### Late Work

Late work *may* be accepted, but you *must* make arrangements with me
first. If you need to turn something in late, for any reason, please
email me *before the deadline*. Depending on the circumstances, I may
(or may not) impose a late penalty on your grade.

### Collaboration & Allowed References

Collaboration on the high-level ideas and approach on assignments is encouraged.
Copying someone else's work is not allowed.
Any collaboration, even at a high level, must be declared when you submit your assignment, in a note at the top of the assignment.
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

Click [here](https://jnear.github.io/cs211-data-privacy/projects) for more complete information.

## CS Student Research Day & Extra Credit

We will **not hold class** on **Friday, September 23**. I encourage you
to attend [CS Student Research
Day](https://www.uvm.edu/~jonaolap/csrd/2022.html) and learn about
the awesome research being done by CS students at UVM!

- If you attend **two full sessions** of talks (~4 talks), **take
  brief notes on the talks you hear**, and **send the notes to me via
  email by 11:59pm on September 23**, I will give **1% extra credit to
  your final grade in the course**

## Schedule

Note that class will **not** be held on the following dates:

- Monday, September 5 (Labor Day)
- Friday, September 23 (please attend [CS Student Research Day](https://www.uvm.edu/~jonaolap/csrd/2022.html))
- Friday, October 14 (Fall Recess)
- November 21-25 (Thanksgiving)

Important due dates:

- Homework assignments are due every *Monday* at 11:59pm.
- In-class weekly exercises are due every *Friday*, by 11:59pm.

Exam dates:

- Midterm exam: Wednesday, October 12, during class (Dewey 314)
- Final exam: December 15, 10:30am - 11:30am (Dewey 314)

Homework dates:

| Item                                                                                            | Due Date |
| -----------------------------------------------------------------------------------------:      | -------- |
| [Homework 1](https://github.com/jnear/cs211-data-privacy/blob/master/homework/CS211_HW_1.ipynb) | 9/12/22  |
| [Homework 2](https://github.com/jnear/cs211-data-privacy/blob/master/homework/CS211_HW_2.ipynb) | 9/19/22  |
| [Homework 3](https://github.com/jnear/cs211-data-privacy/blob/master/homework/CS211_HW_3.ipynb) | 9/26/22  |
| [Homework 4](https://github.com/jnear/cs211-data-privacy/blob/master/homework/CS211_HW_4.ipynb) | 10/3/22  |
| [Homework 5](https://github.com/jnear/cs211-data-privacy/blob/master/homework/CS211_HW_5.ipynb) | 10/17/22 |
| Homework 6                                                                                      | 10/24/22 |
| Homework 7                                                                                      | 10/31/22 |
| Homework 8                                                                                      | 11/7/22  |
| Homework 9                                                                                      | 11/14/22 |
| Homework 10                                                                                     | 12/5/22  |
| Project proposals                                                                               | 11/18/22 |
| Final project writeup/video/implementation                                                      | 12/12/22 |

Schedule of topics:

| Week of... | Topics                                                                                          | Reference |
| ---------: | ------------------------------------------------------------------------------------            | --------- |
| 8/29/22    | Intro to data privacy; de-identification; re-identification (no exercise)                       | Ch. 1     |
| 9/5/22     | k-Anonymity and l-Diversity (no class Monday)                                                   | Ch. 2     |
| 9/12/22    | Intro to differential privacy                                                                   | Ch. 3     |
| 9/19/22    | Sensitivity; Laplace mechanism; post-processing; composition & privacy budget (no class Friday) | Ch. 4, 5  |
| 9/26/22    | Sensitivity & clipping; approximate DP; Advanced composition; Gaussian mechanism                | Ch. 6     |
| 10/3/22    | Local sensitivity; propose-test-release, smooth sensitivity, sample-and-aggregate               | Ch. 7     |
| 10/10/22   | *Intermission.* Review (exam Wednesday; no class Friday; no exercise)                           | None      |
| 10/17/22   | Recent variants of differential privacy                                                         | Ch. 8     |
| 10/24/22   | Exponential mechanism; sparse vector technique                                                  | Ch. 9, 10 |
| 10/31/22   | Privacy-preserving machine learning; differentially private SGD                                 | Ch. 12    |
| 11/7/22    | Local differential privacy                                                                      | Ch. 13    |
| 11/14/22   | Differentially private synthetic data                                                           | Ch. 14    |
| 11/21/22   | No class (Thanksgiving)                                                                         |           |
| 11/28/22   | Privacy in deep learning; Practical systems for privacy                                         |           |
| 12/5/22    | Open challenges; review                                                                         |           |

# Accommodations

In keeping with University policy, any student with a documented
disability interested in utilizing accommodations should contact SAS,
the office of Disability Services on campus. SAS works with students
and faculty in an interactive process to explore reasonable and
appropriate accommodations, which are communicated to faculty in an
accommodation letter. All students are strongly encouraged to meet
with their faculty to discuss the accommodations they plan to use in
each course. A student's accommodation letter lists those
accommodations that will not be implemented until the student meets
with their faculty to create a plan. Contact SAS: A170 Living/Learning
Center; 802-656-7753; access@uvm.edu; or www.uvm.edu/access

# Religious Holidays

Students have the right to practice the religion of their choice. Each
semester students should submit in writing to their instructors by the
end of the second full week of classes their documented religious
holiday schedule for the semester. An arrangement can then be made to
make up the missed work.

# Student Athletes

In order to be excused from classes, student athletes should submit
appropriate documentation to the Professor in advance of all
scheduling conflicts within the first two weeks of class. Those
missing class are expected to submit make-up assignments within a
reasonable time period.
