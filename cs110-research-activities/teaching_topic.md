## Teaching Topic: Week 3 Pre-Class Assignment

Topic: Differential Symbolic Execution with an emphasis on Logical Equivalence

Why it is important: The basis for our reseach experiments will deal with differential symbolic execution. Everything from multiple paths, symbolic assignments, to general terminology will be crucial in advancing our research projects and exploring other research papers dealing.

---
### What is symbolic execution?
**Symbolic Execution** is the means of analyzing a program to determine the flow of inputs during the execution of a program.
- Rather than using the actual values of inputs (parameters, global variables, local variables), an interpreter assumes symbolic values for the inputs and executes as such.
- When the program is done running, the interpreter describes the program execution in terms of expressions + the symbols for expressions and variables. 
  - Whenever a conditional statement is reached, the interpreter also establishes constraints that consider the possible outcomes of each conditional branch and determines whether such outcomes are valid / invalid. 

*EXAMPLE*
`taken from wikipedia, read more: https://en.wikipedia.org/wiki/Symbolic_execution`
<img width="530" alt="image" src="https://user-images.githubusercontent.com/61306390/195430755-dd1a3eac-03ed-4aa7-8f48-dac30eb6c7b3.png">

Steps an interpreter takes:
- The interpreter takes a symbolic value (say A) and assigns it to y
- Goes down each line of code and performs it expectedly (z = A * 2)
- When a condition statement is reached (z==12), the interpreter "forks" two paths and makes a copy of the program state at that branch
- In this conditional, two paths are created: A * 2 == 12 and A * 2 != 12
  - The constaint for a program executing the fail() statement is A == 6
  - The constraint for a program executing the printf("OK") statement is A != 6
- The interpreter then returns the constraints and the possible branches that could have been taken during the program

### What is Differential Symbolic Execution
- From symbolic execution, we found that an interpreter can read through a program and return the possible path constaints / branches for program inputs. 
- What if we had a way to compare all of these constraints and branches?

Using the order of path constaints, the state of the program it is in, and it's current nested position, we can compare two functionally similar yet syntacitcally different pieces of code more efficiently. 
- For sections of code where the path constraints do not align, we assign DELTAS
- For sections of code where the path constraints align, we assign EQUIVALENCES

When symbolic execution is ran on these two blocks of code:
take note that these programs look vastly different in formatting and syntax.
<img width="395" alt="image" src="https://user-images.githubusercontent.com/61306390/195433311-7c570950-d7a4-40b7-8fb6-bedc6af51968.png">

PROGRAM 1:
The constaint for the program to return "old" is !(currentTime - t >= 100)
The constraint for the program to return 0 is (currentTime-t >= 100) 

PROGRAM 2:
The constraint for the program to return old is (currentTime - t) - represented as elapsed - is elapsed < 100
The constraint for the program to return 0 is currentTime-t >= 100 

The symbolic representations of the two programs are identical and the path constraints for the input, output effects are also similar. Thus, DSE would not flag any DELTAS, determine EQUIVALENCES for the program and would not raise any erros. 

