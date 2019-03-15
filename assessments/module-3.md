**1. What is an advantage and a disadvantage of using a linked list over an array?** .25/.5

PROS:
   - Each node within a linked list data structure is independent in memory.
   - The size is dynamic
   - An operating system may use any available memory location to store it
   - Due to the node memory's independence, link lists can be very large when compared to an array data strucutures.
   - Overflow never occurs unless memory is full
   - Insertion and deletions are easier when compared to arrays

CONS:
   - Linked lists can be inefficient to access an element as each node may exist anywhere in physical memory
   - Elements must be access in order as it does not hold an index like an array data structure
   - Access to data elements must be traversed from the head node; this leads to longer retrieval time.
   - Require more memory for storage



**2. On what kinds of data sets would you use binary search? Why?** 0/0.5

Binary search uses a sorted array dataset by a 'divide and conquer' approach for finding a value.  A sorted array consists of values arranged from low[0] to high.  Binary search compares the target value to the middle element of the array.  If the target value is lower then the midpoint, we can discard the upper half and vice versa.  The half in which the target cannot lie is eliminated and the search continues on the remaining half.  A new mid point is established on the new but smaller array and the iteration for the search starts again.  The process continues until the target value is found.


**3. If an algorithm has a logarithmic growth rate, what does that mean?** 0/0.5

An algorithm which halves the dataset with each iteration. The runtime grows by one unit every time we double the input. E.g. Binary Search


**4. What is a relational database?** 0.5/0.5

Relational database is based on the relational model that contains columns and rows of data.  Each row of data is a conceptual unit and the collection of these comceptual units in a table help make up a relational database.


**5. DataStructure** 1/1

> You are a programmer and in charge of implementing the undo function in a word processor.  What data structure would best suit the situation and why?
> a. tree / b. array / c. queue / d. stack

Undo function in a word processor is an operation that allows the last action to be reversed.  A stack LIFO is the data structure that needs to be implemented.


**6. TimeComplexity** 0/1

```
//What is the time complexity of the following code?
FUNCTION foo(array){
    SET total to zero
    FOR each element in array
       FOR each element in array
          INCREMENT total
       ENDFOR
    ENDFOR
   RETURN total
}
```


Quadratic.  Double loop

**7. BinarySearchTree** 0/1
>Given a Binary Tree, convert it to a Binary Search Tree.  The conversion must be done in a way that keeps the original structure of the Binary Tree.  You may not change how the tree is shaped.  Instead, you must move the five values of the tree (10, 27, 14, 23, 5) to there correct locations.  Verbally explain which values would be placed where in the tree (i.e x would take of y at the root because...)

```
      10
     /  \
   27    14
  /        \
23          5

      14
     /  \
   10    23
  /        \
5           27
```

**8. Which kind of join (left, right, inner) would result in the following data set from the account and transaction tables?** 1/1

**Results**

first_name | last_name | trans_id
-----------|-----------|----------
charles    | Reason    | 00055
Carl       | Guass     | 00077
Carl       | Guass     | 00122
Katherine  | Johnson   | (null)
Bernhard   | Riemann   | 00455


**Account**

account_id | first_name | last_name
-----------|------------|----------
00001      | carl       | guass
00002      | charles    | reason
00003      | bernhard   | riemann
00004      | katherine  | johnson

**Transaction**

trans_id | account_id | cost    | date
---------|------------|---------|------------
00122    | 00001      | $127.00 | 02-21-2017
00077    | 00001      | $567.00 | 04-19-2017
00455    | 00003      | $147.00 | 08-10-2017
00055    | 00002      | $780.00 | 01-18-2017


LEFT Join.  The reason is a inner join displays data if data points are included in both tables.  Considering the null value showing up in the trans_id column, a left join displays all account values and transactions.  Null if any transactions are unavailable.


**9. Given the database schema below for a school:** 1/1.5

```
TotalAvailableCourses(CourseID , CourseName, ProfessorID)
Professors(ProfessorID, ProfessorName)
Students(StudentID, StudentName)
StudentCourses(CourseID, StudentID)
```
Implement a query to get a list of all ProfessorID's that teach StudentCourses and the StudentCourses they teach. Note that TotalAvailableCourses and StudentCourses are different.

```
   select Professors.ProfessorID TotalAvailableCourses.CourseName
   from TotalAvailableCourses
   join Professors on TotalAvailableCourses.Professor.id = Professors.ProfessorsID
   join StudentCourses on TotalAvailableCourses.CourseID = StudentCourses.CourseID;
```

**10. Given an array of unsorted integers, write a function to sort them in order from smallest to largest. You may write the function in any language of your choice. You may not use any built-in sort functions.** 0.75/1

```
//Example:
Input: [1,7,5,6,8,9,9,100,24,35,10]
Output: [1,5,6,7,8,9,9,10,24,35,100]**
```

ANSWER ON CODEPEN: https://codepen.io/dangarts/pen/VRWvyR


**11. Write a binary search to search a sorted array for a given element.** 0/1.5
iteration and recursive


