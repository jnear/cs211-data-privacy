---
title: CS 295B Data Privacy
layout: default
---

# UVM CS 295B: Data Privacy (Fall 2018)

## Announcements

### 9/10/18
Homework 1 [has been posted](https://github.com/jnear/cs295-data-privacy/blob/master/homework/Homework%201.ipynb). It is due on 9/17/18 at 11:59pm.

### 8/29/18
Note that there will be **no class** or office hours next week, 9/3 and 9/5.

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

- **Lecture**: Monday and Wednesday, 5:05pm - 6:20pm, Votey 209
- **Instructor**: Joe Near (jnear at uvm dot edu)
- **Office hours**: Thursdays, 2:00pm - 4:00pm, Votey 317

## Resources

- **Homework assignments** will be turned in via [Blackboard](https://bb.uvm.edu/webapps/blackboard/execute/announcement?method=search&context=course&course_id=_123457_1&handle=cp_announcements&mode=cpview)
- **Discussions** will take place on the [course Piazza](http://piazza.com/uvm/fall2018/cs295b)
- **Slides** from lecture are available [here](https://github.com/jnear/cs295-data-privacy/tree/master/slides)

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

 - [Notes on probability distributions](https://www3.nd.edu/~rwilliam/stats1/x11.pdf)

## Policies

### Grading

Your grade for the course will be determined as follows:

- 8 homework assignments (5% each; 40% total)
- 2 in-class quizzes (10% each; 20% total)
- midterm exam (20%)
- final project (20%)

### Exams & Quizzes

There will be two quizzes during class on October 3 and November 26, and a midterm exam during class on October 15.
You will be allowed one physical page (8 1/2" x 11") of notes for each exam.
There is no final exam, and this course will conclude before the University's exam period.

### Homework Assignments

This course will use Python for examples and for programming assignments.
Students are expected to be proficient in Python programming.
Programming assignments will be distributed and turned in as Jupyter notebooks.
See [this page](http://jupyter.org/install) for information on installing Jupyter; the Anaconda method is recommended,
since it also installs the other libraries we will use in the course.

Homework will be turned in via Blackboard.

 - [Homework 1](https://github.com/jnear/cs295-data-privacy/blob/master/homework/Homework%201.ipynb)

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

More information coming soon.

## Schedule

| Date     | Topics        | Reference | Notes / Homework |
| --------:| ------------- | --------- | ---------------- |
| 8/27/18  | Intro to data analytics & data privacy | Nissim, sec. 1&2 |
| 8/29/18  | Survey of privacy techniques | D&R, ch. 1 |
| 9/3/18   | No class (Labor day)
| 9/5/18   | No class
| 9/10/18  | K-Anonymity & re-identification | TBA | [HW1](https://github.com/jnear/cs295-data-privacy/blob/master/homework/Homework%201.ipynb) released
| 9/12/18  | Differential privacy: sensitivity & Laplace mech. | Nissim, sec. 3&4; D&R, ch. 2; D&R, sec. 3.3 
| 9/17/18  | Composition & privacy budget | D&R, sec. 3.5, 3.5.1 | HW1 due, HW2 released
| 9/19/18  | Post-processing & basic algorithm design | D&R, sec. 3.5, 3.5.1 |
| 9/24/18  | Approximate differential privacy & the Gaussian mechanism | D&R, sec. 3.5.2, appendix A | HW2 due, HW3 released
| 9/26/18  | Advanced composition | D&R, sec. 3.5.2
| 10/1/18  | Exponential mechanism | HW3 due, HW4 released
| 10/3/18  | Local sensitivity; Quiz #1 | D&R, sec. 3.4 | Quiz
| 10/8/18  | No class (Fall break)
| 10/10/18 | Smooth sensitivity, medians, and joins | [NSRS07](http://www.cse.psu.edu/~ads22/pubs/NRS07/NRS07-full-draft-v1.pdf), sec. 1-3 | HW4 due, HW5 released
| 10/15/18 | Midterm | . | Midterm
| 10/17/18 | Subsample & aggregate | D&R, sec. 7.1; [NSRS07](http://www.cse.psu.edu/~ads22/pubs/NRS07/NRS07-full-draft-v1.pdf), sec. 4
| 10/22/18 | Language techniques for privacy |TBA | HW5 due, HW6 released
| 10/24/18 | Language techniques for privacy |TBA | 
| 10/29/18 | Variants of differential privacy | Renyi, zCDP, sampling | HW6 due
| 10/31/18 | Intro to private machine learning | Chaudhuri et al.     
| 11/5/18  | Differentially private SGD | Bassily et al. | HW7 released
| 11/7/18  | Objective & output perturbation | Chaudhuri et al.       
| 11/12/18 | Private deep learning | Talwar et al. | HW7 due, HW8 released
| 11/14/18 | Private transfer learning | PATE 1 & 2 | Project proposals due (tent.)
| 11/19/18 | No class (Thanksgiving break)
| 11/21/18 | No class (Thanksgiving break)
| 11/26/18 | Building privacy-preserving systems; Quiz #2 | PINQ, GUPT, Airavat, RAPPOR, Apple, Uber | Quiz, HW8 due
| 11/28/18 | Privacy attacks & open challenges | [Tockar](https://research.neustar.biz/author/atockar/)
| 12/3/18  | Project presentations
| 12/5/18  | Project presentations

