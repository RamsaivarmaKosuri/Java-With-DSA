# Multiplication Table

A multiplication table shows the result of multiplying a number by different integers.

This problem helps us understand:

- Loops
- User Input
- Repeated Calculations
- Mathematical Operations

---

## Problem Statement

Take a number from the user and print its multiplication table from 1 to 10.

---

## Example

For:

```text
5
```

The table will be:

```text
5 x 1 = 5
5 x 2 = 10
5 x 3 = 15
5 x 4 = 20
5 x 5 = 25
5 x 6 = 30
5 x 7 = 35
5 x 8 = 40
5 x 9 = 45
5 x 10 = 50
```

---

## Approach

1. Take a number from the user.
2. Run a loop from 1 to 10.
3. Multiply the number with the loop variable.
4. Print the result.

---

## Program

```java
import java.util.*;

public class JavaBasics {
    public static void main(String[] args) {

        Scanner sc = new Scanner(System.in);

        System.out.print("ENTER NUMBER TO GET THE TABLE : ");

        int n = sc.nextInt();

        for(int i = 1; i <= 10; i++) {
            System.out.println(n + " x " + i + " = " + (n * i));
        }
    }
}
```

---

## Example Input

```text
7
```

## Output

```text
7 x 1 = 7
7 x 2 = 14
7 x 3 = 21
7 x 4 = 28
7 x 5 = 35
7 x 6 = 42
7 x 7 = 49
7 x 8 = 56
7 x 9 = 63
7 x 10 = 70
```

---

## Code Explanation

### Step 1

Take input from the user:

```java
int n = sc.nextInt();
```

Example:

```text
n = 7
```

---

### Step 2

Run a loop:

```java
for(int i = 1; i <= 10; i++)
```

The loop executes 10 times.

---

### Step 3

Multiply:

```java
n * i
```

for every iteration.

---

### Step 4

Print the result:

```java
System.out.println(n + " x " + i + " = " + (n * i));
```

---

## Dry Run

### Example: n = 5

```text
i = 1
5 x 1 = 5

i = 2
5 x 2 = 10

i = 3
5 x 3 = 15

i = 4
5 x 4 = 20

i = 5
5 x 5 = 25

i = 6
5 x 6 = 30

i = 7
5 x 7 = 35

i = 8
5 x 8 = 40

i = 9
5 x 9 = 45

i = 10
5 x 10 = 50
```

---

## Iteration Table

| i | Calculation | Result |
|---|------------|----------|
| 1 | 5 × 1 | 5 |
| 2 | 5 × 2 | 10 |
| 3 | 5 × 3 | 15 |
| 4 | 5 × 4 | 20 |
| 5 | 5 × 5 | 25 |
| 6 | 5 × 6 | 30 |
| 7 | 5 × 7 | 35 |
| 8 | 5 × 8 | 40 |
| 9 | 5 × 9 | 45 |
| 10 | 5 × 10 | 50 |

---

## Flow Diagram

```text
User Enters Number
         ↓
     Start Loop
         ↓
   Multiply n × i
         ↓
    Print Result
         ↓
   Next Iteration
         ↓
      Until 10
```

---

## Your Notes

```java
import java.util.*;

public class JavaBasics {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        System.out.print("ENTER NUMBER TO GET THE TABLE :");

        int n = sc.nextInt();

        for(int i = 1; i <= 10; i++) {
            System.out.println(n + "x" + i + "=" + n * i);
        }
    }
}
```

---

## Key Learning

```text
For Loop
Repeated Calculations
Loop Iterations
User Input
Mathematical Operations
```

---

## Special Note

The multiplication table problem is one of the best beginner exercises because it teaches how loops can perform the same operation multiple times with different values.
