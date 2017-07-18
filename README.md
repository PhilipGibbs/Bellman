# Bellman
The goal is develop and algorithm that solves Richard Bellman's Lost in a Forest problem for convex polygons 

In 1956 Richard Bellman posed the general problem of finding the most efficient route to escape from a forest given certain limited information. The specific case of interest to this project is to find the shape of the shortest path that guarantees escape from a forest given that the size and shape of the forest are known but the initial position and direction are not known.

Only three types of escape path solution are known. For many cases the optimal escape path is simply a straight ine of length equal to the diameter of the forest (The diameter of a shape is the largest distance between any two points in the shape.) This wroks for a citcle and any regular polygon with more than three sides. 

The second solution attributed to Zalgaller is the curve of greatest minimum width. This is the best escape path for a long thin rectangle and some other shapes. 

The third attributed to Besicovitch is a three segment zigzag which is the best escape pwth for a range of iscosceles triangles which include the equilateral triangle. This was proven only recently and with great difficulty.

No other paths are known to be solutions and even the full range of shapes for which these three types of curve are solutions is not known.

The only other conjectured solutions are those in my paper "Lost in an isosceles triangle" which suggests a number of different solutions types for given base angles. These are based mainly on a monte carlo "random paths" algorithm that can be used to find approximate solutions for a given shape.  

Solutions to Bellman's problem have applications to Moser's worm problem because where a solution is known for a given shape that will set an upper bound using a similar shape as a worm cover.

The lack of progress beyond the three known solutions after sixty years has led to the problem being described as "unapproachable." In one article Scott Willaims listed it as one of seven problems whose solution would be worth "a million bucks." However, no actual prize money has been offered.

Aside from its interest as a problem in pure mathematics An efficient algorithmic solution to the problem could be of practical importance to robotics and search tasks

The problem is of interest for very general shapes including shapes that are disconnected or contain holes. For the purposes of simplicity this project will focus on convex polygons, but if this is solved it may be possible to generalise. Note that the convex case is sufficient for applications to the Moser worm problem.

Despite the pessimism about solutions I believe that it may be possible to resolve the problem using a combinatorical result. By analysing the nature of optimal escape paths I have shown that for a convex polygonal forest the escape path must take the form of a curve made piecewise of stright line and circular arc segments. To find the optimal path it should be sufficient to enumerate all the ways in which such a curve can touch the sides of the forest, and then find the geometric optimal for each case.

In this repository I will attempt to subdivide the problem into distinct subproblems which are iether combinatorial or geometric, solve the each subproblems and then implement to form the dolution.

If necessary I will make assumptions and will not be attempting to rigorously prove that the algorithm is correct. 

This goal is ambitious and it may not be possible to complete it.
