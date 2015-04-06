# Lecture 09

## Testing Review

### Testing Categories

* Two major categories - static and dynamic analysis
* Testing falls under dynamic analysis
* Testing takes a very sparse sampling of the input space generally
* Criteria determine how to sample test cases
* Types: Random, Coverage Based { control flow, data-flow, dependencies },
Fault-based { mutation, fault constraints }

### Manual Validation

* Code reviews, walkthrough, cleanroom
* Basic concepts: infeasible paths, coincidental correctness
* Imprecision: tend to over approximate real system behavior
* Sometimes, behavior is under approximated - ignoring branches/loops
* Cost must be considered - (test case selection/execution, oracle, test set eval)
* Test oracle - metamorphic testing can be used as a test oracle (vary something and
look for a corresponding change in output)

### Experimental Evaluation

* Consider subsumption, but also want to get there with smallest test suite possible

### Assertions vs ...

* ...Exceptions - describe expected but infrequent conditions - assertions say what
is always true. Exceptions complect control flow and error handling
* ...Unit Tests - unit testing usually concerned with pre and post values, rather than
intermediate states

### Code Coverage

* Evaluates coverage of functional test cases - shows what aspects of the program
have not been exercised
* Provides a (false) sense of accomplishment
* No operational profile
* Coverage does not provide guarantees that code is fault-free

## Symbolic Evaluation/Execution

* Based on "global behavior" - typical of a static analysis tool
* Creates a functional representation of a path of an executable component
* Symbolic names represent the input values
* The path value PV of a variable for a path describes the value of that var in symbolic names
* An interpreted branch condition is represented as an inequality or equality condition
* Can provide feasible paths through a program without executing the program
* Can also provide fault detection by determining where errors are possible
* Unlike testing, symbolic execution is not dependent on input data values. Rather,
it is dependent on the path
