# Lecture 05

## Design/Code by Contract

* 1947 - Alan Turing discusses the use of assert statements in algorithms
* 1967 - used in formal verification
* 1972 - used for finding faults during execution - based on preprocessors
* 1975 - Assertions introduced as part of programming languages themselves

### Assertions

* Bertrand Meyer includes assertions as part of Eiffel
* C and Java have very limited assertion capabilities
* More sophisticated tools available for Java
* JML adds quantification notation for Java - for all/there exists
* forall i, (0 <= i < N), A[i] <= A[i + 1]
* t.e. i, (0 <= i < N), A[i] > A[i + 1]
* Often want to reference original value Pre(x) or some such thing
* Sometimes, this is available only on a postcondition
* Local assertion - checked at definition site
* Global assertion - defined over a specific scope
* Example of global: GLOBAL ASSERT X > 10 find any use of x in scope and determine
* Loop assertion (invariant) - checked at each iteration at a designated point
* Pre/Post Conditions - checked at start and end of function/method
* Class assertion - checked at return of each method in class (class invariant)

## An assertion mechanism

* High level constructs for assertion expression
* Predefined responses at runtime if the assertion fails
* Automatic translation of logical expressions to executable statements
* Responses: when assertion is violated, issue error, report and terminate
* 3 level: Failure, warning, and info
* Assertion checking is generally suppressed in production

## Assertions vs Exceptions

* Assertion violation -> fault or error, predefined response
* Exception violation -> possibly recoverable unusual case, programmatic response

## Microsoft Assertion Study

* Hypothesis: inverse relationship between fault and assertion density
* On average, 14.5% of faults were detected by assertions in component A, 6.5% in component B
