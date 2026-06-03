# X Pattern

The X Pattern is formed using two diagonals:

- Main Diagonal
- Secondary Diagonal

This pattern helps us understand:

- Row and Column Logic
- Conditions inside Nested Loops
- Diagonal-Based Patterns

---

## Problem Statement

Print an X Pattern of size `n`.

---

## Example Input

```text
5
```

---

## Output

```text
*   *
 * *
  *
 * *
*   *
```

---

## Pattern Analysis

The pattern contains two diagonals.

### Main Diagonal

```text
(1,1)
(2,2)
(3,3)
(4,4)
(5,5)
```

Condition:

```java
row == col
```

---

### Secondary Diagonal

```text
(1,5)
(2,4)
(3,3)
(4,2)
(5,1)
```

Condition:

```java
row + col == n + 1
```

---

## Logic

Print a star when:

```java
row == col || row + col == n + 1
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

                if(row == col || row + col == n + 1) {
                    System.out.print("*");
                } else {
                    System.out.print(" ");
                }

            }

            System.out.println();
        }
    }
}
```

---

## Dry Run

### Row 1

| Position | Condition | Output |
|----------|-----------|---------|
| (1,1) | row == col | * |
| (1,2) | False | Space |
| (1,3) | False | Space |
| (1,4) | False | Space |
| (1,5) | row + col = 6 | * |

Output:

```text
*   *
```

---

### Row 2

| Position | Condition | Output |
|----------|-----------|---------|
| (2,1) | False | Space |
| (2,2) | row == col | * |
| (2,3) | False | Space |
| (2,4) | row + col = 6 | * |
| (2,5) | False | Space |

Output:

```text
 * *
```

---

### Row 3

| Position | Condition | Output |
|----------|-----------|---------|
| (3,1) | False | Space |
| (3,2) | False | Space |
| (3,3) | Both Conditions True | * |
| (3,4) | False | Space |
| (3,5) | False | Space |

Output:

```text
  *
```

---

### Row 4

Output:

```text
 * *
```

---

### Row 5

Output:

```text
*   *
```

---

## Final Pattern

```text
*   *
 * *
  *
 * *
*   *
```

---

## Key Learning

- Nested Loops
- Row and Column Logic
- Diagonal-Based Conditions
- Pattern Visualization
- Problem Solving

---

## Special Note

The X Pattern is one of the first patterns that uses coordinate-based logic.

Instead of counting stars directly, we decide whether to print a star by checking the relationship between the current row and column positions.
