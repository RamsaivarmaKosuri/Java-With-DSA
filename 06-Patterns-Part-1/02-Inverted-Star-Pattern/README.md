# Inverted Star Pattern

In this pattern, the number of stars:

```text
decreases line by line
```

Unlike the normal star pattern:

```text
*
**
***
****
```

Here the stars print in:

```text
reverse order
```

---

## Pattern Output

```text
****
***
**
*
```

---

## Logic Behind Pattern

We use:

```text
2 loops
```

### Outer Loop

Controls:

```text
number of lines
```

---

### Inner Loop

Controls:

```text
number of stars
```

But here:

```text
stars decrease
```

after every line.

---

## Formula Used

```java
n - line + 1
```

Where:

```text
n = total lines
```

This formula decides:

```text
how many stars to print
```

---

## Understanding Formula

Suppose:

```text
n = 4
```

Then:

```text
Line 1 → 4 - 1 + 1 = 4 stars
Line 2 → 4 - 2 + 1 = 3 stars
Line 3 → 4 - 3 + 1 = 2 stars
Line 4 → 4 - 4 + 1 = 1 star
```

---

## Example Program

```java
public class JavaBasics {
    public static void main(String[] args) {

        int n = 4;

        for(int line = 1; line <= n; line++) {

            for(int star = 1; star <= (n - line + 1); star++) {
                System.out.print("*");
            }

            System.out.println();
        }
    }
}
```

## Output

```text
****
***
**
*
```

---

## Code Understanding

### Outer Loop

```java
for(int line = 1; line <= n; line++)
```

Controls:

```text
number of lines
```

Runs:

```text
4 times
```

---

### Inner Loop

```java
for(int star = 1; star <= (n-line+1); star++)
```

Controls:

```text
number of stars
```

Stars reduce after every line.

---

## Dry Run Diagram

```text
n = 4

Line = 1
Stars = 4
Output → ****

Line = 2
Stars = 3
Output → ***

Line = 3
Stars = 2
Output → **

Line = 4
Stars = 1
Output → *
```

---

## Your Notes

```java
// print inverted star pattern

public class JavaBasics {
    public static void main(String[] args) {

        int n = 4;

        for(int line = 1; line <= 4; line++) {

            for(int star = 1; star <= (n-line+1); star++) {
                System.out.print("*");
            }

            System.out.println();
        }
    }
}
```

---

## Important Note

In:

```text
Normal Star Pattern
```

stars:

```text
increase
```

But in:

```text
Inverted Star Pattern
```

stars:

```text
decrease
```

This happens because of:

```java
n - line + 1
```
