# Question - Break Keyword

## Problem Statement

Keep entering numbers from the user until the user enters a:

```text
multiple of 10
```

When user enters a multiple of:

```text
10
```

the program should stop.

We use:

```text
break statement
```

to exit the loop.

---

## Logic

We continuously take input from the user using:

```text
while(true)
```

This creates an:

```text
infinite loop
```

Then we check:

```java
n % 10 == 0
```

If condition becomes:

```text
true
```

we use:

```java
break;
```

to stop the loop.

---

## Example Program

```java
import java.util.*;

public class JavaBasics {
    public static void main(String[] args) {

        Scanner sc = new Scanner(System.in);

        while(true) {

            int n = sc.nextInt();

            if(n % 10 == 0) {
                break;
            }

        }

        System.out.println("User entered multiple of 10");

    }
}
```

---

## Example Input

```text
23
45
67
90
```

## Output

```text
User entered multiple of 10
```

because:

```text
90
```

is divisible by:

```text
10
```

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
break;
```

and loop stops.

---

## Dry Run

Input:

```text
23 → continue
45 → continue
67 → continue
90 → break
```

Program stops.

---

## Your Notes

```java
import java.util.*;

public class JavaBasics {
    public static void main(String[] args) {

        Scanner sc = new Scanner(System.in);

        while(true) {

            int n = sc.nextInt();

            if(n % 10 == 0) {
                break;
            }

        }

        System.out.println("User entered multiple of 10");
    }
}
```

---

## Important Note

```java
while(true)
```

means loop runs:

```text
forever
```

until:

```java
break;
```

is encountered.
