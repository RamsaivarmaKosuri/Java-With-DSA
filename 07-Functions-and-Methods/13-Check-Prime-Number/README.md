# Check Prime Number

A Prime Number is a number that has exactly two factors:

```text
1 and the number itself
```

Examples:

```text
2, 3, 5, 7, 11, 13, 17...
```

Non-Prime Numbers:

```text
4, 6, 8, 9, 10, 12...
```

because they have more than two factors.

---

## Why Learn Prime Numbers?

Prime Numbers are used in:

- Mathematics
- Number Theory
- Competitive Programming
- Coding Interviews
- Cryptography

Prime checking is one of the most common logic-building problems.

---

## Examples

### Prime Number

```text
7
```

Factors:

```text
1, 7
```

Only two factors.

Therefore:

```text
7 is Prime
```

---

### Non Prime Number

```text
12
```

Factors:

```text
1, 2, 3, 4, 6, 12
```

More than two factors.

Therefore:

```text
12 is Not Prime
```

---

## Program

```java
public class JavaBasics {

    public static boolean isPrime(int n) {

        if(n == 2){
            return true;
        }

        for(int i = 2; i <= Math.sqrt(n); i++){

            if(n % i == 0){
                return false;
            }

        }

        return true;
    }

    public static void main(String[] args) {

        System.out.println(isPrime(34));

    }
}
```

---

## Output

```text
false
```

---

## Logic

If a number is divisible by any number between:

```text
2 to √n
```

then it is not prime.

Otherwise it is prime.

---

## Why Use Math.sqrt(n)?

Suppose:

```text
n = 36
```

Factors:

```text
1 × 36
2 × 18
3 × 12
4 × 9
6 × 6
```

After reaching:

```text
√36 = 6
```

the factors start repeating.

Therefore checking beyond √n is unnecessary.

This reduces the number of iterations.

---

## Dry Run

Input:

```text
n = 34
```

Square Root:

```text
√34 ≈ 5.83
```

Loop runs until:

```text
i = 5
```

| Iteration | i | n % i | Result |
|------------|---|--------|---------|
| 1 | 2 | 34 % 2 = 0 | Divisible |

Since:

```text
34 % 2 = 0
```

The function immediately returns:

```text
false
```

Output:

```text
false
```

---

## Another Example

Input:

```text
n = 17
```

Square Root:

```text
√17 ≈ 4.12
```

Loop runs till:

```text
i = 4
```

| Iteration | i | n % i |
|------------|---|--------|
| 1 | 2 | 1 |
| 2 | 3 | 2 |
| 3 | 4 | 1 |

No divisor found.

Therefore:

```text
17 is Prime
```

Output:

```text
true
```

---

## Flow Diagram

```text
isPrime(34)
      │
      ▼
Check n == 2 ?
      │
      ▼
No
      │
      ▼
34 % 2 == 0
      │
      ▼
Return false
```

---

## Time Complexity

Without optimization:

```text
O(n)
```

Using:

```java
Math.sqrt(n)
```

Time Complexity becomes:

```text
O(√n)
```

which is much faster.

---

## Key Learning

- Prime numbers have exactly two factors.
- A number is prime if it is not divisible by any number from 2 to √n.
- Math.sqrt(n) helps optimize the solution.
- The function returns boolean values.
- Prime checking is an important interview problem.

---

## Special Note

From my notes:

```text
if(n == 2){
    return true;
}

for(int i=2; i<=Math.sqrt(n); i++){

    if(n%i == 0){
        return false;
    }

}

return true;
```

The important optimization is:

```java
Math.sqrt(n)
```

Instead of checking all numbers till `n-1`, we only check till `√n`, making the solution more efficient.
