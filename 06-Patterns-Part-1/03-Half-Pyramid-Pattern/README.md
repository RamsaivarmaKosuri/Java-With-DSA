# Half Pyramid Pattern

In this pattern:

```text
numbers increase line by line
```

Unlike star patterns:

```text
*
**
***
****
```

Here we print:

```text
numbers
```

instead of stars.

---

## Pattern Output

```text
1
12
123
1234
```

---

## Logic Behind Pattern

We use:

```text
Nested Loops
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
how many numbers to print
```

The number of values printed:

```text
increases every line
```

---

## Understanding the Pattern

```text
Line 1 → 1 number
Line 2 → 2 numbers
Line 3 → 3 numbers
Line 4 → 4 numbers
```

The inner loop prints from:

```text
1 to line number
```

---

## Example Program

```java
public class JavaBasics {
    public static void main(String[] args) {

        for(int line = 1; line <= 4; line++) {

            for(int num = 1; num <= line; num++) {
                System.out.print(num);
            }

            System.out.println();
        }
    }
}
```

## Output

```text
1
12
123
1234
```

---

## Code Understanding

### Outer Loop

```java
for(int line = 1; line <= 4; line++)
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
for(int num = 1; num <= line; num++)
```

Controls:

```text
numbers to print
```

The inner loop prints numbers from:

```text
1 to line
```

Example:

```text
line = 3
```

prints:

```text
123
```

---

## Dry Run Diagram

```text
Line = 1
num = 1
Output → 1

Line = 2
num = 1, 2
Output → 12

Line = 3
num = 1, 2, 3
Output → 123

Line = 4
num = 1, 2, 3, 4
Output → 1234
```

---

## Your Notes

```java
// print half-pyramid pattern

public class JavaBasics {
    public static void main(String[] args) {

        for(int line = 1; line <= 4; line++) {

            for(int num = 1; num <= line; num++) {
                System.out.print(num);
            }

            System.out.println();
        }
    }
}
```

---

## Important Note

In this pattern:

```text
line number
```

decides:

```text
how many numbers will print
```

Example:

```text
Line 3 → prints 3 numbers
Line 4 → prints 4 numbers
```
