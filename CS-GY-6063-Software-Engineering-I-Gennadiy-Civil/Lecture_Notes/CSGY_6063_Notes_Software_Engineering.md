# CS-GY 6063: Software-Engineering I
- [Hari Varsha V](mailto:hv2241@nyu.edu)
- Fall 2026

## Abstract
These are notes for NYU’s CS-GY 6036, a graduate class on software engineering, as taught by Gennadiy Civil in Fall 2026. Topics
include working as a engineering team, lean sldc, practice agile, go over tdd and ci. 

**Course description**: 
Learn how to conceptualize, build, deploy, maintain and re-factor software in software development teams.

# September 2, 2026

## Introduction
1. No office hours, slack is main poc.
2. No real project ideas, just organized teams. Should ship a real product by end of course.
3. Pretend you're pitching to VC, the project is like a mini-startup and the course is a mini-internship.
4. After midterm, it's be more like labs where you just showcase what you've done and there will be free-form discussions.
5. Whole class is in python. Your team depends on you and you need to depend on the team.

## Teams 
1. Every team does a 20 minute meeting, fill out report after each meeting.
2. Team of 5 present incremental progress with each spring goal.

## Grading
>[!WARNING]
> Negative 360 eval reviews is the root of all evil. Play well with others, and make sure you end up with an A
1. 50% - project is complete, deployed and accessible over the internet, compiles with established code style, and has a robust test suite with 85% coverage.
2. 40% - 360 Team mutual evaluation forms. Evaluate each other inside the team, not outside.
3. 10% - Individual Homework Assignments.
4. Grades are immutable, will not be changed no matter what.

## Respect 
1. Learn the right soft-skills and play the game - adjust according to team's culture and size of company. Learn the process.
2. Treat every person in the team/company as highly as the CEO itself. Make them feel important and noticed.

## Async Team Matching 
1. Grouped to sit together as teams, NASA exercise as a ice-breaker and team bonding experience.

## What is Software Engineering?
1. Software Engineering is the art of compromise, i.e., doing the right trade-offs with the given constraints and resources.
2. Programming is a tool, more of a means to an end. 
3. Software Engineering is programming integrated over time. We build a software system and maintain it
4. Code needs to be well readable and organized that even agents can exactly implement non-trivial features.
5. The worst thing you can do is have software graveyards. Avoid at all costs.
6. Software Engineering is a team activity, like think of the team who cracked enigma(ref: The Imitation Game). 
7. A company needs to be organized in such a way that every new employee brings in exponential revenue. Developing software is different when you're a 3 person team vs 100 vs 1000 and so on.
8. Software Engineering (def): multi person effort of multi version programming 
9. Evaluate your trade-off's and make rational decisions 
10. Really cool quote from Norman Ralph Augustine - *Software is like entropy. It is difficult to grasp, weighs nothing, and obeys the second law of thermodynamics; i.e. it always increases.*
12. Phenomena of Induced Demand in Software. Consider the The Highway Problem or The Washing Machine Paradox(re:The Cowan Paradox) to understand deeper.

## Notes 
1. Find how other companies like Linear doesn't follow agile and just generally see while agile/scrum sucks and what are some better, more productive and sustainable working models.
2. Read a chapter of the Google SWE book every week.
3. Learn top-tier product management using Linear.

# September 9, 2026

## Just Enough Agile and Scrum To Get Started
1. Recap over what software engineering is.
2. Short history of how we develop software - waterfall model.
2.1. Bunch of business analysts come together and interview customers to get requirements. Then SWEs work on the design and implement it. Then we have QAs verify it and SWEs maintain the said software.
2.2. Still prevalent today. Pitfall is obviously thinking customers know what they want and requirements are known.
3. How else do we develop software? - Iterative, Spiral, and RUP. They do waterfall in pieces. Company that originally made it got acquired by IBM and now there's a whole book.   
4. Agile is the solution: being able to move quickly. Based on a Japanese book. Intro'd cross-functional teams and save the company. They were given full freedom and less supervision with the only goal to succeed.
4.1. Started with what it means to be done in 3 months. No paper or slides, just an actual product to be shipped
> ![IMPORTANT]
> Have something ready to show by next class. Basically create the first MVP to showcase. Have daily scrum meetings, and need to present the real deal instead of running it locally. Bring up blockers early on.
4.2. Key Elements:
- Time box: Similar to how dropbox and google works.
- cross-functional Team: Work with the PO to define design decisions and features.
- Thing that can be done at the end of each box: something that is preferably can by shipped.
5. Agile manifesto. Prefer:
- Individual and Interactions: Communicate with people over doing slides and all
- Working software: better than just some docs 
- Customer Collaboration: Always speak to the customer rather than the sales doing the talking over contracts 
- Responding to change: 
6. Intro to Scrum and Scrum Masters (Apparently need to get certified and all)
6.1. Form of agile. Incorporates more of XP.
6.2. Other forms of Agile: Kanban, XP, etc.
6.3. Has a small amount of rules. It gives a deal with complexity
7. Familiarize yourself with how Scrum works in 2026 and how to do it the sane way. Don't fall into propoganda and dogma. 
8. PO is basically the lead. Sprint must have a definite goal and is fixed.


## Sprint 1 
1. Deliver the complete document for the project. Finish the doc from Brightspace.
2. What makes a good project? Should be CRUD, needs to be interactive, needs to be a web app, clear user history, unique between teams and useful in real life.

1. Context and scope
2. Goals and non-goals
3. Actual Design
3.1. System-context-diagram
3.2. API 
3.3. Data storage
3.4. Code and pseudo-code
3.5. Degree of constraint
4. Alternatives considered
5. Cross-cutting concerns

1. Creation and rapid iteration
2. Review (may be in multiple rounds)
3. Implementation and iteration
4. Maintenance and learning

When considering writing a design doc, think about these points:

1. Are you unsure about the right software design, and would it make sense to spend upfront time to gain certainty?
2. Relatedly, would it help to involve senior engineers, who might not be able to review every code-change, in the design?
3. Is the software design ambiguous or even contentious such that achieving organizational consensus around it would be valuable?
4. Does my team sometimes forget to consider privacy, security, logging or other cross-cutting concerns in the design?
5. Is there a strong need for documents that provide high-level insights into the design of legacy systems in the organization?


## Notes
1. Go over articles like Mitchellh's blog post on building large technical books. 
2. Go over articles and essays on why OOPs and Agile suck ass. Especially theprimeagen's videos.
3. Start the linear project and the github repo. Google Design Doc on the project + FigJam for system design. Already setup the CI/CD and deploy it.
4. Blocker on how to scrape data for our original data.

