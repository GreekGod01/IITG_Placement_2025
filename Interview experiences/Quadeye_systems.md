

---

# Interview Experience – Quadeye

## Round 1 ( Technical )

This happened way before placements like 2nd week of October

**Duration :** 40 mins

### 1) First one aptitute question :-

Given a 2^n x 2^n grid and L shaped tiles , provide proof and construction of best possible fit ie leaving as few cells untiled

**Answer ->**
1 will always remain empty 4^n not divisible by 3
can create grid with only one remaining
Induction

```
1) Base case -> single gird
2) Assuming induction hypothesis , break the grid into 4 parts , fill all parts with 1 missing and put the L shaped tile to get perfect 3/4 of the grid .
   Now put the smaller set in the top right to get 1 missing again
```

### 2)

Big endian and little endian ( how will the 2 byte number ABCD be stored ? )

### 3)

class B inherits class A privately and class c inherits class B publicly .
which members of A visible in c ?

### 4)

How can you determine size of L1 , L2 and L3 cache ?

### 5)

what is multicast in networks and how is it accomplished ?
is it server driven ?
what role does client play in it ?

### 6)

How are signals ( like kill() or ctrl + c) handled in cpp ?

---

## Round 2 ( Technical )

**Duration :** 70 mins

This happened after placements and was the longest one.
Interviewer was friendly and tried to cover a variety of topics.
First asked about intern experience and was interested in the business impact of my work

### 1) DSA question 1

Given an array with integers( positive , negative or zero ) and a target ,
you need to find maximum number of disjoint subarrays such that sum of each is equal to target
( not necessary that each element in original array must belong to a subarray )

### 2) DSA question 2

Given an initial array of zeroes and a target array of positive integers ,
you are allowed to perform an operation to choose a subarray and increment it by 1.
Find minimum number of operations to reach the target array.
( Had seen this previously on leetcode medium )

### 3)

Find if a number is a power of 2 in O(1).
(standard problem using bitwise operations)

### 4)

Find the kth rank element in O(n).
Provided the algoritm similar to the quick sort partitioning.
He was somewhat satisfied but asked a follow up for continuous stream of numbers
and hinted the use of heap.
Couldn't really understand the problem properly .

### 5)

Asked to write pseudocode of heap.
Explained the heapify operation and wrote the pseudocode for it.
He Was satisfied.

### 6)

Started with HPC.
Asked if I knew the 5 stage pipeline and asked about stalling.

### 7)

Asked about cycles wasted in case of branch misprediction.
I didn't know but started deriving and thinking out loud so even though I said 2 cycles instead of 3,
he complemented my thinking.

### 8)

Asked about scenarios in which there can be unsolvable hazards and their stallings.
Explained load and use hazard and its stall of 1 cycle.

### 9)

Started with OOPS - asked about constexpr ,
how to change the value of a const int ( using reinterpret cast )

---

## Round 3 ( Technical )

**Duration :** 60 mins

Asked to open code editor and implement a class of string with Small string optimization.
Spent the next hour impementing it but was a little rusty so kept making small mistakes.
It couldn't compile in time for the testcases but was mostly correct inpsite of few syntax mistakes.

---

## Round 4 ( Technical & Onsite )

**Duration :** 60 mins

Again interviewer was very friendly.

### 1)

First asked that if you know the pointer to a node in a Linked List then what changes to make
so that when the LL is traversed from start then the data in that particular node is skipped .

### 2)

How to implement LRU cache in software.
(Just the idea and use of data structures)

### 3)

Asked a very interesting puzzle.
You a given a cylindrical container with a random shaped nozzle on top with some water in it.
The entire height of the container ( including the nozzle is 12 m).
When in upright position , water extends to height 6 m
and when we invert the cylinder, water extends to height 8m
Find ratio of volume of water and container.

![Quadeye Interview](../../images/question.png)

### 4)

Asked an abstract puzzle where a man had a ruler , some length of rope , scissors and some hooks.
Had to use these to get down from some height.
Basically the catch was to tie the rope into a loop so it can be reused after descending a certain height.

### 5) DSA question

N people N tasks, NxN cost matrix for each person task pair .
Need to find minimum cost to finish all tasks.
( Was a little rattled so went on with a greedy apprach but couldnt prove the termination.
Finally had the sense to ask the contraints and when got to know N is small
then expalined the bit dp approach in detail )

Asked some other questions which I dont remember

---

## Round 5 ( Technical & Onsite )

**Duration :** 40 mins

Was a very scary guy and wasn't giving even the slighest affirmation or response after each question.

### 1)

As soon as he entered the room he asked what is segmentation fault and why does it occur.

### 2)

Given an Array of positive integers , find the following

```
A) F( subbarray ) = sum of subarray
   Find sum of F of all subarrays ( Quickly did it )

B) F( subbarray ) = product of subarray
   Find sum of F of all subarrays ( Struggled for 3-4 mins with hit and trial )

C) F( subbarray ) = xor of subarray
   Find sum of F of all subarrays
```

Broke down on this one.
Struggled for a good 10 -15 mins.
Even explained a couple of wrong answers somehow mistaking distributivity of xor operation over addition.
Was just about to give up when finally tried a combinatorial approach which worked but the damage was done

### 3)

Asked a simple brainstellar puzzle about the Cantor Pairing function.
He was unhappy when he got to know I already knew it.

### 4)

What is a shallow and a deep copy ?
Asked to make deep copy of a LL with some data.
Now the LL also had random pointers to some node in the same LL.
Asked to make a deep copy of this , maintaining the structure.
Did this with some additional memory.
Now he asked to not use any auxiliary memory.
Couldn't answer it satisfactorily then but in retrospect could have used memory of the recursion
and implemented a sort of dfs.

### 5)

Showed a piece of code and was asked its TC.
Was a simple code with complexity about O( N log( log (N)))

---

## Round 6 ( Partner & Onsite )

Very friendly and senior guy.
Talked in general about intern experience including the company and project,
about HFT industry , work and culture at Quadeye.

---

## Round 7 ( HR & Onsite )

Typical HR round.
She spent a lot of time explaining the benefits provided by the company.

---

## Verdict

**IUKUK**

---

## General Tips for a candidate

If you are preparing for this company I assume you satisfy the required branch and cgpa.
They do test general IQ through puzzles ( mostly Brainstellar type) and CP problems
so being proficient in these help but the level required is really not hard.

As for knowledge based problems, if you prepare even a week properly for systems
then you can easily solve most of these questions.

Favourite topics include
HPC( particularly 5 stage pipeline and stalling) ,
cache ,
basic and advanced OOPS involving copy elision , runtime polymorphism ,
move semantics , basic metaprogrmaming etc.

---


