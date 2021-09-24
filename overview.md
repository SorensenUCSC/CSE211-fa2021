---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

title: "Overview"
layout: single
classes: wide
---

## Class Description

Welcome to CSE 211: Compiler Design! In this class we will explore one of the most import tools in computer science: the compiler. In particular, we will explore how compiler techniques transform high level languages into low-level languages, i.e. closer to the instructions that processors can actually execute. We will study how compilers can automatically make code more efficient and safe on modern processors. When you leave this class you should be comfortable with: specifying programming language grammars, performing flow analysis on intermediate languages, and understanding advanced optimization techniques, such as automatically transforming sequential code into parallel code. 

## Required Background

This class has a prerequisite of an introductory compiler course. However, because this is a graduate course, we will have students from many different undergrad programs. It is difficult to rely on very specific backgrounds. Because of this, I have been lenient with prerequisites and I hope we can cover a variety of topics that are interesting and accessible to everyone.

Because this is a graduate level class, I do expect a general strong CS foundation. In particular, you should be:

- comfortable using a linux command-line (this is how your assignments will be submitted).
- programming in a high-level language (e.g. Python)
- programming in a low-level language (e.g. C)
- a high-level understanding of basic parsing (i.e. regular expressions and context-free grammars)
- a high-level understanding computer architecture, i.e. basic processor design and how ISA instructions are executed

## Class Modules

This class will be split into 5 modules, each of which are roughly two weeks. The first three modules will follow a typical course style structure while the last two will be structured more like a reading group, where we discuss recent or classic papers in the area.

* **Module 1: Parsing Overview:** We will discuss the components of a parser: including tokenizing, grammar specification, and parser generators. 

* **Module 2: Flow Analysis:** We will discuss different flow analysis (aka static analysis). This includes AST traversals, SSA form, and applications such as finding potential uses of uninitialized variables.

* **Module 3: Automatic Parallelization:** We will discuss how compilers can be used to transform sequential code blocks into equivalent forms that can be executed in parallel.

* **Module 4: Domain Specific Languages:** We will discuss domain specific languages and how compilers can leverage the domain constraints to perform even more optimizations. Topics may include languages for machine learning and graph applications.

* **Module 5: Optimization Policies:** We will discuss the impact of compiler optimizations and how to determine if optimizations actually provide reliable and portable performance improvements. 

## Class Format

Each class is 65 minutes. I will try to arrive 15 minutes early and stay 15 minutes late for questions or discussion (pending classroom availability). 

_Non-protected materials_ will be hosted on this website. This includes homework assignments, schedules, references, etc.

_Protected materials_ will be hosted on the Canvas website that you will need your university credentials to access. These materials include any zoom links, lecture recordings, tests, grades, etc.

There will be an official forum in the Canvas that you can use to discuss course topics and ask questions. If we want a different forum (slack or discord), I will consider hosting one. We have a small class so I hope we can have lively discussions!

## Attendance

This is a small graduate course and live discussions will be a valuable part of the learning experience. As such, I expect you to make an effort to attend. **Attendance will be 10% of your grade**. I will take role at the beginning of each class.

Please message me if you will miss a lecture to avoid losing attendance credit. You can have up to 3 excused absences. If the normally scheduled date and time will be an issue for you, please let me know ASAP.

## Accessibility

UC Santa Cruz is committed to creating an academic environment that supports its diverse student body. If you are a student with a disability who requires accommodations to achieve equal access in this course, please submit your Accommodation Authorization Letter from the Disability Resource Center (DRC) to me by email, preferably within the first two weeks of the quarter. I would also like us to discuss ways we can ensure your full participation in the course. I encourage all students who may benefit from learning more about DRC services to contact DRC by phone at 831-459-2089 or by email at drc@ucsc.edu.

## Office Hours:

Office hours will be 3 - 4 pm on Wednesdays. I do not mind having in-person or remote meetings. I will host a Google doc sign up sheet that you can use to sign up. If you don't sign up, I will leave my office door open during these hours when I am available. Because this is a small class, I imagine if you swing by there is a good chance I will be available.

I will hold additional office hours by appointment. Please don't hesitate to email me!

## Homework:

There will be one assignment per module, for a total of 5 homeworks. 

I will provide a docker image with an up-to-date version of Ubuntu and a suite of useful software installed. The homework assignments will include a specification of how the assignment must execute. It must execute inside the Docker container to be graded. If you need/want additional software in the Docker image, please just ask! 

With the exception of the final homework assignment, all homeworks will be posted 2 weeks before they are due. The last homework will be posted a week before it is due and will have a reduced workload.

## Tests:

There will be two tests in this course: a midterm and a final. The midterm is worth (~10%). The final will be worth more at 30%

Due to remote classes last year, I gave take-home, open-note, tests so that we did not have to deal with the difficulties of remote exams. I liked this approach and I would like to try it for in-person classes.

You will have 1 week to complete the midterm. Please plan accordingly because you will also have an assignment out at this time. You will have 8 hours to complete the final exam.

You are free to consult notes, books, or the internet. While the test is active, you are not allowed to discuss the test with another person (either in the class or online). For example, you  _can_  google concepts that are on the test. You  _cannot_  post a test question to stackoverflow.

_a note on timing_: my tests are designed to take 120 minutes  _if_  they were given in-person. In practice, students take much longer on take-home tests because you can spend time validating answers and less time studying before hand. Because of this, many students spend much longer on take-home tests. Please consider this when budgeting time.

## Paper Assignment

Scientific literacy is a key skill that every grad student should learn. Towards that goal, this class will require a paper assignment. This consists of finding a conference or journal paper that has a strong compiler component and writing a short review for the paper. 

The review should roughly be 4 pages double spaced. Please organize it as follows:

- **Motivation:** what is the problem and why is it important?
- **Compiler component:** what is the compiler component and how does it relate to what we have learned?
- **Illustrative example:** find a small example that you can clearly explain, especially related to the compiler component. This might be a small program and a description of how the compiler transforms the program.
- **Key results:** what are the important results of this paper and how did the compiler enable them?

Please pre-approve the paper with me. Additionally, I can suggest papers. The reports will be two weeks before the quarter ends. Dates for the paper assignment are summarized [here](homeworks.html#paper-assignments-and-final-projects).

## Final Project

You can substitute the final exam for a final project. The project will need to be pre-approved by me no later than 2 weeks before the end of the semester. To propose a project, please write a 1 page summary clearly describing the compiler element to the project and how it relates to what we are learning.

Your final project deliverable will be a 6 page double spaced report detailing your project with an emphasis on the compiler aspects of your project. Think of it like a mini conference paper, with a
required "compiler design and implementation" section. I expect this section will be roughly 2 pages of your report. You will also be required to give a 15 minute presentation about your final project to
the class. Dates for the final project are summarized [here](homeworks.html#paper-assignments-and-final-projects).

If you are a PhD student, I strongly recommend thinking about a final project related to your thesis.

## Grade Breakdown

- Attendance: 10%
- Homeworks: 40% (8 points each)
- Paper Assignment: 10%
- Midterm: 10%
- Final Exam/Project: 30%

I will be grading all assignments and tests. If you want to discuss a grade, please contact me no later than 1 week after the grades are posted.

_If enough students have final presentations, we may not be able to cover the last module fully. In that case there will be 4 homeworks, each worth 12.5%. To clarify: this is my preferred case! I want to see lots of presentations!_

## Academic Integrity

One of the joys of university life is socializing and working with your classmates. I want you to make friends with each other and discuss the material. This is an advanced topics course; there is a high chance that your classmate will be your colleague throughout your career!

**That said, I expect all assignments (homeworks, tests, paper reviews, presentations, final projects) to be your own original work.**

If you work together with a classmate on an assignment, please mention this, e.g. in the comments of your code. If you use a figure you didn't create in a presentation, then it needs a citation. Please review the [universities policy on plagiarism](https://guides.library.ucsc.edu/citesources/plagiarism)

This class has a zero tolerance policy on cheating. Please don't do it. I would much rather get a hundred emails asking for help than have to refer anyone for academic misconduct.

## COVID Policy

We are still in the midst of a global pandemic. This quarter will surely have challenges related to this. I hope we can all approach our interactions with empathy and understanding. I will do my best to accommodate the various individual challenges that may arise. Please communicate with me early and often! 

Currently, this is designated as an _in-person_ class. It is **not** a hybrid class, that is, you do not have the option to attend remotely without an approved reason. As explained in the [attendance](attendance) section, I do expect you to plan on primarily attending in person. If you cannot attend in person for reasons related to COVID (e.g. if you or someone close to you gets sick), let me ASAP to discuss accommodations. You will not lose attendance points in these cases and I will do my best to provide lecture materials to you.

If I am unable to attend (e.g. if I get COVID), then I will aim to teach remotely as long as I am feeling well enough.

## Related Seminar

Lindsey Kuper and I are co-organizing the [Language, Systems, and Data (LSD) seminar](https://lsd-ucsc.github.io/lsd-seminar/2021fa/) this year. I highly recommend attending that course (either for credit or for personal interest). The seminar will be hybrid: if you would like to join in person, we are planning on meeting in room E2-398. If you would like to join remote, let me know and I can get you zoom links.

### Acknowledgements

This page is based off of Lindsey Kuper's CMPS290S, Fall 2018 [website](http://composition.al/CMPS290S-2018-09/). 
