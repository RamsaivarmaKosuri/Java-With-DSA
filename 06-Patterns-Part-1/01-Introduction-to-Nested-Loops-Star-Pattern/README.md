# Introduction to Nested Loops (Star Pattern)

Before learning patterns, we first need to understand:

```text
Nested Loops
```

A:

```text
loop inside another loop
```

is called a:

```text
Nested Loop
```

Patterns are mainly built using:

```text
nested loops
```

---

## How We Solve Patterns?

In patterns, we mainly focus on:

### 1. Number of Lines (n)

Handled by:

```text
Outer Loop
```

The outer loop decides:

```text
how many rows or lines
```

the pattern should have.

---

### 2. Number of Times (i)

Handled by:

```text
Inner Loop
```

The inner loop decides:

```text
how many times something should print
```

in each line.

---

### 3. What to Print?

Example:

```text
*
1
A
#
```

This decides:

```text
what should appear in pattern
```

---

## Visual Understanding

For this pattern:

```text
*
**
***
****
```

### Outer Loop → Lines

```text
Line 1
Line 2
Line 3
Line 4
```

### Inner Loop → Stars

```text
Line 1 → 1 star
Line 2 → 2 stars
Line 3 → 3 stars
Line 4 → 4 stars
```

---

## Example Program

```java
public class JavaBasics {
    public static void main(String[] args) {

        for(int line = 1; line <= 4; line++) {

            for(int star = 1; star <= line; star++) {
                System.out.print("*");
            }

            System.out.println();
        }
    }
}
```

## Output

```text
*
**
***
****
```

---

## Code Understanding

### Outer Loop

```java
for(int line = 1; line <= 4; line++)
```

Controls:

```text
number of lines
```

This runs:

```text
4 times
```

---

### Inner Loop

```java
for(int star = 1; star <= line; star++)
```

Controls:

```text
number of stars
```

For every line:

```text
Line 1 → 1 star
Line 2 → 2 stars
Line 3 → 3 stars
Line 4 → 4 stars
```

---

## Dry Run (Visual Diagram)

☐ Line 1

```text
line = 1
star = 1

*
```

☐ Line 2

```text
line = 2
star = 1, 2

**
```

☐ Line 3

```text
line = 3
star = 1, 2, 3

***
```

☐ Line 4

```text
line = 4
star = 1, 2, 3, 4

****
```

---

## Your Notes

```java
// patterns(part 1)

// in patterns first we need to understand how it is or we solve them by using three types

// 1.lines(n) ----> outer loop ----> n times

// 2.number of times(i) ---> inner loop ---> i times

// 3.what to print ? ----> like example "*"

// print star pattern

public class JavaBasics {
    public static void main(String[] args) {

        for(int line = 1; line <= 4; line++) {

            for(int star = 1; star <= line; star++) {
                System.out.print("*");
            }

            System.out.println();
        }
    }
}
```

---

## Important Note

In patterns:

```text
Outer loop = number of lines
Inner loop = work inside each line
```

This concept is the:

```text
foundation of pattern problems
```
