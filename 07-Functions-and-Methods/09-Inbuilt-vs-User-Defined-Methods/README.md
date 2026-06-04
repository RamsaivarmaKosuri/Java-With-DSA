# Inbuilt vs User Defined Methods

In Java, methods are mainly divided into two types:

1. User Defined Methods
2. Inbuilt Methods

---

## What are Methods?

A method is a block of code that performs a specific task.

Methods help us:

- Reuse code
- Reduce code duplication
- Improve readability
- Make programs easier to maintain

---

## Types of Methods

```text
Methods
│
├── User Defined Methods
│
└── Inbuilt Methods
```

---

## User Defined Methods

User Defined Methods are the methods created by programmers according to their requirements.

Examples:

```java
factorial()
sum()
product()
```

Example Program:

```java
public class JavaBasics {

    public static int sum(int a, int b) {
        return a + b;
    }

    public static void main(String[] args) {
        System.out.println(sum(5, 3));
    }
}
```

Output:

```text
8
```

---

## Inbuilt Methods

Inbuilt Methods are already provided by Java.

We can directly use them without creating them ourselves.

Examples:

```java
Math.pow()
Math.sqrt()
Math.max()
Scanner.nextInt()
```

Example Program:

```java
import java.util.*;

public class JavaBasics {

    public static void main(String[] args) {

        System.out.println(Math.pow(2,3));
        System.out.println(Math.sqrt(25));
        System.out.println(Math.max(10,20));
    }
}
```

Output:

```text
8.0
5.0
20
```

---

## Comparison Table

| User Defined Methods | Inbuilt Methods |
|---------------------|----------------|
| Created by Programmer | Already provided by Java |
| Written according to requirement | Ready to use |
| Need method definition | No need to define |
| Example: factorial() | Example: Math.sqrt() |

---

## Easy Understanding

Suppose you want to calculate factorial.

You create:

```java
factorial()
```

This becomes a User Defined Method.

Suppose you want square root.

Java already provides:

```java
Math.sqrt()
```

This becomes an Inbuilt Method.

---

## Real Life Analogy

Think of a mobile phone.

### Inbuilt Features

```text
Camera
Calculator
Clock
Gallery
```

These are already available.

### User Created Features

```text
Notes
Projects
Files
Documents
```

Created according to your needs.

Similarly:

```text
Java Methods
│
├── Inbuilt
└── User Defined
```

---

## Key Learning

- Methods are used to perform specific tasks.
- Java provides many ready-made methods.
- Programmers can create their own methods.
- User Defined Methods solve custom problems.
- Inbuilt Methods save development time.

---

## Special Note

From my notes:

```text
Methods

User Defined
-------------
factorial()
sum()
product()

Inbuilt
--------
Math.pow()
Math.sqrt()
Math.max()
sc.nextInt()
```

While programming, we use both types of methods together.

For example:

- Create a factorial() method ourselves.
- Use Math.pow() provided by Java.

This makes programming faster and more efficient.
