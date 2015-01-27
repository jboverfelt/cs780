# Lecture 02

# Formal Models

* Graphs are most common representation
* ASTs, call graphs, program dependence graphs

# Graphs

* G = (N, E) where N is the node set and E the edge set
* A path P through a graph G is a sequence of edges
* Cycle - a path whose start node and end node are the same
* In graphs that represent programs, loops are shown as cycles

# ASTs and Computation Tree

* Computation tree models all possible executions of a system
* Tree is theoretically bounded, but practically infinite
* Computation tree provides a theoretical upper bound
* Too large to create for anything interesting

# Control Flow Graph

* Represents flow of executable behavior
* Nodes, Edges, start node, terminal node
* Node -> executable instruction (statement, fragment, set of statements)
* Edge -> *potential* transfer of control depending on conditionals
* CFG over-estimates the executable behavior - it may display currently infeasible paths
* In general determining if paths are feasible or not is not possible (halting problem)
* Unreachable code is dead code, but not the other way around

# Call Graph

* G = (N, E, s)
* N is a set of invokable entities
* E represents potential invocation
* s = unique start node
