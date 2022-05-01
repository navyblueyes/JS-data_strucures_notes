# Data Structures for Coding Interviews in JavaScript

### Introduction to Arrays

#### Arrays
- `push()` function
    - Basic
        - complexity of the `push()` operation will be O(1)
            - only have to update the `length` of the array and add new element
    - ![](img/1.01.001.jpg)
- `pop()` function
    - Basic
        - complexity of the `pop()` operation will be O(1)
            - only have to update the `length` of the array and remove one element
    - ![](img/1.01.002.jpg)
- `shift()` function
    - Basic
        - complexity of the `shift()` operation will be O(n) 
            - have to ...
                - remove the element at index 0
                - shift all the elements to the left, 
                - and update length of an array.
    - ![](img/1.01.003.jpg)
- `unshift(value)`
    - Basic
        - complexity of the `unshift()` operation will be O(n) 
            - have to 
                - update the length of an array
                - shift all the elements to the right
                - add the new element at index 0.
    - ![](img/1.01.004.jpg)
- `delete` keyword
    - Basic
        - Elements of an array can be deleted using `delete`
            - However
                - `delete` leaves undefined holes in the array
                    - aka... `undefined`
            - Better to use the shift() or pop() method.
    - Complexity
        - complexity of the `delete()` function will be O(n)
            - have to ...
                - remove the first element
                - move all the following elements to the left.
    - ![](img/1.01.005.jpg)
- `reverse()` function
    - Basic
        - complexity of the reverse() function will be O(n) since we have to...
            -  traverse all the elements of an array.
    - ![](img/1.01.006.jpg)
- `splice()` function
    - Basic
        - used to add or remove elements.
        - first parameter is the **index number**, where the new elements should be spliced in
            - index number
            - where the new elements should be spliced in
        - second parameter is the **number of elements** that should be removed
            - put `0` if you don’t want to remove anything
        - complexity
            - O(n)
                - worst-case, we have to shift n−1 elements.
    - ![](img/1.01.007.jpg)
- `slice()` function
    - Basic
        - used to slice out a piece of an array into a new array.3
        - first parameter --> index number
            - start of the slicing takes place
        - second parameter --> index number
            - up to which the array should be sliced out
            - the new array excludes this index number
                - if you want the very end of the array...
                    - leave second parameter empty
    - complexity of `slice()` function is O(n)
        - to returns a new array,
            - needs to run from the start to the end
        - worst-case
            - need to make a copy of all the elements present in the array
    - ![](img/1.01.008.jpg)
- `filter()` function
    - Basic
        - used to create a new array based on output of a function
        - filters out elements that do not pass the function
    - ![](img/1.03.00.jpg)
- `concat()` function
    - Basic
        - concatenate any number of arrays you want by..
            - specifying all of them as parameters to `concat()` function.
    - complexity
        -  O(m+n)
            - m is the size of the first array
            - n is the size of the second array
        - need to copy elemebts of both arrays **one by one** into a new array
    - ![](img/1.01.009.jpg)
- `for...of` statement 
    - Basic
        - conditional statement for looping through an array
    - ![](img/1.01.010.jpg)

#### var vs. let vs. const
- `const` Keyword
    - `const` is block-scoped
        - variable declared with `const` cannot be redeclared 
    - ![](img/1.02.001.jpg)
- var Keyword
    - function-scoped 
        - if declared anywhere else besides a function, 
            - will exist in the global scope.
        - ![](img/1.02.002.jpg)
- let Keyword 
    - block-scoped.
        - cannot be redeclared within the block
        - cannot be accessed outside the block
    - ![](img/1.02.003.jpg)
        - error because we initialized the `num` variable in the if-statement block
        - As it has been declared using `let`, 
            - we cannot access it outside the if block
    - ![](img/1.02.004.jpg)
        - works fine if... 
            - we use var as they are function-scoped ... and 
            - can be accessed throughout the function.

#### Challenge 1: Remove Even Integers From an Array
- Problem
    - Problem Statement
        - Implement a function `removeEven(arr)`
            - takes an array arr in its input
            - removes all the even elements from a given array.
    - Input
        - array with random integers.
    - Output
        - array with only odd integers
    - Sample Input

        ```[1,2,4,5,10,6,3]```
    - Sample Output 
        
        ```[1,5,3]```
    - Picture
        - ![](img/1.03.005.jpg)
- Coding Exercise 
    - ![](img/1.03.006.jpg)

#### Challenge 2: Merge Two Sorted Arrays
- Problem
    - Problem Statement
        - Implement a function `removeEven(arr)`
            - takes an array arr in its input
            - removes all the even elements from a given array.
    - Input
        - array with random integers.
    - Output
        - array with only odd integers
    - Sample Input

        ```[1,2,4,5,10,6,3]```
    - Sample Output 
        
        ```[1,5,3]```
    - Picture
        - ![](img/1.03.005.jpg)
- Coding Exercise 
    - ![](img/1.03.006.jpg)
#### Solution Review: Merge Two Sorted Arrays
#### Challenge 3: Find Two Numbers that Add up to "value"
#### Solution Review: Find Two Numbers that Add up to "value"
#### Challenge 4: Array of Products of All Elements
#### Solution Review: Array of Products of All Elements
#### Challenge 5: Find Minimum Value in Array
#### Solution Review: Find Minimum Value in Array
#### Challenge 6: Find First Unique Integer in an Array
#### Solution Review: First First Unique Integer in an Array
#### Challenge 7: Find Second Maximum Value in an Array
#### Solution Review: Find Second Maximum Value in an Array
#### Challenge 8: Right Rotate an Array by n
#### Solution Review: Right Rotate an Array by n
#### Challenge 9: Rearrange Positive & Negative Values
#### Solution Review: Rearrange Positive & Negative Values
#### Challenge 10: Rearrange Sorted Array in Max/Min Form
#### Solution Review: Rearrange Sorted Array in Max/Min Form
#### Challenge 11: Maximum Sum Subarray
#### Solution Review: Maximum Sum Subarray
#### Arrays Quiz: Test Your Understanding of Arrays

### Introduction to Linked Lists
### Introduction to Stack/Queues
### Introduction to Graphs
### Introduction to Trees
### Trie
### Introduction to Heap
### Introduction to Hashing
### Summary of Data Structures
