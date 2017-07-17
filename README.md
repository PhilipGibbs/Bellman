# Bellman
The goal is develop and algorithm that solves Richard Bellman's Lost in a Forest problem for convex polygons 

In 1956 Richard Bellman posed the general problem of finding the most efficient route to escape from a forest given certain limited information. The specific case of interest to this project is to find the shape of the shortest path that guarantees escape from a forest given that the size and shape of the forest are known but the initial position and direction are not known.

Only three types of escape path solution are known. For many cases the optimal escape path is simply a straight ine of length equal to the diameter of the forest (The diameter of a shape is the largest distance between any two points in the shape.) This wroks for a citcle and any regular polygon with more than three sides. 

The second solution attributed to Zalgaller is the curve of greatest minimum width. This is the best escape path for a long thin rectangle and some other shapes. 

The third attributed to Besicovitch is a three segment zigzag which is the best escape pwth for a range of iscosceles triangles which include the equilateral triangle. This was proven only recently and with great difficulty.

No other paths are known to be solutions and even the full range of shapes for which these three types of curve are solutions is not known.

The only other conjectured solutions are those in my paper "Lost in an isosceles triangle which suggests a number of different solutions types for given base angles. These are based mainly on a monte carlo "random paths" algorithm that can be used to find approximate solutions for a given shape.  
