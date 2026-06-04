# Primes in Range

In this problem, we print all Prime Numbers within a given range.

Instead of writing the prime-checking logic repeatedly, we reuse the previously created:

```java
isPrime()
```

function.

This is a good example of:

```text
Function Reusability
```

---

## Why Learn This?

This problem helps us understand:

- Function Reusability
- Prime Number Logic
- Nested Function Calls
- Loops with Functions
- Problem Decomposition

---

## Example

Input:

```text
25
```

Output:

```text
2 3 5 7 11 13 17 19 23
```

These are all prime numbers from:

```text
2 to 25
```

---

## Program

```java
public class JavaBasics {

    public static boolean isPrime(int n){

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

    public static void primeInRange(int n){

        for(int i = 2; i <= n; i++){

            if(isPrime(i)){
                System.out.print(i + " ");
            }

        }

        System.out.println();
    }

    public static void main(String[] args) {

        primeInRange(25);

    }
}
```

---

## Output

```text
2 3 5 7 11 13 17 19 23
```

---

## Easy Understanding

We check every number from:

```text
2 to n
```

For each number:

```java
isPrime(i)
```

is called.

If the number is prime:

```java
System.out.print(i + " ");
```

prints it.

---

## Function Flow Diagram

```text
primeInRange(25)
        │
        ▼
Check 2 → Prime → Print
        │
        ▼
Check 3 → Prime → Print
        │
        ▼
Check 4 → Not Prime
        │
        ▼
Check 5 → Prime → Print
        │
        ▼
...
        │
        ▼
Check 25 → Not Prime
```

---

## Dry Run

Input:

```text
n = 10
```

| Number | isPrime() Result | Output |
|----------|----------------|---------|
| 2 | true | 2 |
| 3 | true | 3 |
| 4 | false | - |
| 5 | true | 5 |
| 6 | false | - |
| 7 | true | 7 |
| 8 | false | - |
| 9 | false | - |
| 10 | false | - |

Final Output:

```text
2 3 5 7
```

---

## Detailed Example

Input:

```text
n = 25
```

Prime Numbers:

| Number | Prime? |
|----------|---------|
| 2 | Yes |
| 3 | Yes |
| 5 | Yes |
| 7 | Yes |
| 11 | Yes |
| 13 | Yes |
| 17 | Yes |
| 19 | Yes |
| 23 | Yes |

Output:

```text
2 3 5 7 11 13 17 19 23
```

---

## Time Complexity

The outer loop runs:

```text
n times
```

The prime check runs:

```text
O(√n)
```

Therefore:

```text
O(n√n)
```

---

## Key Learning

- Function Reusability
- Prime Number Logic
- Loops with Functions
- Nested Function Calls
- Efficient Prime Checking using √n

---

## Special Note

From my notes:

```text
public static void primeInRange(int n){

    for(int i=2;i<=n;i++){

        if(isPrime(i)){
            System.out.print(i+" ");
        }

    }

}
```

The best part of this program is that we reuse the already created:

```java
isPrime()
```

function.

This follows an important programming principle:

```text
Write Once, Reuse Multiple Times
```

which makes code cleaner, shorter, and easier to maintain.
