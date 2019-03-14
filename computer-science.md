# Computer Science Fundamentals

## Table of contents

### CS Fundamentals
- CS Overview

### Data Structures
- Data Structure Overview
- Stack and Queues
- Link Lists
- Hash Tables
- Trees & Graphs

### Algorithms
- [Algorithm Overview](#algorithm-overview)
- [Time Complexity Basics](#time-complexity-basics)
- Recursion
- [Search Algorithms](#search-algorithms)
- Sorting Algorithms

### Databases and SQL
- DB and SQL Overview
- Relational Databases
- Fundamental SQL Commands
- Operators in SELECT statements
- JOIN statements

---

## CS Fundamentals
### CS Overview

Lorem ipsum

## Algorithms
### Algorithm Overview

**Algorithms** is a sequence of steps taken to complete a task that yields a result and finishes in a finite amount of time. 

### Time Complexity Basics
**Time complexity** is a metric used to describe the efficiency of an algorithm. It is express as a function that estimates the time it takes to execute a program.  This is determined by calculating how quickly the time to run the program grows relative to the amount of input we feed into the program.  The calculation is not measured in time, but instead as a function of the variable `n`, where `n` is the input size, and `f(n)` is the rate the algorithm grows as the input size grows.

**Runtime** can refer to the physical time duration of an algorithm, but is often used synonymously with time complexity.

**Big O Notation** is a simplified analysis of an algorithm's efficiency
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


#### Types of Growth Rate

- **CONSTANT Growth Rate O(1)** - An algorithm that will always execute in the same amount of time regardless of the size of the input data set
   - E.g. Statement (incrementing an integer)
- **LOGARITHMIC Growth Rate O(log n)** - An algorithm which halves the dataset with each iteration. The runtime grows by one unit every time we double the input.
   - E.g.   Common in binary search
- **LINEAR Growth Rate O(n)** - An algorithm whose performance will grow linearly and in direct proportion to the size of the input data set.
   - E.g. common in a single FOR loop (chech each element)
- **LOG-LINEAR Growth Rate O(n log n)** - An algorithm which halves the data each time for each of n times.
   - E.g.  Common in many sorts such as merge and heap sort (divide and conquer approach)
- **QUADRATIC Growth Rate O(n^2)** - An algorithm whose performance is directly proportional to the square of the size of the input data set. 
   - E.g. Common among nested for loops (checking pairs)
- **EXPONENTIAL Growth RateO(2^n)** - An algorithm whose growth doubles with each addition to the input data set.  
   - E.g. Exhaustive search / Common among recursive algorithms.

![alt text](https://cdn-images-1.medium.com/max/900/1*FKql5rhPdskhNAFV2D0RUQ.jpeg "Big O Chart")

---

### Search Algorithms

