Closed Interval Tree
===================
Software Engineering, 2nd year, Algorithm Analysis, University of Iceland 2014

Tree for closed intervals [a, b], that is each node has one interval written in Java

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



## GRADE
Grade 60% for the code and 40% for test client. 

Grade: 9.5 / 10.0
