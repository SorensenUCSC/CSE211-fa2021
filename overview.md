---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

title: "Overview"
layout: single
classes: wide
---

## Class Description

Welcome to CSE 211: Compiler Design! In this class we will explore one of the most import tools in computer science: the compiler. In particular, we will explore how compiler techniques can aid programmers in making their code more efficient on modern processors. When you leave this class you should be comfortable writing an optimizing (and safety checking) compiler for a simple programming language. We will explore classic topics in static analysis, but also look at modern concepts in automatic parallelization and domain-specific languages.

## Necessary Background

This class has a prereq of an introductory compiler course. However, because this is a grad course, we will have students from many different undergrad programs. It is difficult to rely on very specific backgrounds. Some compiler class experience will be helpful, but so will classes in related subjects, like programming languages, systems, and parallel programming.

Because this is a graduate level class, I do expect a general strong CS foundation. In particular, you should be:

- comfortable using a linux command-line (this is how your assignments will be submitted).
- programming in a high-level language (e.g. Python)
- programming in a low-level language (e.g. C)
- a high-level understanding of basic parsing (i.e. regular expressions and context-free grammars)
- a high-level understanding of parallel programming and computer architecture

## Class Modules

This class will be split into 5 modules, each of which are roughly two weeks:

* **Module 1: Parsing Overview:** This module will go over parsing at a high-level. This includes tokenizing, parsing context-free grammars, parser generators, and how to quickly create a parser for a simple programming language.


* **Module 2: Flow Analysis:** This module will go over different flow analysis (aka static analysis). We will discuss different AST traversals, SSA form, and applications such as pointer-analysis.

* **Module 3: Automatic Parallelization:** This module will go over how programs written for a single thread can be automatically turned into a parallel program using compiler transformations. We will discuss several types of parallelization, from SIMD units available on most modern processors, to more elaborate software-hardware co-design parallelism, e.g. Decoupled Access Execute.

* **Module 4: Domain Specific Languages:** Here we will discuss various domain specific languages and how compilers can leverage the domain constraints to perform even more optimizations. We will look at widely used DSLs for ML (e.g. tensorflow), as well as more niche languages (e.g. for graph analytics).

* **Module 5: Optimization Policies:** This module will explore the impact of compiler optimizations and how to determine if optimizations actually provide reliable and portable performance improvements. 

## Class Format

Each class is 85 minutes. I will break each lecture into two 40 minute
lectures with a 5 minute break between. I will plan to have the zoom
room open 15 minutes before class starts and 15 minutes
afterwards. You can use this time to ask questions or socialize with
your classmates.

I will enable global chat for the zoom lectures. You may use this to
ask questions or comments throughout the lecture. Peer-to-peer chat
will be disabled as it can be distracting.

_Non-protected materials_ will be hosted on this website. This
includes homework assignments, schedules, references, etc.

_Protected materials_ will be hosted on a Canvas website that you will
need your university credentials to access. These materials include
zoom links, lecture recordings, tests, grades, etc.

There will be an official forum in the Canvas that you can use to
discuss course topics and ask questions. I will not host any other
official forum for the class (e.g.\ slack or discord). Feel free to
organize yourselves. If you do so, I only ask that you make an effort
to include all your classmates and adhere to academic integrity (and
also forward me any fun pictures of pets that might get posted).

## Attendance

This is a small graduate course and live discussions will be a
valuable part of the learning experience. As such, I expect you to
make an effort to attend the live broadcast of this class on
zoom. **Attendance will be 10% of your grade**. I will upload
recordings of the class to canvas, but this is not a substitute for
attendance. I will take role at the beginning of each class.

Please message me if you will miss a lecture to avoid losing
attendance credit.

If the normally scheduled date and time will be an issue for you,
please let me know ASAP.

## Accessibility

UC Santa Cruz is committed to creating an academic environment that supports its diverse student body. If you are a student with a disability who requires accommodations to achieve equal access in this course, please submit your Accommodation Authorization Letter from the Disability Resource Center (DRC) to me by email, preferably within the first two weeks of the quarter. I would also like us to discuss ways we can ensure your full participation in the course. I encourage all students who may benefit from learning more about DRC services to contact DRC by phone at 831-459-2089 or by email at drc@ucsc.edu.

## Office Hours:

Office hours will be 3 - 4 pm on Wednesdays. The Zoom link can be
found on Canvas.

I will hold additional office hours by appointment. Please don't
hesitate to email me!

_If you are in a different time zone that makes these hours difficult,
please message me and we can make accommodations_

## Homework:

There will be one assignment per module, for a total of 5 homeworks.

I have set up an Amazon EC2 server where homework will be turned
in. The Canvas website has instructions for accessing this server and
how to submit assignments.

You are generally free to use any language, library, scripts,
etc. that you would for the assignments as long as they execute on the
EC2 server. I am happy to install additional software if you'd like;
just message me. Each homework will have a recommended
language/framework to use. These recommendations should be widely
accessible on a variety of machines, but will definitely be available
on the EC2 server.

You do not have to use the recommended language or framework, but
please message me first to approve substitutions. Your solution will
have to execute on the EC2 server and I may need to install
software. Depending on your choice, I may not be able to provide as
much assistance during office hours.

The homeworks will be posted at least 2 weeks before they are due and can be found [here](homeworks.html).

## Tests:

There will be two "tests" in this course: a midterm and a final. The
midterm will be worth as much as a single homework assignment
(~10%). The final will be worth more at 30%

I put tests in quotes because it is extremely difficult to have tests
in virtual classes. I'm not going to try anything crazy like [eye
tracking
software](https://www.vox.com/recode/2020/5/4/21241062/schools-cheating-proctorio-artificial-intelligence). You
will get the test as pdf worksheet and have 2 days to complete it. I
will design the tests to take ~85 minutes, the time of a class. You
are free to consult the internet, any books (or even your pet dog if
you have one). I simply request that you do not discuss the test with
each other until everyone has turned it in.

## Paper Assignment

You have the option to substitute one homework (or midterm) for a
paper assignment. A paper assignment consists of finding a recent
paper that has a strong compiler component and writing a short review
for the paper. You are also required to present a 15 minute overview
of the paper to the class. We will do these presentations in the final
week.

The review should roughly be 4 pages double spaced. Please organize it
as follows:

- Motivation: what is the problem and why is it interesting?
- Compiler component: what is the compiler component and how does it relate to what we have learned?
- Illustrative example: find a small example that you can clearly explain, especially related to the compiler component. This might be a small program and a description of how the compiler transforms the program.
- Key results: what are the important results of this paper and how did the compiler enable them?

Please pre-approve the paper with me. Additionally, I can suggest
papers. The reports will be two weeks before the quarter ends. If you
do all homeworks and the midterm, then your lowest grade will be
dropped. Dates for the paper assignment are summarized [here](homeworks.html#paper-assignments-and-final-projects).

If you are a PhD student, I strongly recommend doing a paper
assignment for one of your related works.

## Final Project

You can substitute the final exam for a final project. The project
will need to be pre-approved by me no later than 2 weeks before the
end of the semester. To propose a project, please write a 1 page
summary clearly describing the compiler element to the project and how
it relates to what we are learning.

Your final project deliverable will be a 5 page double spaced report
detailing your project with an emphasis on the compiler aspects of
your project. Think of it like a mini conference paper, with a
required "compiler design and implementation" section. I expect this
section will be roughly 2 pages of your report. You will also be
required to give a 15 minute presentation about your final project to
the class. Dates for the final project are summarized [here](homeworks.html#paper-assignments-and-final-projects).

If you are a PhD student, I strongly recommend thinking about a final
project related to your thesis.

## Grade Breakdown

- Attendance: 10%
- Homeworks: 50% (10% each)
- Midterm: 10%
- Final Exam/Project: 30%

I will be grading all assignments and tests. If you want to discuss a
grade, please contact me no later than 1 week after the grades are
posted.

_If enough students have paper and final presentations, we may not be
able to cover the last module fully. In that case there will be 4
homeworks, each worth 12.5%. To clarify: this is my preferred case! I
want to see lots of presentations!_

## Academic Integrity

One of the joys of university life is socializing and working with your
classmates. I want you to make friends with each other and discuss the
material. This is an advanced topics course; there is a high chance
that your classmate will be your colleague throughout your career!

**That said, I expect all assignments (homeworks, tests, paper
  reviews, presentations, final projects) to be your own original
  work.**

If you work together with a classmate on an assignment, please mention
this, e.g. in the comments of your code. If you use a figure you
didn't create in a presentation, then it needs a citation. Please
review the [universities policy on
plagiarism](https://guides.library.ucsc.edu/citesources/plagiarism)

This class has a zero tolerance policy on cheating. Please don't do
it. I would much rather get a hundred emails asking for help than have
to refer anyone for academic misconduct.

## Privacy

I want to include a quick note on Privacy. I will largely be using Zoom for remote lectures. You should be aware that:

- I will be recording lectures to host on Canvas for you to review. Things you do or say will be recorded. I doubt that this will be an issue, but if you want me to remove any part of the recording, please just let me know.
- Zoom chats are not private. Please be respectful and kind and assume everyone can see what you are typing.
- I will use best-practices to keep our Zoom lectures private to the class. Despite our best efforts, [Zoom has a checkered history w.r.t. privacy](https://www.theverge.com/2020/4/1/21202584/zoom-security-privacy-issues-video-conferencing-software-coronavirus-demand-response). However, Zoom is the best tool we have available and these risks are simply part of the reality we must deal with.

## Related Seminar

Lindsey Kuper and I are co-organizing the [Language, Systems, and Data
(LSD) seminar]() this year. I highly recommend signing up for that
course alongside this one. Because it is a remote seminar, we will
have student speakers from all over giving presentations; come join
us!

## Acknowledgements

This page is based off of Lindsey Kuper's CMPS290S, Fall 2018
[website](http://composition.al/CMPS290S-2018-09/). If you enjoy the
material in this compiler class, consider taking an advanced topics
class from her!