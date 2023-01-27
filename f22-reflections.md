# Jeffrey's Research Log! Fall
---
*Research Topic:* Integrating Compositional Symbolic Execution into the Binary Analysis Platform, angr

*Main Research Paper:* Compositional Symbolic Execution Using Fine Grained Summaries

*Research Description:* Symbolic Execution's greatest challenge is its inability to maneuver around path explosion. Loops and recursive calls cause symbolic execution to malfunction and create far too many branches than necessary. Thus, this greatly detriments the scalability and efficiency of symbolic execution as the same code block will be analyzed and sent to the constraint solver an X amount of times. Compositional Symbolic Execution solves this by reducing calls to the constraint solver, yet this new version of symbolic execution has not been made publically available, especially for Binary Analysis Platforms. The Bultan Group - Erica Liu, Adrian Lindell, and Jeffrey Mun - will be integrating CSE into angr for that sole purpose. 

---
## Week #, MM/DD/YYYY

### Weekly Goals
- [] Goal 1
- [] Goal 2

__Day, Time Spent__
- [] Task 1
- [] Task 2

__Key Takeaways__
- [] Takeaway 1
- [] Takeaway 2

__Reflections__
REFLECTION PARAGRAPH

## Week 10, 11/27/2022

### Weekly Goals
- [] Finalize Proposal
- [] Practice Presentation
- [] Address Feedback and change proposal accordingly

__Monday, Time Spent: 3 hrs__
- [X] Primary V-Lab meeting, Sophia, Jeffrey, Erica, and Adrian in attendance
   - Might do a practice run of the presentation in front of everyone
   - everyone also wants to watch our final presentation...
- [X] Met up with Laboni in the Verification Lab to flesh out some details about our proposal
   -  I was the only one there, it was a 1:1 meeting
   -  More clarification on CSE's significance and the significance of transporting its functionality onto angr
      - CSE reduces calls to the constraint solver
      - CSE exists for source code, but not for binary code
      - angr is a binary analysis platform that works on binary code
         - significance of binary code = might not always have the soruce code
- [X] Revisited feedback with Prof. Mirza in class
   - we have a lot of work to do. ;'(

__Tuesday, Time Spent: 2 Hrs__
- [X] Scheduled group meeting, Sophia, Jeffrey, Erica, and Adrian in attendance
   - Addressed feedback comments and made changes to the proposal
   - I worked on adding a constraint solver section, fleshing out our problem statement, and rewriting the motivation
   - Also working on presentation slide deck to prepare for our run through tomorrow

__Wednesday, Time Spent: 2 Hrs__
- [X] Finished Research proposal
- [X] Group Meeting, Sophia Jeffrey Ercia and Adrian in attendance
- [X] Sent research proposal final draft to Laboni for final critiques

__Thursday, Time Spent: 1 Hr__
- [X] Finished Research Presentation Slides
   - Practiced in front of Laboni and Professor Bultan
   - Received critiques and changed accordingly
   - Finalized last minute details to prepare for Final Presentation
   - Professor Bultan said that our proposal was very exciting and will be impressive to pull off :)

__Monday, Time Spent: 2 Hrs__
- [X] Performed final presentation to ERSP group
- [X] Submitted Final Proposal into Gauchospace
   - [X] Finished with Fall Quarter of ERSP

__Key Takeaways__
- [X] ERSP is done!
- [X] Gonna miss Sophia, but I am excited to work with everyone moving forward


---
## Week 9, 11/20/2022

### Weekly Goals
- [X] Figure out goals with ERSP
   - View Week 8 Reflection
- [X] Decide if I want to continue with ERSP
   - Yes
- [] Finalize presentation and proposal for submission
   - DELAY TO NEXT WEEK

__Sunday, Time Spent 2 Hrs:__
- [X] Found more graphics for the proposal
- [X] Expanded more on KATCH and compositional symbolic execution vs differential symbolic execution vs functional symbolic execution
- [X] Clarified more on Fine Grained Summaries


__Monday, Time Spent 1 Hr:__
- [X] Conducted grad student interview with Mara, a PhD student in the Verification Lab
- [X] Reflection 4 

__Saturday, Time Spent 1 Hr:__
- [X] Last minute changes to the presentation slide deck
   - Reread the CSE paper to highlight important sections necessary for our presentation
   - Transport comments from Laboni onto the primary google dock
- [X] Investigate more on the constraint solver and why it is important for CSE

__Key Takeaways__
- [] Thanksgiving break makes it hard to do work
- [] Grad school is an interesting direction that I've never thought of.

__Reflections__
Not much to really update, I think this week was really chill. I can't really do too much work as we haven't received our feedback yet, but it is nice to take a break from worrying about the proposal all the time.

---

## Week 8, 11/13/2022

### Weekly Goals
- [X] Receive peer review on our proposal
- [X] Finalize relevant research papers
- [] Test out angr and become familiar with python / ocaml
   - [] Determine how to recreate the Control Flow Graphs / change angr's inner implementation
   - DELAYED TO NEXT WEEK

__Friday, Time Spent: 1.5 Hr__
- Had Grad meeting with Laboni, Sophia, Jeffrey, Adrian, and Erica in attendance
   - Went over Compositional Symbolic Execution
   - Worked over our misunderstandings
      - Not pseudocode, but rather abstract symbols for variables etc...
- Got the news from Sophia that she will not be continuing ERSP for the W23 / S23 quarters.
   - Reflect on this

__Thursday, Time Spent: 1 Hr__
- Originally had our grad meeting scheduled, but it got sidetracked due to another VLab meeting happening at the same time
   - Pushed to Friday
- Setup angr on SSH Linux computer

__Wednesday, Time Spent: 2 hr__
- [X] Went to writing lab to receive feedback
- [X] Finished project proposal
   - Project proposal rewrite went really well! We used some of the peer feedback to guide our writing, but most of our writing and edits were taken from our grad mentor (Laboni) and Chinmay's comments. The writing lab wasn't too useful though, I thought that they didn't know how to read a research paper and that it was mainly directed towards literature and essay-esque writing.
   - Worked on assignments due the next week

__Tuesday, Time Spent: 1 hr__
- [X] Wrote peer review for Prof. Gupta's group

__Monday, Time Spent: 1 hr__
- [X] No writing lab, got cancelled due to strike
- [X] Reread over Laboni's 2nd revision and Chinmay's comments on proposal
   -[X] Fixed similar mistakes pointed out in both reviews

__Key Takeaways__
- [X] Why do I really want to do research? What do I want to gain out of it?
- [X] Symbolic Execution is Hard..

__Reflections__
Sophia just told our group that she will not be continuing with ERSP, and it really got me thinking about why I want to do research and what my motivations are for the group. Some factors I am considering is time committment, effort, and just general interest, but I know that some of my other group members are also a little iffy on the whole subject. ERSP for me was a way to get closer with my TAs and other Professors at UCSB, making more friends, and getting more invested in UCSB's CoE culture. Have I achieved this? Yes. But now that I am starting to do more research, my shift for ERSP has changed to a more academic standpoint. 

---

## Week 7, 11/06/2022

### Weekly Goals
- [X] Receive feedback from Chinmay and Laboni on our research problem switch
- [X] Finish proposal enough for Peer Reviews
- [X] Determine new scope for project and do appropriate research

__Wednesday, November 9 Time Spent 2 hr__
- [X] Free proposal writing time in class, worked with Sophia over Zoom
   - Found more clarification on what our project should be
   - Determined questions for Laboni at tomorrow's lab meeting
   - Asked Prof. Mirza and Chinmay on appropriate stylings / how to approach a changed direction
   - Reread our research papers individually and fleshed out any decrepancies in our paper

__Tuesday, November 8 Time Spent 2 hr__
- [X] 2 hour team sync, Erica, Adrian, Sophia, and Jeffrey all in attendance
   - Reviewing assigned research paper tasks
   - Deciding new approach for paper
   - Rewrite proposal to fit new approach

__Monday, November 7 Time Spent 2 hr__
- [X] Read over sample proposal and give critiques
- [X] Read paper #13 and #20 to find more info on different forms of DSE
   - Under constrained symbolic execution w/ fine grained summaries
   - Create questions for tomorrow's team sycn
   - 
__Reflections__
REFLECTION PARAGRAPH

---

## Week 6, 10/31/2022

### Weekly Goals
- [] Goal 1
- [] Goal 2

__Thursday, November 3rd Time Spent: 1 hr__
- [X] Found that function-wise differential symbolic execution has already been implemented
   - [X] Changing our project scope to a new direction
   - [X] Need to find out what direction we want to go into
- [X] Read more research papers
   - [X] 13 Compositional symbolic execution using fine-grained summaries 
   - [X] 20 Under Constrained Differential Symbolic Execution: Generating fine-grained summaries
- [X] Sophia, Jeffrey, Erica, and Adrian all in attendance

__Wednesday, November 2nd Time Spent: 1 hr__
- [X] Group meeting on Zoom from 6:00-7:00
   - Caught up on Github assignment
   - Organized thoughts for Thursday lab mentor meeting

__Monday, October 31st Time Spent: 1 hr__
- [X] V-Lab meeting from 11:00-12:00
   - Received feedback from Professor Bultan on project scope
   - Sophia took note 
   - Sophia, Adrian, Jeffrey, and Erica all in attendance

__Reflections__
REFLECTION PARAGRAPH

---
__
## Week 5, 10/24/2022

### Weekly Goals
- [X] Finish Related Works section of Proposal
- [X] Figure out direction for proposal
- [] Setup angr on CSIL and Mac
   - Finished Mac setup
- [X] Begin Programming
- [X] Setup Proposal

__Friday, October 28, Time Spent: 2 Hours__
- [X] Zoom meeting with ERSP group to finish initial project proposal
   - Took around 1 hour when we were all working together
- [X] Sent over initial project proposal to Laboni for review

__Thursday, October 27, Time Spent: 2 hours__
- [X] Meeting with Laboni
   - Erica, Sophia, Adrian, and Jeffrey in Attendance
   - Received login information for Linux systems
   - Established project scopes
      - Comparing Function-Wise DSE in BAP vs Angr

__Wednesday, October 26, Time Spent: 2 hours__
- [X] Setup Angr on Mac
- [X] Create script to fast-install angr
- [X] Play around with software
- [X] Created possible research proposals
   - Variation in for loops and recursion (1 to 10 and 10 to 1 and while i < 10)
   - Improving Angr with a GUI
   - Ways to save memory through binary analysis
   - Cybersecurity DSE on computer program states
   - Crytography to reduce scope of possible passwords
   - Symbolic Execution to deliver satistical data on branches (Grammarly for Code)

__Tuesday, October 25, Time Spent: 1.5 hours__
- [X] Wrote summaries for group-agreed important papers
- [X] Edited introduction section on proposal (Overleaf)
- [X] Researched more gaps in literature

__Monday, October 24, Time Spent: 2 hours__
- [X] Attend VLab meeting
- [X] Update mural with new extensions of papers
   - BAP and ANGR focus
   - Stray away from Debugging and testing softwares
- [X] Write related works section 

__Key Takeaways__
- [X] Coming up with new ideas is hard, every good idea or interesting idea I have has already been solved / done
- [X] With such a hard topic to learn, I find it difficult to understand the subject enough to propose a research direction

__Reflections__
REFLECTION PARAGRAPH

__Literature Search Part 3__
*Write a one-paragraph summary of the paper, in your own words*
*Write about the relationship between this paper and your original paper*
*Specify why you chose the paper*

**Paper 1: Using Binary Analysis Frameworks: The Case for BAP and angr**
One of the main tools for applying symbolic execution to computer programs is a binary analysis platform. When a project executable, also called a binary, is inputted into a binary analysis platform, the program does all of the heavy lifting which converts the binary code into an intermediate mathematical representation and creates a logical method summary on it. The two leading platforms for binary analysis are angr and BAP.

This paper summarizes the uses of a binary analysis platform and cross-compares BAP and angr to evaluate each others' strengths weaknesses. angr's main strengths are its ease of use, python compatibility, and the ability to work on a program hollistically. BAP's main strengths are its high functionality, OCaml compatibility, and its ability to split a program into individualized function-wise bits.

We chose this paper because one of our main research scopes is to cross compare the two programs on how they handle new execution methods. This paper provided the best motivations for our research scope and helped our group understand the differences and significances between binary analysis platforms.

**Paper 2: Compositional Symbolic Execution Using Fine-Grained Summaries**
Symbolic execution's weakness is its inability to take care of path explosion, leading to memory and runtime inefficiencies. This paper introduces the idea of compositional symbolic execution, separating a program into compositional pieces, using fine grained summaries, matching input-output pairs based on arbitrary code blocks rather than entire functions. This solves issues to the underlying constraint solver because it abstracts symbolic execution into digestible parts.

We chose this paper because it will be one of the methods we are trying to implement into BAP / angr for cross comparison. Can both of the programs support it? Does one of them support it better than the other? This paper provides a very good understanding of compositional symbolic execution as well as a depper dive into its capabilities. 

**Paper 3: Under-Constrained Symbolic Execution: Correctness Checking for Real Code**
This paper introduces a novel framework, UC-KLEE, to solve the scalability issues of symbolic execution. Focusing more on a debugging application of symbolic execution, this paper uses the program to spot-apply patches to see whether a program would crash / would not return an exepcted output. This program goes even further to find memory leaks, unitialized data, and areas that would have been glossed over through traditional debugging methods.

We chose this paper because it is similar to our idea of executing symbolic execution on a larger program by breaking it down. We are cross comparing programs on angr and BAP, but this adds a chance for us to think about applicability in the real world.

--- 
## Week 4, 10/16/2022

### Weekly Goals
- [X] Find more resources to begin project
- [X] Be ready to start the next week and begin writing proposal

__Monday, October 17 Time Spent: 2 Hour__
- [X] Verification Lab Meeting
   - Adrian took notes
   - Went over current progress within the Lab
   - Discussed ERSP progress and possible start times
- [X] Dicussed with Prof. Bultan on possible opportunities
- [X] Teaching topic done

__Wednesday, October 19 Time Spent: 2 Hours__
- [X] ERSP Group Meeting
   - Taught each other the rest of the teaching topics
   - Caught up on Constraint-Effect Solving and ANGR

__Thursday, October 20 Time Spent: 1 Hour__
- [X] VLab Advisor Meeting
   - More clarification on Logical Method Summary and Constraint Solving
      - Proof by Negation
- [X] Research Proposal Thinking
   - Function-Wise Differential Symbolic Execution

__Sunday, October 23 Time Spent: 2 Hours__
- [X] Meet with ERSP Group to finish literature proposal
- [X] Find more research papers to connect on Mural
- [X] Write related works section

__Key Takeaways and Reflection__
- We have the luxury/deficit of a really hard topic
   - I enjoy having the capacity to learn so much, but I don't enjoy how unapplicable it is to my daily life.
   - I feel like groups working with more real-world-applicable projects have the pleasure of synthesizing daily inquiries with their technologies, but ours is so computer-focused.
---

## Week 3, 10/9/2022

### Weekly Goals
- [X] Be better at DSE
- [X] Figure out my commitments and make priorities


__Saturday, October 12 Time Spent: 2 Hour__
- [X] Created slides for teaching topic
- [X] Practiced creating logical method summaries for my own work
- [X] Included more information on logical method summaries

__Thursday, October 12 Time Spent: 1 Hour__
- [X] Meeting with Laboni
   - Discussed future plans and programming ideas
   - Revisited teaching topic progress
   - Updated progress
   - I should visit more Logical Method Summaries
   - Discussed best venues for our firled
- [X] Preliminary teaching topic preparation
   - Read research article and watched MIT lecutre video on Symbolic Execution

__Wednesday, October 12 Time Spent: 1 Hour__
- [X] Catch up meeting with Bultan group
   - Went over VLab notes
   - Reviewed teaching topics
   - Considered questions for Laboni
   - Attendees: Sophia, Jeffrey, Erica, Adrian
- [X] Consider time commitment for ERSP and converse with Prof. Mirza

__Tuesday, October 11 Time Spent: 1 Hour__
- [X] Finish research for teaching topic
   - Resources referenced:
   - https://en.wikipedia.org/wiki/Symbolic_execution
   - https://dl.acm.org/doi/10.1145/1453101.1453131
   - Report given by Laboni
- Link to teaching topic: 	https://ersp-22-reflection-logs/teaching_topic.md

__Key Takeaways__
- [X] Effort and interest are all that is needed to make progress
- [X] It is great to be in a discipline where there is so much to choose from
- [X] I can take things slowly, I'm only 19

__Reflections__
There is a huge rat race in Computer Science where everyone is trying to be on top of the pyrmaid, but that isn't something that should affect my own progress. Why bother pursuing avenues I'm not even interested in? It is okay to take things slow, but with passion. 

---

## Week 2, 10/02/2022

### Weekly Goals
- [X] Develop skills on learning how to read a research paper
- [X] Develop more understanding about research topic and terminology
- [] Establish a research question to frame focus for the upcoming weeks
- [X] Familiarize self with V-Lab setup and people
- [X] Read over a research paper on Symbolic Execution to become more familiar with research topic

__Saturday, October 8 Time Spent: 1.5 Hours__
- [X] Finished second pass of DSE Research paper
   - I realized that I had actually understood it a lot better my first pass than I expected
   - This was just for more clarity, but the math makes sense when I read it
- [X] Research more into teaching topic

__Thursday, October 6 Time Spent: 2 Hours __
- [X] Met with graduate mentor, Laboni, and receive more clarity on difficult concepts from the DSE first pass
- [X] Assign teaching topics accordingly
   - I was assigned with taking a deep dive into Differential Symbolic Execution to make it easier for our group to understand
- [X] Learned about other important topics and programs
   - ANGR
   - BAB
   - Constaint Solving
- [X] Begin reading "State of War" and a survey of binary code similarities
- Notes from meetings, courtesy of Sophia Weiler: https://docs.google.com/document/d/1J7kZYvHW4ZUQ6APIMgC_ARZvYdpaMYOS3W3i-xElWvg/edit?usp=sharing

__Tuesday, October 4 Time Spent: 1.5 Hours__
- [X] Read over Differential Symbolic Execution research paper by Person, Dwyer, Elbaum
   - Notes: https://github.com/Jumshim/ersp-22-reflection-logs/blob/main/cs110-research-activities/research_first_pass.md

__Monday, October 3 Time Spent: 1 Hour__
- [X] Attend VLab Meeting at meet research time with Professor Bultan
- [X] Read over slides on Symbolic Execution (25-35)
   - **Symbolic State** : maps variables to symbolic values
   - Programs are run on symbolic values
   - **Path Condition** is a quantifier-free formula that encodes all branch decisions taken so far
      - When using math operators (+, -, *, /, <, >, = ...), checks if they are valid programs. Are they both integers?
      - All paths form a program's execution tree which deem certain paths as feasible and others unfeasible


__Sunday, October 2 Time Spent: 1 hour__
- [X] Establish Meeting Time
- [X] Read and Take Notes on "How to Read an Engineering Research Paper
   - Research paper outline:
      - Introduction states motivations and outlines solution
      - Body: author's solution to a problem and detailed evaluation of solution
      - Recap: Dicussion of primary contributions
   - Important Questions to Keep in Mind:
      - What are the motivations? Unstated people problem vs technical problem? Why o we not have a trivial solution yet? What are our solutions?
      - What is the proposed solution? How is it achieved and what makes it better than the status quo?
      - Evaluation of Proposed solution? Make the case for the idea
      - Analysis of Identified Problem: Pros, Cons, Flaws, Benefits, Arguments,...
      - What are the contributions? Ideas, software, techniques are also included in contributions
      - What are future directions?
      - Leftover questions? Future takeaways?

__Key Takeaways__
- [X] I need to touch up on my Discrete Mathematics skills
- [X] Research papers aren't always determining the same goal, they can be very hard to understand and read
- [X] I think our group is the best >.<

__Reflections__

The more I learn about the reseach project and interact with my group mates, the more excited I become. I genuinely believe that our project is the most interesting and can't wait to start doing hands-on experiments and formulating my own thoughts on it. I do think it has a very high standard of entry, these research papers are very confusing, but I know it will be worth it in the end. BULTAN SUPREMACY!

---

## Week 1, 09/26/2022

### Weekly Goals
- [ ] Become friends with project-mates
- [ ] Successfully onboard required materials to begin research proposal brainstorming

__Thursday, September 29 - Time Spent: 1.5 Hours__
- [X] Established boundaries and communicated with teammates
- [X] Made a cute group chat so we can communicate
- [X] Organized first meeting time to finish research preparation and the offical main meeting (Next Wednesday, October 5 from 5:00-7:00 PM)
   - Established smaller meeting times where everyone is available for mentor meetings
   - Preferred modes of communication established

__Tuesday, September 28 - Time Spent: 2 Hours__
- [X] Wednesday Pre-Class Assignments
  -   Initialized research logs: Chose to write my logs on Github to force myself to learn proper git flow, markdown language, and repository management
  -   Wrote reflections
  -   Read through the ERSP contract and signed the consent forms
- [X] Answer Reflection-Log Questions

__First Log Reflection__

How did the logs differ in style (not just in content)? What advantages do you see in one style over another?
- From reading through the sample reflection logs, they each differred in the format, writing style, and organization. The main difference in format I noticed was the choice between Github Markdown Pages and a typical Google Docs format. Each of the stylistic design choices were also unique to each person (colors, pictures, bold, headers, etc...), showing that these effort should be put into these reflection logs to make them individualized projects. The writing style also changed person to person, some kept it short and simple while others took the time to write a whole diary entry. Finally, in terms of organization, every ERSP reflection log had similar requirements (goals, reflections, tasks, time spent, date ...) but the way they were synthesized onto a page was different. 
- For the advantages of the style, I think it just depends on the person. Google Docs versus Github Markdown both have their respective pros-and-cons (familiarity and usability vs challenging and learning). Bullet-point-esque and diary reflection logs just reflect how a person thinks and mirrors a person's thoughts onto paper.

How do you think the logs were useful, both to the researcher as well as those working with the researcher?
- Keeping an organized system of reflection is useful in almost every scenario, but writing logs in a research standpoint adds more focus, critical thinking, and back-traceable history. Just think about it, writing about one's thoughts isn't easy. For a researcher, just remembering about what they had done, what inspired some emotions they felt, and what conflicts happened forces them to grow individually and revisit important topics which would have disappeared as an afterthought. For those working with the researcher having these logs enables a better working environment as well as an orderly system of tracking goals and progress. 

Did the students keeping their logs seem to meet their goals? Did they get better at meeting their goals over time?
 - The students did seem to meet their goals! Of course the zealousness of the reflections and effort put in started to drop off as more time in the year progressed, but I am pretty sure they managed to accomplish as much as they wanted to. Whenever there was an unfinished goal, they just pushed it to the following week (of course for bigger goals this happened more and more frequently as time progressed), but I'm sure they accomplished what they wanted to do.
 
What makes me most excited about ERSP, and why?
- The #1 bringer of excitement is the chance to meet more friends. I have not had too many opportunities to meet many engineering majors, so the fact that I will be spending so much time with the same people, through struggles and triumphs, is a very warm thought. 

What makes me the most nervous about ERSP, and why?
- The #1 bringer of anxiety to me is the fear of not having enough time. What if I choose a research direction which is millions of times more complex than I anticipated? What if I do not vibe with my teammates? What if I am forced to choose between two of my favorite commitments because a day is only 24 hours? 
