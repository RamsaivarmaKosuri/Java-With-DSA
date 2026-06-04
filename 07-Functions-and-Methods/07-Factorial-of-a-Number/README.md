# Factorial of a Number

Factorial is a mathematical operation used to find the product of all positive integers less than or equal to a given number.

Factorial is represented using the symbol:

```text
!
```

For example:

```text
5! = 5 × 4 × 3 × 2 × 1 = 120
```

---

## Why Learn Factorial?

Factorial is used in:

- Mathematics
- Permutations and Combinations
- Probability
- Binomial Coefficient
- Competitive Programming

It is also one of the most common beginner-level function problems.

---

## Formula

```text
n! = n × (n-1) × (n-2) × ... × 1
```

Examples:

```text
1! = 1
2! = 2 × 1 = 2
3! = 3 × 2 × 1 = 6
4! = 4 × 3 × 2 × 1 = 24
5! = 5 × 4 × 3 × 2 × 1 = 120
```

---

## Program

```java
public class JavaBasics {

    public static int f(int n) {

        int fact = 1;

        for(int i = 1; i <= n; i++) {

            if(n < 0) {
                System.out.println("enter valid integer");
            } else {
                fact = fact * i;
            }

        }

        return fact;
    }

    public static void main(String[] args) {
        System.out.println(f(5));
    }
}
```

---

## Output

```text
120
```

---

## Easy Understanding

Suppose:

```text
n = 5
```

Initially:

```text
fact = 1
```

Now multiply each number from 1 to 5:

```text
fact = 1 × 1 = 1
fact = 1 × 2 = 2
fact = 2 × 3 = 6
fact = 6 × 4 = 24
fact = 24 × 5 = 120
```

Final Answer:

```text
120
```

---

## Dry Run

For:

```text
n = 5
```

| Iteration | i | fact Before | fact After |
|------------|---|------------|------------|
| 1 | 1 | 1 | 1 |
| 2 | 2 | 1 | 2 |
| 3 | 3 | 2 | 6 |
| 4 | 4 | 6 | 24 |
| 5 | 5 | 24 | 120 |

Final Output:

```text
120
```

---

## Dry Run Diagram

```text
fact = 1

1 × 1 = 1
      ↓
1 × 2 = 2
      ↓
2 × 3 = 6
      ↓
6 × 4 = 24
      ↓
24 × 5 = 120
```

---

## Time Complexity

```text
O(n)
```

Because the loop runs `n` times.

---

## Key Learning

- Creating functions
- Using loops inside functions
- Returning values from functions
- Understanding iterative calculations
- Building logic for mathematical problems

---

## Special Note

From my notes:

```text
Factorial of a number is calculated by multiplying all positive integers from 1 to n.
```

In the above code, the negative number check is placed inside the loop.

A better approach would be to check:

```java
if(n < 0)
```

before starting the loop, because factorial is not defined for negative numbers.

This makes the program more efficient and easier to understand.
