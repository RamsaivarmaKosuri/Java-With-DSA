# Space & Time Complexity (Reading Material)

> **Note**
>
> In some topics, you will hear terms such as:
>
> - Time Complexity
> - Space Complexity
> - Big O Notation
> - O(n)
> - O(log n)
>
> Don't worry if these terms seem confusing right now.
>
> The complete topic will be covered later as a separate chapter.
>
> For now, this reading material will help you understand the basic idea behind these concepts.

---

# Why Do We Need Complexity Analysis?

A single problem can often be solved in multiple ways.

For example:

```text
Problem
   ↓
Solution 1
Solution 2
Solution 3
```

All solutions may give the correct answer.

However:

- Some solutions are faster
- Some solutions are slower
- Some use more memory
- Some use less memory

Therefore, we need a way to compare different algorithms and choose the best one.

This is where:

```text
Time Complexity
```

and

```text
Space Complexity
```

become important.

---

# Scenario

Imagine you lend your pen to one of your 100 friends.

Now you want your pen back.

Your goal is:

```text
Find the friend who has your pen.
```

We will use this example to understand both Time Complexity and Space Complexity.

---

# Space Complexity

## What is Space Complexity?

Space Complexity represents:

```text
How much memory is required
for an algorithm to complete its task.
```

In simple words:

```text
How much space does the program need?
```

---

## Pen Example

Imagine you need different rooms to organize your search.

The more rooms you use,

the more space is required.

Similarly in programming:

```text
Variables
Arrays
Objects
Functions
Data Structures
```

all consume memory.

The total memory used contributes to:

```text
Space Complexity
```

---

# Time Complexity

## What is Time Complexity?

Time Complexity represents:

```text
How much work an algorithm performs
before completing its task.
```

In simple words:

```text
How many operations are executed?
```

---

## Important Note

Time Complexity is **NOT actual clock time**.

It does not mean:

```text
2 seconds
5 seconds
10 seconds
```

Instead, it measures:

```text
How many times statements execute.
```

---

## Pen Example

Imagine you are searching for your pen among 100 friends.

The method you choose determines the Time Complexity.

Different methods require different amounts of work.

---

# Types of Time Complexity

## 1. Best Case Time Complexity

The fastest possible scenario.

Example:

```text
You immediately remember
who has the pen.
```

Very little work is required.

---

## 2. Average Case Time Complexity

The average amount of work needed.

Example:

```text
Sometimes you find the pen early.
Sometimes you find it late.

Average effort is considered.
```

---

## 3. Amortized Time Complexity

Average performance over many repeated operations.

Example:

```text
You search for pens every day.

Instead of analyzing one search,
we analyze many searches together.
```

---

## 4. Worst Case Time Complexity

The maximum amount of work needed.

Example:

```text
The last friend has the pen.

You must ask everyone before finding it.
```

This is usually the most important complexity discussed in interviews.

---

# Big O Notation

Big O Notation is used to represent complexity.

Examples:

```text
O(1)
O(log n)
O(n)
O(n²)
```

Read them as:

```text
Big Oh of 1
Big Oh of log n
Big Oh of n
Big Oh of n squared
```

---

# Common Complexity Examples

## O(1) — Constant Time

### Pen Example

You remember exactly who has the pen.

```text
Go directly to that friend.
```

Only one operation is required.

### Visual

```text
Friend → Pen Found
```

Fastest possible complexity.

---

## O(log n) — Logarithmic Time

### Pen Example

Divide 100 friends into two groups.

Ask:

```text
Is the pen in Group A or Group B?
```

Choose the correct group.

Divide again.

Repeat until only one person remains.

### Visual

```text
100
 ↓
50
 ↓
25
 ↓
12
 ↓
6
 ↓
3
 ↓
1
```

Very efficient.

---

## O(n) — Linear Time

### Pen Example

Ask each friend one by one.

```text
Friend 1
Friend 2
Friend 3
...
Friend 100
```

Worst case:

```text
100 questions
```

---

## O(n²) — Quadratic Time

### Pen Example

Ask one friend:

```text
Do you have the pen?
```

Then ask:

```text
Do the other 99 friends have it?
```

Repeat the process for every friend.

### Visual

```text
100 × 100
```

Huge amount of work.

Very slow for large inputs.

---

# Complexity Comparison

| Complexity | Performance |
|------------|------------|
| O(1) | Best |
| O(log n) | Very Fast |
| O(n) | Good |
| O(n log n) | Efficient |
| O(n²) | Slow |
| O(n³) | Very Slow |

---

# Important Point

Many beginners think:

```text
Time Complexity = Time in Seconds
```

This is incorrect.

Complexity measures:

```text
Number of operations performed.
```

Not actual clock time.

Example:

```java
for(int i=0;i<n;i++){
    System.out.println(i);
}
```

Complexity:

```text
O(n)
```

because the statement executes:

```text
n times
```

---

# Why Don't We Consider Hardware?

Different computers have:

- Different Processors
- Different RAM
- Different Operating Systems

Therefore actual execution time varies.

To compare algorithms fairly:

```text
We ignore hardware differences.
```

and focus on:

```text
Number of operations performed.
```

---

# Summary

While analyzing an algorithm, we mainly focus on:

1. Time Complexity
2. Space Complexity

### Time Complexity

Measures:

```text
How much work an algorithm performs.
```

or

```text
How many operations execute.
```

---

### Space Complexity

Measures:

```text
How much memory is required.
```

---

A problem can have multiple solutions.

Our goal is to choose the solution that:

```text
Uses less time
Uses less memory
Produces the correct output
```

---

# Easy Note to Remember

Imagine you are searching for a pen.

```text
Time Complexity
=
How much effort you make to find it
```

```text
Space Complexity
=
How much extra space/resources you use while finding it
```

---

## Quick Revision Trick

```text
Time Complexity → Work Done

Space Complexity → Memory Used
```

---

## One-Line Memory Trick

```text
Time = Effort

Space = Memory
```

Whenever you get confused, remember this line and you'll recall the entire concept.

---

# Interview Questions

### 1. What is Time Complexity?

Time Complexity measures the number of operations performed by an algorithm.

---

### 2. What is Space Complexity?

Space Complexity measures the amount of memory used by an algorithm.

---

### 3. What is Big O Notation?

Big O Notation is a way to represent the efficiency of an algorithm.

Example:

```text
O(1)
O(log n)
O(n)
O(n²)
```

---

### 4. Which is faster: O(n) or O(n²)?

```text
O(n)
```

because it performs fewer operations as input size grows.

---

### 5. Does Time Complexity represent actual execution time?

No.

It represents:

```text
Number of operations performed
```

not actual seconds.

---

### 6. Why do we analyze Time and Space Complexity?

To compare algorithms and choose the most efficient solution.

---

### 7. Which complexity is considered best?

```text
O(1)
```

because it performs a constant number of operations.
