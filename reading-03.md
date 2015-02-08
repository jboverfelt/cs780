# Reading Assignment 03

## Question 1

A "subsumes" relationship between two coverage criteria means that satisfying
one criterion necessarily means satisfying the other criterion. More formally,
if criterion A subsumes criterion B, then the set of programs which satisfy A is a
superset of the set of programs which satisfy B. An example of a subsumes relationship
exists in the fact that branch coverage subsumes statement coverage. This is illustrated
nicely in Figure 2c in the paper. This figure presents a control flow graph for the
following pseudocode:

```
for i := e1 to e2 do
	S
end
```

If we set e1 = e2, then all nodes of the graph are visited, satisfying statement
coverage. However, two edges are not traversed, leaving branch coverage unsatisfied.
Thus, it is possible to satisfy statement coverage without also satisfying branch coverage.

## Question 2

A feasible version of a particular adequacy criterion is defined as an adequacy criterion
which can be satisfied by a finite test set. That is, the feasible version is, by definition,
finitely applicable. This notion is needed in order to practically apply the criteria focused on
in the paper, such as statement coverage, branch coverage, and path coverage. Since finding dead
code is undecidable and paths may be infinite, the classical definitions of these criteria are
not feasible. For example, while path coverage is not possible in the presence of loops,
one can use a subset of path coverage called simple path coverage. In simple path coverage,
paths are only considered if they visit each edge in the path at most one time. This avoids
potentially infinite cycles and makes a test set which meets this criteria finitely applicable.
