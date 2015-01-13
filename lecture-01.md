# Lecture 01

## Background

* A crisis is when we have not solved some fundamental challenges with area
* Crisis in SE is inability to deliver software that is in accordance with the specification
  and developed within estimated time and developed within estimated budget
* Costs can approach $1000 per LOC
* For every KLOC, 3-10 faults
* 1-1000 LOC/day
* Average 30 LOC/day
* F-4 fighter 8% of software control
* F-22 85% was provided by software - 1.7 million lines of code

## Questions

* What do we mean by quality?
* What is an error? Can errors be shown to be absent?
* How much testing? What to test?
* How can we better manage the SDLC?

## Stakeholders (and their stakes)

* Users -> { correctness, usability }
* Developers -> { "control" of software, maintainability, other internal qualities... }
* Testers -> { testability }
* Customers -> { within budget, visible/satisfactory progress and feedback }
* Investors -> { profit, dividends }
* Innocent Bystanders -> { does no harm, provides the needed service }

## Products

* Software quality is relative to stakeholder interests
* Product is "good" if it meets the needs of *all* stakeholders
* Software product is not a monolithic thing - quality means different things
* Air traffic control system - emphasis on safety
* Game - emphasis on speed/gameplay
* Competitive website - emphasis on usability
* Mars rover - correctness primary focus - maybe less so on security

## Correctness

* Only prove correctness through testing via exhaustive testing (infeasible)
* Need formal methods for proof of correctness

## Maintenance

* Corrective (bugs 20%)
* Adaptive (20%)
* Perfective (60%)
