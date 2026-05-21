# Loops Basics

Loops are used to execute a block of code repeatedly.

Instead of writing the same code again and again, we use loops.

Loops save:

- Time
- Code length
- Effort

---

## Why Do We Use Loops?

Imagine printing:

```text
Hello
```

10 times.

Without loops:

```java
System.out.println("Hello");
System.out.println("Hello");
System.out.println("Hello");
System.out.println("Hello");
System.out.println("Hello");
System.out.println("Hello");
System.out.println("Hello");
System.out.println("Hello");
System.out.println("Hello");
System.out.println("Hello");
```

This becomes very lengthy.

Using loops:

```java
for(int i = 1; i <= 10; i++) {
    System.out.println("Hello");
}
```

This is shorter and cleaner.

---

## Types of Loops in Java

### 1. While Loop

Used when number of iterations is not fixed.

---

### 2. For Loop

Used when number of iterations is known.

---

### 3. Do While Loop

Executes at least:

```text
one time
```

even if condition becomes false.

---

## Your Notes

```text
LOOPS

TYPES:
while
for
do while
```

---

## Real Life Example

Think of an alarm clock.

If alarm rings every day:

```text
repeat → repeat → repeat
```

That repeating process is similar to a:

```text
Loop
```

---

## Important Note

Loops continue execution until condition becomes:

```text
false
```
