# Reading Assignment 02

## Question 1

Inspections are a formal process of reviewing both design and code
that makes use of a diversified team. This team validates design
and code at agreed upon "checkpoints" throughout the creation
of the software. The team is anchored by the moderator, who handles
administrative tasks like scheduling meetings and provides an objective
voice during the inspection. The moderator is joined by the designer and
the coder, who designed and implemented the code respectively. These three
are joined by the tester, who was responsible for writing and running
test cases on the code being inspected. The inspection process begins with a preparation
period, where the designer outlines the general flow of the code. This period
is followed by the preparation and inspection phases, where the inspection team
attempts to understand the design and the code before hunting for errors. Once errors
are found, a rework period is used to correct those errors. Finally, the inspection
team follows up to to ensure that all issues have been corrected. Documentation should
be produced throughout this process to ensure that every step has been followed.

Fagan describes a good sized inspection team as being comprised of 4 people - one
for each of the roles described above.

Inspections are not to be confused with walk-throughs. Walk throughs are informal,
and vary widely between organizations. As a result, walk throughs lack the repeatability
of inspections. Additionally, they are not typically scheduled with same regularity of inspections.

## Question 2

The Hawthorne effect refers to an individual's proclivity to increase their productivity
in response to the knowledge that they are being observed by someone. This can have a positive
effect on software inspection, as designers and coders may feel incentivized to produce a higher
quality product if they know they are being observed.

## Question 3

Fagan unequivocally states that code inspection results must *never* be used in performance
appraisals. Inspections are first and foremost for the programmer's benefit, and must be treated
solely as a mechanism for identifying and removing errors from designs and code.

## Question 4

Similar to the literature review, Porter's experiment showed little difference in the effectiveness
of an inspection when team size was varied. As a result, Porter postulates that effort could be reduced
by decreasing the inspection team size to two without a measurable loss in quality. Regarding multiple sessions,
Porter found that using two session of two reviewers each was more effective, but obviously required more effort.
Practitioners will have to decide if the trade off is worth it. In the literature review, Tsai, et al found that
more sessions result in more defects found, but more work is required of the moderator to remove duplicate
defects between sessions.
