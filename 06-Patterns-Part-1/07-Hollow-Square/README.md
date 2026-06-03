# Hollow Square

A Hollow Square is a pattern where stars are printed only on the boundary, while the inner area remains empty.

This pattern helps us understand:

- Boundary Checking
- Nested Loops
- Row and Column Logic
- Conditional Statements

---

## Problem Statement

Print a Hollow Square Pattern of size `n`.

---

## Example Input

```text
5
```

---

## Output

```text
*****
*   *
*   *
*   *
*****
```

---

## Pattern Analysis

In a Hollow Square:

- First Row contains all stars.
- Last Row contains all stars.
- First Column contains stars.
- Last Column contains stars.
- All remaining positions contain spaces.

For a square of size `5 × 5`:

```text
*****
*   *
*   *
*   *
*****
```

---

## Easy Understanding

Ask yourself:

```text
Is the current position on the boundary?
```

If YES:

```text
Print *
```

Otherwise:

```text
Print Space
```

The boundary means:

```java
row == 1
```

OR

```java
row == n
```

OR

```java
col == 1
```

OR

```java
col == n
```

---

## Logic

Print a star when:

```java
row == 1 || row == n || col == 1 || col == n
```

Otherwise print a space.

---

## Program

```java
import java.util.*;

public class JavaBasics {
    public static void main(String[] args) {

        Scanner sc = new Scanner(System.in);

        int n = sc.nextInt();

        for(int row = 1; row <= n; row++) {

            for(int col = 1; col <= n; col++) {

                if(row == 1 || row == n ||
                   col == 1 || col == n) {

                    System.out.print("*");
                }
                else {
                    System.out.print(" ");
                }

            }

            System.out.println();
        }
    }
}
```

---

## Dry Run Table (n = 5)

### Row 1

Since `row == 1`, every position prints a star.

| Column | Output |
|----------|--------|
| 1 | * |
| 2 | * |
| 3 | * |
| 4 | * |
| 5 | * |

Output:

```text
*****
```

---

### Row 2

| Position | Condition | Output |
|-----------|-----------|--------|
| (2,1) | col == 1 | * |
| (2,2) | False | Space |
| (2,3) | False | Space |
| (2,4) | False | Space |
| (2,5) | col == n | * |

Output:

```text
*   *
```

---

### Row 3

| Position | Condition | Output |
|-----------|-----------|--------|
| (3,1) | col == 1 | * |
| (3,2) | False | Space |
| (3,3) | False | Space |
| (3,4) | False | Space |
| (3,5) | col == n | * |

Output:

```text
*   *
```

---

### Row 4

| Position | Condition | Output |
|-----------|-----------|--------|
| (4,1) | col == 1 | * |
| (4,2) | False | Space |
| (4,3) | False | Space |
| (4,4) | False | Space |
| (4,5) | col == n | * |

Output:

```text
*   *
```

---

### Row 5

Since `row == n`, every position prints a star.

| Column | Output |
|----------|--------|
| 1 | * |
| 2 | * |
| 3 | * |
| 4 | * |
| 5 | * |

Output:

```text
*****
```

---

## Final Pattern

```text
*****
*   *
*   *
*   *
*****
```

---

## Key Learning

- Nested Loops
- Boundary Checking
- Row and Column Logic
- Conditional Statements
- Pattern Visualization

---

## Special Note

The Hollow Square introduces one of the most important pattern concepts:

```java
row == 1 || row == n || col == 1 || col == n
```

This is called **Boundary Checking**.

Many advanced patterns are built using the same idea, so understanding this pattern will make future pattern problems much easier.
