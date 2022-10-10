# Differential Symbolic Execution by Person, Dwyer, and Elbaum
### Jeffrey Mun 5970595 Professor Bultan's Group
----
# Read the paper's abstract. Then record in your reading log what you think the main problem the paper is solving is, and what you think the paper's main contribution is. This should be in your own words.
- Current Problem: Existing techniques for characterizing code changes are imprecise and lead to unnecessary maintenance efforts
   - Main scope: Detecting and characterizing effects of software changes for software maintenance upkeep
   - Solution: Application of symbolic execution techniques which compute precise behavioral characterizations of changes, *Differential Symbolic Execution*

# Now, read the introduction, and highlight or underline any words, terms or concepts that you do not understand, but don't stop to try to figure them out, yet. When you have finished reading the introduction, answer the following in your reading log:
- Regression testing: differences are used to focus re-testing efforts by selecting only test cases which exercise modified selections of codde
   - Current testing methods: source file *diff*, but fails with negligible changes to syntax or formatting
- Why DSE? DDSE allows a program to "skip" the symbolic execution parts of a program that are unchanged between versions
   - Reduces analysis costs and avoid fundamental limitations of symbolic execution
   - Supports a wide range of program evolution tasks such as equivalence checking and regression test generation
   - Precisely characterizes changes between two program versions

# Give more detail about the specific problem(s) that this paper is addressing. While your answer above might have been very general, you should try to give more detail here.
 - More specification steps why DSE is better than *diff* or regular SE
   1) Precisely characterizes behavioral program differences through symbolic execution
   2) Develops techniques to compute over-approximating symbolic methodd summaries by identifying and automatically summarizing the behavior of common program fragments
   3) Defines and characterizes behavioral equivalences between program / version differences
   4) Post-processing symbolic execution results are computed to find such differences
   5) Defines conditions when DSE analysis results account for program behavior
   6) Describes applications of DSE to support the automation of program evolution tasks

# What terms or concepts are you confused about, and how important do you think each will be to your understanding of the paper?
 - Equivalence Checking
 - Regression Testing
 - Black Box Testing
 - White Box Testing
 - Equivalence and Deltas

# Next, skip to the "Experiments" or "Results" section and read it, again continuing to highlight (but not worry too much about) things you don't understand. Then, in your log record the answer to this questions: "How does the author show that their approach is successful? What evidence does the author provide? Is it compelling"
 - The author shows that their approach is successful by mathematically and logically proving how equivalcne-judged-based testing are sound on basic functions
 - There aren't official conclusions or results to the research question, rather this paper is presented more expositorily instead of researchy
  - They break down the functions of testing and what aspects are essential to testing
  - Logical values, Program Behavior, Symbolic Program State, Incomplete Program summaries, Abstract summaries, Equivalences and Deltas, DSE variations, Error handling, and Tool Support
  - Through mathematical proofs and examples, they show that DSE offers ways to accomodate for the essential values of testing


# Now, read the "Background" or "Related Work" section. After you are done, answer this question in your log: "How does the work in this paper build on what has been done before?" Your answer doesn't have to be perfect. Just give it your best shot. You'll answer this question again on your next pass.
 - What tools are referenced in the Related work section?
  - Source Difference
  - Logitudinal Program Analysis
  - Assembly code
- How does the research in question use these tools?
  - Originally, program differences have been adequate in judging the differences in source doe
    - Yet, the imprecision of these techniques cause larger parts of a program difficult to decipher and focus on
  - The paper also uses the idea of longitudinal program analysis, or targeting program analysis to version histories, in their work
  - The authors calim that DSE is the first instance of longitudinal analysis framework which realizes these benefitss
    - Compares and contrasts LPA to show that DSE provides a more comprehensive differential program

# Finally, read the "meat" of the paper which describes the new approach or technique that the paper proposes. Continue to highlight what you don't understand, but also highlight ares that you feel are important. Use a different annotation for each, so you can distinguish between them. When you are finished, answer these questions in your reading log:
**3 Summarizing Program Behavior**
- Symbolic summaries capture a set of distinct cases of a program's behavior
  - Loops, recursion, and complex arithmetic expressions result in variedd symbolic summaries
  - Precision is a concern (more complexity = more paths)
  - Completeness is a concern (one summary is more complete than another due to feasibility)

**4.1 Functional Equivalence and Delta**
- Function equivalence ignores the internal details of a method (syntax, formatting, structure) and focuses on "what" effect it gives for an input
   - Similar to black box methods of testing
 - *Delta*: captures behavioral differences between methods symbolically

**Conclusion**
- Core of DSE: deltas and equivalence
   - Equivalence and deltas: Sensitive only to black-box behavior that consider a measure of white-box behavior
- Future work: further develop DSE algorithms, enineer scalable implementations of those algorithms, develop automated support for DSE client applications, and study the cost and effectiveness of DSE in software maintenace tasks. 

# To the best of your understanding, what is proposed in this paper? The answer to this question should contain as much detail as possible, and should be a few paragraphs long, most likely.
 - The paper in whole offers a basis to improve modern forms of testing and debugging. Current efforts rely on source code differencing and version history matching, but these are inefficient in time, money, and energy because they highlight negligible differences such as syntax and formatting. Differential symbolic execution, the approach offered by the research paper, promotes a new way of testing: debugging based on program and methodological behavior rather than source code comparison.
 -  While there are multitidues of benefits for Differential Symbolic Execution, current technologies aren't built to support and track the analysis of its results. To accomodate this limitation, the team in the paper even adapted a toolset from a popular framework (Java PathFindder) to support mixed symbolic and concrete execution of integer and real data types. Based on the testing done in this new framework, they concluded that the CVC3 inputs encodde completeness, equivalence, and inddividual checks requried to calculate partition-effects deltas (the goals of DSE).
 - Finally, despite the small sample size of experiments possible to check with DSE (small mathematical computations, nothing large of scale), the results are promising. Out of 95 methods examined with current tools, 68 were able to be analyzed using DSE with full support. This was even a conservative assessment and proper procedures of analysis would have supported the conclusion even more. 

# What are the key concepts/terms/ideas that are blocking your more complete understanding of this paper? These should be the things you highlighted as confusions that you feel are most important for you to understand in order to understand this paper.
 - Pure mathematical and boolean proofs
  - Have only taken CS40, so revisiting these complex proofs and symbols is intimidating
- Scope of the project
  - Never had much problem with source code differencing, so it is hard to grasp the value of this energy
- Incomplete vs Complete symbolic summaries
- Equivalences and Deltas
- Refactoring assitance

# Pass 2
----
## Part 2.1
- Revisiting 5.2
   - Difficult topics: Functional Equivalence
   - Symbolic Execution
   - Abstract summaries
- The difficult aspects were addressed in a share excel file with my research group:
   -  Difficult Terms Dictionary: https://docs.google.com/spreadsheets/d/1vSvVDRM01zhh9HELbt__LugGeyf2Qdg_bZXGSx98GXw/edit?usp=sharing


## Part 2.2
What is your takeaway message from this paper?
What is the motivation for this work (both people and technical problem), and its distillation into a research question? Why doesn't the problem have a trivial solution? What are the previous solutions and why are they inadequate?
What is the proposed solution? Why is it believed it will work? How does it represent an improvement? How is the solution achieved?
What is the author's evaluation of the solution? What logic, argument, evidence, artifacts (e.g., a proof-of-concept system), or experiments are presented in support of the idea?
What is your analysis of the identified problem, idea and evaluation? Is this a good idea? What flaws do you perceive in the work? What are the most interesting or controversial ideas? For work that has practical implications, ask whether this will work, who would want it, what it will take to give it to them, and when it might become a reality?
What are the paper's contributions (author's and your opinion)? Ideas, methods, software, experimental results, experimental techniques...?
What are the future directions for this research (author's and hours, perhaps driven by shortcomings or other critiques)?
What questions are you left with? What questions would you like to raise in an open discussion of the work (review interesting and controversial points above)? What do you find difficult to understand? List as many as you can.
