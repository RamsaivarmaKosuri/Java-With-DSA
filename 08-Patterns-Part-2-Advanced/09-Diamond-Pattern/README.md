# Diamond Pattern

The Diamond Pattern is one of the most important star patterns in Java.

It combines:

- Nested Loops
- Spaces
- Stars
- Symmetry

The pattern looks like a diamond shape.

---

# Why Learn Diamond Pattern?

The Diamond Pattern helps in understanding:

- Pattern Symmetry
- Space Management
- Nested Loops
- Upper Half and Lower Half Logic

Many advanced interview patterns are based on Diamond Pattern concepts.

---

# Pattern Output

For:

```java
diamond(4);
```

Output:

```text
   *
  ***
 *****
*******
*******
 *****
  ***
   *
```

---

# Program

```java
public class JavaBasics{

    public static void diamond(int n){

        // First Half
        for(int i=1;i<=n;i++){

            // Spaces
            for(int j=1;j<=n-i;j++){
                System.out.print(" ");
            }

            // Stars
            for(int j=1;j<=(2*i)-1;j++){
                System.out.print("*");
            }

            System.out.println();
        }

        // Second Half
        for(int i=n;i>=1;i--){

            // Spaces
            for(int j=1;j<=n-i;j++){
                System.out.print(" ");
            }

            // Stars
            for(int j=1;j<=(2*i)-1;j++){
                System.out.print("*");
            }

            System.out.println();
        }
    }

    public static void main(String[] args) {
        diamond(4);
    }
}
```

---

# Understanding the Logic

The Diamond Pattern consists of:

```text
Upper Half
+
Lower Half
```

Visual:

```text
   *
  ***
 *****
*******
-------
*******
 *****
  ***
   *
```

The line is only for understanding and is not printed.

---

# Formula Used

## Spaces

```java
n - i
```

## Stars

```java
(2 * i) - 1
```

---

# Understanding the Star Formula

Observe:

```text
1
3
5
7
```

These are odd numbers.

The formula:

```java
(2 * i) - 1
```

produces:

| i | Stars |
|---|--------|
| 1 | 1 |
| 2 | 3 |
| 3 | 5 |
| 4 | 7 |

---

# First Half Dry Run

Input:

```java
diamond(4);
```

---

## Row 1

```text
i = 1
```

Spaces:

```text
4 - 1 = 3
```

Stars:

```text
(2 × 1) - 1 = 1
```

Output:

```text
   *
```

---

## Row 2

```text
i = 2
```

Spaces:

```text
4 - 2 = 2
```

Stars:

```text
(2 × 2) - 1 = 3
```

Output:

```text
  ***
```

---

## Row 3

```text
i = 3
```

Spaces:

```text
4 - 3 = 1
```

Stars:

```text
(2 × 3) - 1 = 5
```

Output:

```text
 *****
```

---

## Row 4

```text
i = 4
```

Spaces:

```text
4 - 4 = 0
```

Stars:

```text
(2 × 4) - 1 = 7
```

Output:

```text
*******
```

---

# First Half Summary Table

| Row (i) | Spaces | Stars | Output |
|----------|---------|---------|---------|
| 1 | 3 | 1 |    * |
| 2 | 2 | 3 |   *** |
| 3 | 1 | 5 |  ***** |
| 4 | 0 | 7 | ******* |

---

# Second Half Dry Run

The second half is simply the reverse of the first half.

---

## Row 4

Output:

```text
*******
```

---

## Row 3

Output:

```text
 *****
```

---

## Row 2

Output:

```text
  ***
```

---

## Row 1

Output:

```text
   *
```

---

# Second Half Summary Table

| Row (i) | Spaces | Stars | Output |
|----------|---------|---------|---------|
| 4 | 0 | 7 | ******* |
| 3 | 1 | 5 |  ***** |
| 2 | 2 | 3 |   *** |
| 1 | 3 | 1 |    * |

---

# Complete Dry Run Table

| Row | Spaces | Stars |
|------|---------|---------|
| 1 | 3 | 1 |
| 2 | 2 | 3 |
| 3 | 1 | 5 |
| 4 | 0 | 7 |
| 4 | 0 | 7 |
| 3 | 1 | 5 |
| 2 | 2 | 3 |
| 1 | 3 | 1 |

---

# Pattern Observation

### Spaces

```text
3
2
1
0
0
1
2
3
```

Spaces:

```text
Decrease
Then Increase
```

---

### Stars

```text
1
3
5
7
7
5
3
1
```

Stars:

```text
Increase
Then Decrease
```

---

# Visual Representation

```text
   *
  ***
 *****
*******
*******
 *****
  ***
   *
```

Notice:

```text
Perfect Symmetry
```

The upper half mirrors the lower half.

---

# Loop Analysis

## Outer Loop 1

```java
for(int i=1;i<=n;i++)
```

Creates:

```text
Upper Half
```

---

## Outer Loop 2

```java
for(int i=n;i>=1;i--)
```

Creates:

```text
Lower Half
```

---

## Inner Loop 1

```java
for(int j=1;j<=n-i;j++)
```

Prints:

```text
Spaces
```

---

## Inner Loop 2

```java
for(int j=1;j<=(2*i)-1;j++)
```

Prints:

```text
Stars
```

---

# Time Complexity

Outer Loops:

```text
2n
```

Inner Loops:

```text
n
```

Overall:

```text
O(n²)
```

---

# Easy Memory Trick

Think:

```text
Pyramid
+
Inverted Pyramid
=
Diamond
```

or

```text
Upper Half
+
Mirror Image
=
Diamond
```

---

# Key Learning

- Diamond Pattern uses symmetry.
- Spaces decrease and then increase.
- Stars increase and then decrease.
- Odd number star logic is used.
- Diamond is built using two pyramids.

---

# Special Note

Remember:

```java
Spaces = n - i
```

and

```java
Stars = (2 * i) - 1
```

These two formulas create the entire Diamond Pattern.
