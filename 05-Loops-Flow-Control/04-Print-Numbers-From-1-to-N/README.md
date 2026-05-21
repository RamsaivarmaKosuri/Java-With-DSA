# Print Numbers from 1 to N

This program prints numbers from:

```text
1 to N
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

## Logic

We start printing from:

```text
1
```

and continue until:

```text
N
```

After every iteration, count increases by:

```text
1
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

        while(count <= n) {
            System.out.println(count);
            count++;
        }

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
1
2
3
4
5
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

User enters the ending number.

Example:

```text
5
```

---

### Step 3

```java
int count = 1;
```

We start printing from:

```text
1
```

---

### Step 4

Condition:

```java
count <= n
```

checks whether count is less than or equal to:

```text
n
```

If condition becomes:

```text
true
```

loop runs.

---

### Step 5

```java
System.out.println(count);
```

prints the current number.

---

### Step 6

```java
count++;
```

increases value by:

```text
1
```

Loop repeats until condition becomes:

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
count = 1 → print 1
count = 2 → print 2
count = 3 → print 3
count = 4 → print 4
count = 5 → print 5
count = 6 → stop
```

---

## Your Notes

```java
import java.util.*;

public class wh {
    public static void main(String args[]) {

        Scanner sc = new Scanner(System.in);

        int n = sc.nextInt();

        int count = 1;

        while(count <= n) {
            System.out.println(count);
            count++;
        }

    }
}
```

---

## Important Note

The loop stops when:

```text
count > n
```
