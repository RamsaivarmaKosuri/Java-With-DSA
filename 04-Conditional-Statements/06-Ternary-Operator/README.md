# Ternary Operator

Ternary operator is a shortcut for:

```text
if-else
```

It works using:

```text
3 operands
```

That is why it is called:

```text
Ternary Operator
```

---

## Syntax

```java
variable = (condition) ? statement1 : statement2;
```

### Understanding

If condition is:

```text
true
```

then:

```text
statement1
```

executes.

Otherwise:

```text
statement2
```

executes.

---

## Example 1: Find Larger Number

```java
public class JavaBasics {
    public static void main(String[] args) {

        int a = 5;
        int b = 3;

        int larger = (a > b) ? a : b;

        System.out.println(larger);

    }
}
```

## Output

```text
5
```

### Understanding

Condition:

```java
(a > b)
```

Result:

```text
true
```

So:

```text
a
```

gets selected.

---

## Example 2: Check Even or Odd

```java
public class JavaBasics {
    public static void main(String[] args) {

        int number = 7;

        String type = (number % 2 == 0) ? "EVEN" : "ODD";

        System.out.println(type);

    }
}
```

## Output

```text
ODD
```

### Understanding

Condition:

```java
number % 2 == 0
```

Result:

```text
false
```

So:

```text
"ODD"
```

gets selected.

---

## Your Notes

```java
boolean larger = (5 > 3) ? true : false;
```

```java
String type = (5 % 2 == 0) ? "EVEN" : "ODD";
```

---

## Important Note

Ternary operator is used when we want to write:

```text
if-else
```

in a shorter way.
