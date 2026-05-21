# Print Whether a Number is Odd or Even

This program checks whether a number is:

```text
Even
```

or

```text
Odd
```

using:

```text
if-else
```

statement.

---

## Logic

If:

```text
number % 2 == 0
```

then number is:

```text
Even
```

Otherwise:

```text
Odd
```

---

## Why `%` (Modulus)?

`%` gives the remainder.

Example:

```text
10 % 2 = 0
```

If remainder is:

```text
0
```

then number is even.

---

## Example Program

```java
public class JavaBasics {
    public static void main(String[] args) {

        int number = 7;

        if(number % 2 == 0) {
            System.out.println("Even");
        }
        else {
            System.out.println("Odd");
        }

    }
}
```

## Output

```text
Odd
```

---

## Another Example

```java
int number = 10;
```

## Output

```text
Even
```

---

## Understanding

Condition:

```java
number % 2 == 0
```

checks remainder.

If remainder is:

```text
0
```

→ Even number

Else:

```text
Odd number
```
