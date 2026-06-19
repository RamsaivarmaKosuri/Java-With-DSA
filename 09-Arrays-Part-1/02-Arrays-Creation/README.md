# Arrays Creation

Before using an array, we must create it.

Creating an array means:

```text
Reserving memory for multiple elements of the same data type.
```

Arrays support four basic operations:

1. Create
2. Input
3. Output
4. Update

In this topic, we will focus on the first operation:

```text
Array Creation
```

---

# Array Creation Syntax

```java
datatype arrayName[] = new datatype[size];
```

Example:

```java
int marks[] = new int[50];
```

Meaning:

```text
Create an integer array
named marks
with size 50.
```

---

# Breaking Down the Syntax

Example:

```java
int marks[] = new int[50];
```

| Part | Meaning |
|--------|----------|
| int | Data Type |
| marks | Array Name |
| [] | Indicates Array |
| new | Allocates Memory |
| int[50] | Creates 50 Integer Spaces |

---

# How Memory is Allocated

Example:

```java
int marks[] = new int[5];
```

Memory:

```text
Index

0    1    2    3    4
-----------------------
0 | 0 | 0 | 0 | 0
-----------------------
```

Notice:

```text
Java automatically stores default values.
```

For integer arrays:

```text
0
```

is stored initially.

---

# Default Values in Arrays

If values are not provided, Java automatically assigns default values.

| Data Type | Default Value |
|------------|--------------|
| int | 0 |
| float | 0.0 |
| double | 0.0 |
| long | 0 |
| short | 0 |
| byte | 0 |
| char | '\u0000' |
| boolean | false |
| String | null |

---

# Method 1 : Create Empty Array

```java
int marks[] = new int[50];
```

Output:

```text
Array of size 50 created.
```

Initially:

```text
0 0 0 0 0 ...
```

---

# Method 2 : Create and Initialize Together

```java
int numbers[] = {1,2,3};
```

Memory:

```text
Index

0   1   2
-----------
1 | 2 | 3
-----------
```

Java automatically determines:

```text
Size = 3
```

---

# Example

```java
int numbers[] = {1,2,3};
```

| Index | Value |
|---------|---------|
| 0 | 1 |
| 1 | 2 |
| 2 | 3 |

---

# Another Example

```java
int moreNumbers[] = {4,2,66};
```

Memory:

```text
Index

0   1   2
------------
4 | 2 | 66
------------
```

Size:

```text
3
```

---

# String Array Example

```java
String fruits[] = {"apple","mango","banana"};
```

Memory:

```text
Index

0         1         2
------------------------
apple | mango | banana
------------------------
```

Size:

```text
3
```

---

# Method 3 : Declare First, Create Later

```java
int marks[];

marks = new int[5];
```

This is also valid.

Here:

```java
int marks[];
```

declares the array.

Later:

```java
marks = new int[5];
```

allocates memory.

---

# Dry Run Example

Program:

```java
int numbers[] = {1,2,3};
```

### Step 1

Array created.

```text
Size = 3
```

---

### Step 2

Store values.

```text
Index 0 → 1
Index 1 → 2
Index 2 → 3
```

---

### Step 3

Final Memory

```text
Index

0   1   2
-----------
1 | 2 | 3
-----------
```

---

# Real-Life Analogy

Think of an apartment building.

```text
Flat Numbers

0
1
2
3
4
```

When the building is constructed:

```text
Rooms Exist
But Nobody Lives There Yet
```

Similarly:

```java
int marks[] = new int[5];
```

Memory exists.

Values can be stored later.

---

# Common Beginner Mistakes

## Mistake 1

```java
int marks[];

marks[0] = 95;
```

Problem:

```text
Memory was never allocated.
```

Correct:

```java
int marks[] = new int[5];

marks[0] = 95;
```

---

## Mistake 2

```java
int marks[5];
```

This is valid in C/C++.

But not in Java.

Correct:

```java
int marks[] = new int[5];
```

---

# Interview Notes

### Why do we use `new`?

Answer:

```text
The new keyword allocates memory for the array.
```

---

### Can array size be changed later?

Answer:

```text
No.
Arrays have a fixed size.
```

---

### What happens if values are not provided?

Answer:

```text
Java automatically stores default values.
```

---

# Key Observations

| Concept | Observation |
|-----------|-------------|
| Array Size | Fixed |
| Index Starts | 0 |
| Memory | Continuous |
| Same Data Type | Required |
| new Keyword | Allocates Memory |

---

# Easy Memory Trick

Remember:

```text
Create → Store → Access
```

Example:

```java
int marks[] = new int[5];
```

Create

↓

```java
marks[0] = 95;
```

Store

↓

```java
System.out.println(marks[0]);
```

Access

---

# Key Takeaways

- Arrays must be created before use.
- Arrays store elements of the same data type.
- The `new` keyword allocates memory.
- Arrays have fixed size.
- Java automatically assigns default values.
- Arrays can be created with or without initial values.
- Array indexing starts from 0.
