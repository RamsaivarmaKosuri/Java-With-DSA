# Factorial of a Number

Factorial is one of the most common mathematical problems used to understand loops.

A factorial of a number is the product of all positive integers from:

```text
1 to n
```

---

## What is Factorial?

Factorial of a number is represented by:

```text
n!
```

Formula:

```text
n! = n × (n-1) × (n-2) × ... × 1
```

---

## Examples

```text
1! = 1

2! = 2 × 1 = 2

3! = 3 × 2 × 1 = 6

4! = 4 × 3 × 2 × 1 = 24

5! = 5 × 4 × 3 × 2 × 1 = 120
```

---

## Problem Statement

Take a:

```text
non-negative integer
```

from the user and calculate its factorial.

---

## Approach

1. Take input from the user.
2. Check if the number is negative.
3. If negative, factorial does not exist.
4. Otherwise, multiply all numbers from 1 to n.
5. Print the result.

---

## Program

```java
import java.util.*;

public class JavaBasics {
    public static void main(String[] args) {

        int fact = 1;

        Scanner sc = new Scanner(System.in);

        System.out.print("ENTER NON-NEGATIVE INTEGER : ");

        int n = sc.nextInt();

        if(n < 0) {
            System.out.print("FACTORIAL DOES NOT EXIST FOR NEGATIVE NUMBER");
        }
        else {

            for(int i = 1; i <= n; i++) {
                fact *= i;
            }

            System.out.print("THE FACTORIAL OF A NUMBER IS : " + fact);
        }
    }
}
```

---

## Example Input

```text
5
```

---

## Output

```text
THE FACTORIAL OF A NUMBER IS : 120
```

---

## Code Explanation

### Step 1

Create a variable:

```java
int fact = 1;
```

Why 1?

Because factorial is based on:

```text
multiplication
```

and multiplying with 1 does not change the value.

---

### Step 2

Take input:

```java
int n = sc.nextInt();
```

---

### Step 3

Check:

```java
if(n < 0)
```

Factorial is not defined for negative numbers.

---

### Step 4

Run loop:

```java
for(int i = 1; i <= n; i++)
```

Loop starts from:

```text
1
```

and goes till:

```text
n
```

---

### Step 5

Multiply:

```java
fact *= i;
```

which means:

```java
fact = fact * i;
```

---

## Dry Run

### Example: n = 5

```text
fact = 1

i = 1
fact = 1 × 1 = 1

i = 2
fact = 1 × 2 = 2

i = 3
fact = 2 × 3 = 6

i = 4
fact = 6 × 4 = 24

i = 5
fact = 24 × 5 = 120
```

Final Answer:

```text
120
```

---

## Visual Representation

```text
Start

fact = 1

      ↓

1 × 1 = 1

      ↓

1 × 2 = 2

      ↓

2 × 3 = 6

      ↓

6 × 4 = 24

      ↓

24 × 5 = 120

      ↓

Answer = 120
```

---

## Flow Diagram

```text
User Enters Number
         ↓
Check Negative?
    ↙         ↘
 Yes          No
  ↓            ↓
Print Error   Calculate Factorial
                   ↓
             Print Result
```

---

## Your Notes

```java
import java.util.*;

public class JavaBasics {
    public static void main(String[] args) {

        int fact = 1;

        Scanner sc = new Scanner(System.in);

        System.out.print("ENTER NON-NEGATIVE INTEGER :");

        int n = sc.nextInt();

        if(n < 0) {
            System.out.print("FACTORIAL DOES NOT EXIST FOR NEGATIVE NUMBER");
        }
        else {

            for(int i = 1; i <= n; i++) {
                fact *= i;
            }

            System.out.print("THE FACTORIAL OF A NUMBER IS : " + fact);
        }
    }
}
```

---

## Key Learning

```text
For Loop
Multiplication Accumulator
Mathematical Computation
Input Validation
Problem Solving
```

---

## Special Note

```text
0! = 1
```

This is a special mathematical rule and is commonly asked in interviews and exams.
