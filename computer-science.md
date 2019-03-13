# Computer Science Fundamentals

## Table of contents

Algorithms
- [Time Complexity Basics][Time Complexity Basics]
   - [Detail](https://github.com/dangarts/docs/blob/master/computer-science.md#types-of-growth-ratedetail)

---

## Time Complexity Basics

***Time complexity*** is a metric used to describe the efficiency of an algorithm. It is express as a function that estimates the time it takes to execute a program.  This is determined by calculating how quickly the time to run the program grows relative to the amount of input we feed into the program.  The calculation is not measured in time, but instead as a function of the variable `n`, where `n` is the input size, and `f(n)` is the rate the algorithm grows as the input size grows.

***Runtime*** can refer to the physical time duration of an algorithm, but is often used synonymously with time complexity.

***Big O Notation*** Simplified analysis of an algorithm's efficiency
1. Big O gives us the complexity in terms of the input size, N
2. Machine-independent
3. examine basic computer steps
4. Can be used to measure TIME and SPACE

Types of measurements: Big O can examine the 
   - **worst-case** 
   - best-case
   - average-case

General rules
1. Ignore(drop) constants
> 5n -> O(n)
2. Certain terms 'dominate' others
> most efficient -> least efficient
> O(1) < O(logn) < O(n) < O(nlogn) < O(n^2) < O(2^n) < O(n!)


### Types of Growth Rate(detail)

- **CONSTANT Growth Rate O(1)** - the runtime of the function does not change whether processing one piece of data or processing a million pieces of data
   - E.g. Statement (incrementing an integer)
- **LOGARITHMIC Growth Rate O(log n)** - the runtime grows by one unit every time we double the input.
   - E.g.   Common in binary search
- **LINEAR Growth Rate O(n)** - the runtime of the function and the amount of data it processes are directly proportional to each other.
   - E.g. common in a single FOR loop (chech each element)
- **LOG-LINEAR Growth Rate O(n log n)** - the runtime halves the data each time for each of `n` times.
   - E.g.  Common in many sorts such as merge and heap sort (divide and conquer approach)
- **QUADRATIC Growth Rate O(n^2)** - the runtime is directly proportional to the square of the size of the input data set. 
   - E.g. Common among nested for loops (checking pairs)
- **EXPONENTIAL Growth RateO(2^n)** - the runtime doubles with each addition to the input size.  
   - E.g. Exhaustive search / Common among recursive algorithms.

![alt text](https://cdn-images-1.medium.com/max/900/1*FKql5rhPdskhNAFV2D0RUQ.jpeg "Big O Chart")