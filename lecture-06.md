# Lecture 06

## Mutation Testing

### Random Testing

* Decide which are the legal inputs and generate test cases randomly over the program
input domain
* Can use as a benchmark to determine if a test criteria is better than random
* Drawbacks: need to have an oracle for each test case
* Tests the program uniformly - this may not match real usage

### Error Seeding

* Insert typical faults into the system
* Determine how many of those inserted faults are found by your test suite
* Assumption that finding the seeded faults means finding real faults is
dependent on the seeded faults being representative of real faults

### Mutation Testing

* Insert simple faults - resulting program(s) are called mutants
* Apply test suite to each program and check mutants "killed" (test case failed)
* Only one test needs to fail
* A large number of live mutants means that the test suite is inadequate.
* 100% mortality is not achievable - mutants can be semantically equivalent
* Determining if two programs semantically equivalent is NP-Hard

### Assumptions

* Competent Programmer Hypothesis - programmers write code that is reasonably close to the
desired program
* Coupling effect - detecting simple atomic faults will lead to
the detection of more complex faults

### Atomic Faults

* Constant replacement x := x + 5 becomes x := x + 6
* Scalar variable replacement - replace one variable with a variable of the same type
* Operator replacement
* Unary operator insertion
* Statement deletion

### Mutation System

* Uses initial execution to determine the oracle
* Creates mutants
* List seeded errors that resulted in live mutants
* User states interactively if the mutant is equivalent

### Drawbacks

* Very expensive - finding equivalent mutants is a manual process
* Killing all mutants is very hard - last 20% extremely difficult
* Inherent assumptions need more study

### Comparisons

* Mutation coverage subsumes branch coverage, but suite for mutation testing is much larger
