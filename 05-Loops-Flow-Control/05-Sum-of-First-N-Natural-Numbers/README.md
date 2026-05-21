# Sum of First N Natural Numbers

This program calculates the:

```text
Sum of first N natural numbers
```

using:

```text
while loop
```

Here:

```text
N
```

is entered by the user.

---

## What are Natural Numbers?

Natural numbers start from:

```text
1
```

Example:

```text
1, 2, 3, 4, 5...
```

---

## Logic

We start from:

```text
1
```

and keep adding numbers until:

```text
N
```

Example:

If:

```text
N = 5
```

Then:

```text
1 + 2 + 3 + 4 + 5 = 15
```

---

## Example Program

```java
import java.util.*;

public class JavaBasics {
    public static void main(String args[]) {

        Scanner sc = new Scanner(System.in);

        int n = sc.nextInt();

        int count = 1;
        int sum = 0;

        while(count <= n) {

            sum = sum + count;
            count++;

        }

        System.out.println(sum);

    }
}
```

---

## Example Input

```text
5
```

## Output

```text
15
```

---

## Code Understanding

### Step 1

```java
Scanner sc = new Scanner(System.in);
```

Used to take input from user.

---

### Step 2

```java
int n = sc.nextInt();
```

User enters the value of:

```text
N
```

Example:

```text
5
```

---

### Step 3

```java
int count = 1;
```

Starts counting from:

```text
1
```

---

### Step 4

```java
int sum = 0;
```

Variable used to store total sum.

Initially:

```text
0
```

---

### Step 5

Condition:

```java
count <= n
```

checks whether counting should continue.

---

### Step 6

```java
sum = sum + count;
```

adds current number into sum.

Example:

```text
sum = 0 + 1 = 1
sum = 1 + 2 = 3
sum = 3 + 3 = 6
sum = 6 + 4 = 10
sum = 10 + 5 = 15
```

---

### Step 7

```java
count++;
```

increases count by:

```text
1
```

until condition becomes:

```text
false
```

---

## Dry Run

For input:

```text
n = 5
```

```text
count = 1 → sum = 1
count = 2 → sum = 3
count = 3 → sum = 6
count = 4 → sum = 10
count = 5 → sum = 15
count = 6 → stop
```

---

## Your Notes

```java
import java.util.*;

public class natural {
    public static void main(String args[]) {

        Scanner sc = new Scanner(System.in);

        int n = sc.nextInt();

        int count = 1;
        int sum = 0;

        while(count <= n) {

            sum = sum + count;
            count++;

        }

        System.out.println(sum);
    }
}
```

---

## Important Note

Natural numbers start from:

```text
1
```

not:

```text
0
```
