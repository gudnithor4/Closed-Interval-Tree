Closed Interval Tree
===================
Software Engineering, 2nd year, Analysis of Algorithms, University of Iceland 2014

Tree for closed intervals [a, b], each node has one interval.

Written in Java

Command line operations
------------------------
- ’+ a b’ push the closed interval [a, b] into the tree
- ’-’ a b remove the closed interval [a, b] from the tree
- ’?o a b’ prints out all intervals in the tree that intersect the given interval [a, b]
- ’?i a b’ prints out all intervals [c, d] in the tree that include [a, b] c <= a og b <= d.
- ’?p a’   print out all intervals in the tree that include the point a

Input Example:
- + 1 2
- ?o 2 3
- + 2 3
- + 0 4
- ?i 2 3
- - 2 3
- ?p 2
- ?p 5

Output Example:
- [1, 2]
- [0, 4] [2, 3]
- [0, 4] [1, 2]
- []

Test:
- $java Verkefni2 < s1.in | diff -w s1.out - | wc -l
- If this returns 0 there is no difference between the correct output and the trees output

