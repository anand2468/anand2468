# Data Structures & Algorithm

# Introduction to DSA

+ `data structures` are used to represent the data in computer in a simpler way   
+ `algoriths` are step by stem process to solve the problem

>Data structure and algorithms help in understanding the nature of the problem at a deeper level and thereby a better understanding of the world.

## data structure
**data structure** is a mathematical or logical model of an organization of data. Data structure is a way to organise the data 
accessable to computer. the main purpose is to reduce the space and time complexities. an efficient data structure 
will use of minimal memory and makes use of less computaion time

types of data structures
+ arrays
+ strings
+ linked lists
+ stacks
+ queues
+ heap
+ graph
+ trees

## what is Algorithms?
Now, let’s switch to the other side of the coin and see what is meant by the term algorithm. Algorithms are well-defined sets of instructions designed that are used to solve problems or perform a task. To explain in simpler terms, it is a set of operations performed in a step-by-step manner to execute a task.


# kadane's algorithm
```
1) initilise
    max_so_far = min_inf
    max_ending_here = 0,

2) iterate over each element in array
    a) max_enging_here += a[i]
    b) if max_ending_here > max_so_far then
        max_so_far = max_ending_here
    c) if max_ending_here < 0 then
        max_ending_here = 0

3) return max_so_far
```
using dp
```
dp[i] = max(dp[i-1]+a[i] , a[i])
```

## *Dynamic Programming*
my fav & 1st algo
* It is used to solve optimal problems.
* The problems which have overlaping substructured pattern is solved using _dp_.
* There are two approaches in *dp*, `top-down-approach` and `bottom-up-approach`.

### Top Down Approach ⬇️ 
  it is also called as *momoization*. Generaly recurson is used in top down approach
### Bottom Up Approach ⬆️
  It is also called as *tabulation*. *Iteration* is used in this process
