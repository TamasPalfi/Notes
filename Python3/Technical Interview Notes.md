# Python3 Technical Interview Notes
Notes for **Python3 interview basics** will be located here.  It will primarily consist of basic topics that are commonly tested on **technical interviews** such as string methods, integer methods, common data structures, common algorithms, and so on.  Will eventually include more complex things as my preparation goes further.  I will be including anything that I feel the need to have a 2nd look on before any technical interview.  This will likely be my most extensive technical interview notes page as I am currently focused on improving my python skills with the **goal of obtaining a data science or ML job** out of college.  Most of these notes will be the results of practicing technical questions on [LeetCode](https://leetcode.com/).  Check out the website, it is a great resource to prep for an interview in any language.  *These notes are for public use but please cite me (@TamasPalfi) if showcase it elsewhere*. 

## Good Technical Interview Practices
- strongly consider stating and even writing out the brute force solution to a problem first if a better solution doesn't immediatly come to mind.  Important to solve the problem at hand first and then optimize.  However, this isn't always an option given the quick assessment times of many online tests.  Also, good choice to fall back to if cant find the best solution.

## General 
- *is* should be used for identity testing.  It is the same as id(a) == id(b).  *EX: Checking to see if a an element of a list matches an target object, you would use is.*
- *==* is used for equality comparison/testing.  It would be used to see if two objects contain the same data.  *EX: Checking to see if two strings are equal to one another*

## Strings



## Integers



## Dictionaries
- **BIG TIP TO NOTE:** Python's dictionaries are implemented as Hash Tables (and as such have same time/space complexities)!  See python documentation [here](https://docs.python.org/3/library/stdtypes.html#typesmapping)  Thus, I would recommend in interviews to use dictionaries as you are quite often more familiar with them due to it being one of the key data structures taught, but mention to the interviewer this distinction. 


## Hash Tables
- Hash tables are one of the fastest data structures for storing data that follows the *Key:Value* pairing approach.  They take up **O(N)** space complexity and their operation speeds are: **O(1)** for best-case of insert, fetch, and delete and **O(n)** for worst-case of insert, fetch, and delete.  The best case speeds occur when a good hash function is utilized and as such there is only one key:value pair filling in each bucket of the hash table.  The worst case occurs with a unoptimal hash function is utlized resulting in several data objects being placed in the same bucket.  This causes the operations' speed at that bucket to increase to O(n) due to the resulting search for the appropriate key have to look through an array or linked list rather than just a single key value.  Worst-case complexity can also occur when the hash table is full leading to the neccessary steps of rehashing each key:value pair in a larger hash table.  See [this](https://stackoverflow.com/questions/9214353/hash-table-runtime-complexity-insert-search-and-delete) for a more concrete answer to the complexity speeds and reasoning.
- Another option rather than Hash Tables is the commonly used **Red-Black Trees** data structure.  A hash table is often the preffered structure to use due to its advantage in average operation speed and easier implementation.  However, it is the case that although the RB Tree is harder to implement and has worst-average case complexity; it will self-balance (resize) and its operation speeds are O(logN) for insert, fetch and delete for both best and worst case with the same space complexity of O(N).  Thus, there are cases in which the RB Tree could perform better.  See [this](https://softwareengineering.stackexchange.com/questions/234793/why-does-python-use-hash-table-to-implement-dict-but-not-red-black-tree) for the full answer to this question.


## Functions
