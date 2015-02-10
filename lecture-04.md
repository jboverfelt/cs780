# Lecture 04

## Black/White Box Testing

### Why Black Box Testing?

* May not have access to the code
* Look at specified behavior rather than implemented behavior

### Why White Box Testing?

* Being able to see code reveals possible edge cases
* Better chance of discovering faults through systematic test case selection

## Coverage Criteria

* 1973: NASA reports that it only has 1/3 statement coverage
* Usually can get around 80%
* Not the greatest measure of reliability
* Branch coverage is better - catch implicit else and looping
* Condition (hidden path) coverage ensures all conditionals have been covered in compound conditionals
* Path coverage even better, but infeasible
* Coincidental correctness - executing a statement does not mean all faults will be revealed
