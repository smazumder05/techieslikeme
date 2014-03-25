---
layout: post
title: "The hardest part about software development is to decide what to develop"
modified: 2014-03-24 16:24:17 -0400
tags: [software development]
image:
  feature: 
  credit: 
  creditlink: 
comments: true 
share:  true
---
> #### "If I had an hour to solve a problem I’d spend 55 minutes thinking about the problem and 5 minutes thinking about solutions.” – Albert Einstein. 

I see computing mainly as problem solving; therefore, it is critical to understand the real world problems that a particular software development initiative needs to solve.  I used to get frustrated with my users and clients’ inability to make up their minds and clearly state their problems that needed to be solved.  Then I realized that as a software engineer it is my responsibility to work closely with my users and help them define their issues. 
 
###Problem Domain

A litmus test on understanding a problem domain that needs to be solved is to write a one pager (not more than that) on the essence of the problem that I am tasked to solve.  Often, I have seen developers on my team (including myself) describe a very different problem to the one that needed to be addressed. Describing one’s understanding of the problem in one’s own words and in a concise manner clarifies any glaring misunderstandings. It is very helpful to me to begin a project with a one pager.

###Requirements Gathering
Any attempt to gather ALL possible requirements at the onset, I believe, will fail or cause significant delays to the overall project. Therefore my goal during early stages of software development is to identify a few key requirements and start working from there. As a mainly iterative process, requirements needs to be identified, captured, prioritized and acted upon throughout the lifecycle of a project.

Software requirements and usefulness truly becomes relevant to users once they get to use it. Therefore, the initial versions of any software should satisfy some key requirements and then build from there. As a software matures, its users almost always find more and more innovative ways of applying it into their everyday lives, whether work or personal. Hence, requirements gathering for a software is never really over.

The two main areas of requirements that needs to be covered are functional and nonfunctional or system level requirements.  In this article, I will focus on how some of the key functional software requirements can be hashed out by finding answers to some pointed questions.  [I have created this list in github, so please feel free to add any other general questions that might help us formulate better requirements.](https://github.com/smtechnocrat/softwaredevelopmentproblem/blob/master/functional-requirements.md)

###Functional

Here are the main questions for which I need answers to capture some of the initial requirements for a software development project:

1. What is the business objective behind the requested functionality?
2. What basic functionality do you need for this part of the system?
3. What is the underlying goal of the requirement?
4. Is this particular design critical to the business goal, or would any design be equally effective?
5. How does it work today?
6. What specific steps do you go through to complete a task in the system?
7. What do you not like about the system today?
8. If X does not happen, then what should happen?
9. What do you want to have happen in the future?
10. Are there any known constraints from other systems or users?
11. What are the non-functional requirements that apply for each of the users, operating environments, and interfacing systems?
12. Keep drilling deeper with variations of “why?”

In order to formulate use cases, here are some questions that need to be answered:

1. Use case description
  * What is the actor’s goal?
  * What are the high level actions the actor will need to take to reach that goal?

2. Assumptions
  * What assumptions are we making when analyzing this use case?

3. Frequency of Use
  * How many times per minute, hour, or day will this use case be executed?

4. Actor
  * Who uses the system (what is their job)?
  * What other systems will interact with this system?
  * Who or what provides information to the system?
  * Who or what receives information from the system?

5. Trigger
  * What event causes this use case to happen?
  * What actor initiates this use case?

6. Preconditions
  * What conditions must be true before this use case can begin?
  * What state is the system in before this use case can begin?

7. Success End Conditions
  * What conditions must be true when the use case ends?
  * What state will the system be in at the end of the use case?

8. Main Steps
  * How does the actor interact with the system?
  * What does the system do at this step? (present options, display data, execute a process)?
  * What does the system do next?
  * What does the actor do next?
  * Is there part of this use case that is another use case called by multiple other use cases?

9. Alternative Courses
  * What possible error conditions exist at each step of the main scenario?
  * If X doesn’t happen, what should happen?
  * What are the interrupts that can happen at any time?
  * What is the “non-happy” path?
  * What other possible actions can the user take at each step?
  * If the user cancels out at any step, what should happen?

Next time, I will cover the *non-functional requirements* of any software.  One critical aspect that is often overlooked during requirements gathering is the non-functional system level requirements such as availability, scalability, etc. Therefore, I have also created a list of all non-functional requirements that a system may need to meet. Not all aspects of these non-functional requirements may be applicable for all software but it is useful to have all aspects covered. 
