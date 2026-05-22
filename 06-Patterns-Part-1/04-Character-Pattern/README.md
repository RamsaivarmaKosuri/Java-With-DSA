# Character Pattern

In this pattern:

```text
characters (alphabets)
```

are printed instead of:

```text
stars or numbers
```

The characters print in:

```text
sequence order
```

like:

```text
A → B → C → D...
```

---

## Pattern Output

```text
A
BC
DEF
GHIJ
```

---

## Logic Behind Pattern

We use:

```text
Nested Loops
```

and a:

```java
character variable
```

to print letters.

We start with:

```java
char ch = 'A';
```

Then after printing:

```text
one character
```

we increase it using:

```java
ch++;
```

This moves character to:

```text
next alphabet
```

Example:

```text
A → B
B → C
C → D
```

---

## Understanding Character Increment

In Java:

```java
char
```

stores characters using:

```text
ASCII / Unicode values
```

Example:

```text
A = 65
B = 66
C = 67
```

So when we do:

```java
ch++;
```

Java automatically moves to:

```text
next character
```

Example:

```text
'A' → 'B'
'B' → 'C'
'C' → 'D'
```

---

## Example Program

```java
public class JavaBasics {
    public static void main(String[] args) {

        char ch = 'A';

        for(int line = 1; line <= 4; line++) {

            for(int chars = 1; chars <= line; chars++) {

                System.out.print(ch);
                ch++;

            }

            System.out.println();
        }
    }
}
```

## Output

```text
A
BC
DEF
GHIJ
```

---

## Code Understanding

### Step 1

```java
char ch = 'A';
```

We start character from:

```text
A
```

---

### Step 2

Outer loop:

```java
for(int line = 1; line <= 4; line++)
```

Controls:

```text
number of lines
```

---

### Step 3

Inner loop:

```java
for(int chars = 1; chars <= line; chars++)
```

Controls:

```text
number of characters to print
```

Example:

```text
Line 1 → 1 character
Line 2 → 2 characters
Line 3 → 3 characters
Line 4 → 4 characters
```

---

### Step 4

```java
System.out.print(ch);
```

prints current character.

---

### Step 5

```java
ch++;
```

moves to:

```text
next character
```

Example:

```text
A → B → C → D → E...
```

---

## Dry Run Diagram

```text
Initially:

ch = A

Line = 1
Print → A
ch becomes B

Line = 2
Print → B C
ch becomes D

Line = 3
Print → D E F
ch becomes G

Line = 4
Print → G H I J
```

---

## Your Notes

```java
// print character pattern

public class JavaBasics {
    public static void main(String[] args) {

        char ch = 'A';

        for(int line = 1; line <= 4; line++) {

            for(int chars = 1; chars <= line; chars++) {

                System.out.print(ch);
                ch++;

            }

            System.out.println();
        }
    }
}
```

---

## Important Note

```java
ch++
```

works because:

```text
characters internally have numeric values
```

So Java automatically moves to:

```text
next alphabet
```

Example:

```text
A → B → C → D
```
