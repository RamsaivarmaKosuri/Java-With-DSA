# Binomial Coefficient

The Binomial Coefficient is used to calculate the number of ways to choose `r` objects from `n` objects.

It is represented as:

```text
nCr
```

and is read as:

```text
n choose r
```

---

## Why Learn Binomial Coefficient?

The Binomial Coefficient is used in:

- Mathematics
- Probability
- Combinations
- Pascal's Triangle
- Competitive Programming

This problem also teaches an important programming concept:

```text
Function Reusability
```

where one function can be used inside another function.

---

## Formula

```text
nCr = n! / (r! × (n-r)!)
```

Example:

```text
5C2 = 5! / (2! × 3!)

    = 120 / (2 × 6)

    = 120 / 12

    = 10
```

---

## Program

```java
public class JavaBasics {

    public static int factorial(int n) {

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

    public static int binomial(int n, int r) {

        int fact_n = factorial(n);
        int fact_r = factorial(r);
        int fact_nmr = factorial(n-r);

        int coef = fact_n / (fact_r * fact_nmr);

        return coef;
    }

    public static void main(String[] args) {
        System.out.println(binomial(5, 2));
    }
}
```

---

## Output

```text
10
```

---

## Easy Understanding

Given:

```text
n = 5
r = 2
```

Formula:

```text
nCr = n! / (r! × (n-r)!)
```

Substituting values:

```text
5C2 = 5! / (2! × 3!)
```

Calculate factorials:

```text
5! = 120
2! = 2
3! = 6
```

Now:

```text
5C2 = 120 / (2 × 6)

     = 120 / 12

     = 10
```

Final Answer:

```text
10
```

---

## Function Flow Diagram

```text
main()
   │
   ▼
binomial(5,2)
   │
   ├── factorial(5) = 120
   │
   ├── factorial(2) = 2
   │
   ├── factorial(3) = 6
   │
   ▼
120 / (2 × 6)
   │
   ▼
10
```

---

## Dry Run Table

### Step 1

Calculate:

```text
factorial(5)
```

| i | fact |
|---|------|
| 1 | 1 |
| 2 | 2 |
| 3 | 6 |
| 4 | 24 |
| 5 | 120 |

Result:

```text
120
```

---

### Step 2

Calculate:

```text
factorial(2)
```

| i | fact |
|---|------|
| 1 | 1 |
| 2 | 2 |

Result:

```text
2
```

---

### Step 3

Calculate:

```text
factorial(3)
```

| i | fact |
|---|------|
| 1 | 1 |
| 2 | 2 |
| 3 | 6 |

Result:

```text
6
```

---

### Step 4

Apply Formula

| Value | Result |
|---------|--------|
| n! | 120 |
| r! | 2 |
| (n-r)! | 6 |
| 120 / (2 × 6) | 10 |

Final Output:

```text
10
```

---

## Time Complexity

Factorial function runs:

```text
O(n)
```

Since factorial is called three times:

```text
O(n)
```

overall.

---

## Key Learning

- Function Reusability
- Returning Values from Functions
- Mathematical Computations
- Factorial Application
- Problem Decomposition

---

## Special Note

From my notes:

```text
Here first we created a factorial function to calculate factorial and another function to calculate the Binomial Coefficient.
```

This is a good example of code reusability.

Instead of writing factorial logic multiple times, we create one function and use it whenever required.

This makes the code cleaner, shorter, and easier to maintain.
