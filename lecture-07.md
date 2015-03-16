# Lecture 07

## Data Flow Coverage

### Control Flow and Data Dependence

* Most important: test paths that are likely to produce an error
* Control flow graph alone is not sufficient - need to add data dependence
* Need to look at places where variables are defined and used

### Data Flow Coverage Criteria

* All-Defs: Some definition clear subpath from each definition to some use
reached by that definition. Select a path that includes the definition of a variable
to one or all of its uses. Each definition reaches some use.
* All-Uses: Each definition to all its respective uses and each successor node of the use.
* All-C-Uses, Some-P-Uses - each definition needs to reach each of its computation uses
and some of its predicate uses
* All-Def-Use: Exercise every possible path from the definition to the use and each successor of each use
