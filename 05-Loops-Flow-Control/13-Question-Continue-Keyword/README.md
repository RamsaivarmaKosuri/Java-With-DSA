# Question - Continue Keyword

## Problem Statement

Display all numbers entered by the user except:

```text
multiples of 10
```

If user enters a number divisible by:

```text
10
```

that number should be:

```text
skipped
```

using:

```text
continue statement
```

---

## Logic

We continuously take numbers from the user.

If a number becomes:

```text
multiple of 10
```

we use:

```java
continue;
```

to skip that iteration.

Otherwise:

```text
print the number
```

---

## Example Program

```java
import java.util.*;

public class JavaBasics {
    public static void main(String[] args) {

        Scanner sc = new Scanner(System.in);

        while(true) {

            System.out.println("Enter your number : ");

            int n = sc.nextInt();

            if(n % 10 == 0) {
                continue;
            }

            System.out.println("Number was : " + n);
        }
    }
}
```

---

## Example Input

```text
23
40
57
90
18
```

## Output

```text
Number was : 23
Number was : 57
Number was : 18
```

Because:

```text
40 and 90
```

are multiples of:

```text
10
```

so they are skipped.

---

## Code Understanding

### Step 1

```java
while(true)
```

creates an:

```text
infinite loop
```

which runs forever.

---

### Step 2

```java
int n = sc.nextInt();
```

takes input from user.

---

### Step 3

Condition:

```java
n % 10 == 0
```

checks whether number is divisible by:

```text
10
```

---

### Step 4

If condition becomes:

```text
true
```

Java executes:

```java
continue;
```

This skips current iteration.

So:

```text
that number does not print
```

---

### Step 5

If condition becomes:

```text
false
```

Java executes:

```java
System.out.println("Number was : " + n);
```

and prints the number.

---

## Dry Run

```text
23 → print
40 → skip
57 → print
90 → skip
18 → print
```

---

## Your Notes

```java
import java.util.*;

public class JavaBasics {
    public static void main(String[] args) {

        Scanner sc = new Scanner(System.in);

        while(true) {

            System.out.println("Enter your number : ");

            int n = sc.nextInt();

            if(n % 10 == 0) {
                continue;
            }

            System.out.println("number was : " + n);
        }
    }
}
```

---

## Important Note

```java
continue;
```

does not stop the loop.

It only:

```text
skips current iteration
```

and moves to the:

```text
next iteration
```
