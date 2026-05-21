# Print Numbers from 1 to 10

This program prints numbers from:

```text
1 to 10
```

using:

```text
while loop
```

---

## Logic

We start from:

```text
1
```

and keep printing numbers until:

```text
10
```

After every iteration, value increases by:

```text
1
```

---

## Example Program

```java
public class JavaBasics {
    public static void main(String args[]) {

        int count = 1;

        while(count <= 10) {
            System.out.println(count);
            count++;
        }

    }
}
```

## Output

```text
1
2
3
4
5
6
7
8
9
10
```

---

## Code Understanding

### Step 1

```java
int count = 1;
```

We start counting from:

```text
1
```

---

### Step 2

Condition:

```java
count <= 10
```

checks whether count is less than or equal to:

```text
10
```

If:

```text
true
```

loop executes.

---

### Step 3

```java
System.out.println(count);
```

prints current value.

---

### Step 4

```java
count++;
```

increases count value by:

```text
1
```

This repeats until:

```text
count becomes 11
```

Then condition becomes:

```text
false
```

and loop stops.

---

## Dry Run

```text
count = 1 → print 1
count = 2 → print 2
count = 3 → print 3
...
count = 10 → print 10
count = 11 → stop
```

---

## Important Note

Always update the loop variable.

Example:

```java
count++;
```

Otherwise:

```text
Infinite Loop
```

may happen.
