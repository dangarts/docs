# Computer Science Fundamentals

## Table of contents

Algorithms
- Time Complexity Basics


---

### Time Complexity Basics

***Time complexity*** is a metric used to describe the efficiency of an algorithm. It is express as a function that estimates the time it takes to execute a program.  This is determined by calculating how quickly the time to run the program grows relative to the amount of input we feed into the program.  The calculation is not measured in time, but instead as a function of the variable `n`, where `n` is the input size, and `f(n)` is the rate the algorithm grows as the input size grows.

***Runtime*** can refer to the physical time duration of an algorithm, but is often used synonymously with time complexity.

***Big O Notation*** Simplified analysis of an algorithm's efficiency
1. Big O gives us the complexity in terms of the input size, N
2. Machine-independent
3. examine basic computer steps
4. Can be used to measure TIME and SPACE

- Types of measurements: Big O can examine the 
   - **worst-case** 
   - best-case
   - average-case

- General rules
1. Ignore constants
   E.g. 5n -> O(n)
2. Certain terms 'dominate' others
   E.G. O(1) < O(logn) < O(n) < O(nlogn) < O(n^2) < O(2^n) < O(n!)

![alt text](https://cdn-images-1.medium.com/max/900/1*FKql5rhPdskhNAFV2D0RUQ.jpeg "Big O Chart")

