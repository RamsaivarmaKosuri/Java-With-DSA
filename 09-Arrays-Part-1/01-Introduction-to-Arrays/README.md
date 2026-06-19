# Introduction to Arrays

### Meaning

An Array is a collection of elements of the same data type stored in contiguous (continuous) memory locations.

Example:

```java
int marks[] = {90, 85, 95, 80, 75};
```

Here:

- All elements are of type `int`
- Elements are stored continuously in memory
- Each element is accessed using an index

---

## Memory Representation

```text
Index

0     1     2     3     4
---------------------------
90 | 85 | 95 | 80 | 75
---------------------------
```

Notice:

```text
All elements are stored one after another.
```

This is called:

```text
Contiguous Memory Allocation
```

---

## Why Arrays?

Without Arrays:

```java
int mark1 = 90;
int mark2 = 85;
int mark3 = 95;
int mark4 = 80;
int mark5 = 75;
```

With Arrays:

```java
int marks[] = {90,85,95,80,75};
```

Arrays make code:

- Cleaner
- Shorter
- Easier to manage

---

## Real-Life Analogy

Think of a train.

```text
[90] [85] [95] [80] [75]
```

Every compartment stores a value.

Similarly, array elements are stored together in memory.

---

## Key Points

| Property | Description |
|-----------|-------------|
| Data Type | Same Type |
| Memory | Continuous |
| Index Starts | 0 |
| Size | Fixed |

---

## Interview Definition

An Array is a collection of elements of the same data type stored in contiguous memory locations and accessed using indexes.

---

## Key Takeaways

- Arrays store multiple values.
- All elements must have the same data type.
- Elements are stored in continuous memory locations.
- Array indexing starts from 0.
- Arrays are one of the most important data structures in DSA.
