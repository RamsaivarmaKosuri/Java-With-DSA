# Introduction to Functions

In Java:

```text
Functions are blocks of code
```

that perform a:

```text
particular task
```

and can be:

```text
reused multiple times
```

Instead of writing same code again and again, we place it inside a:

```text
function
```

and call it whenever needed.

---

## Why Do We Need Functions?

Suppose we want to print:

```text
hello
```

many times after doing some work.

Without functions:

we have to write same code:

```text
again and again
```

This creates:

```text
code repetition
```

and makes code difficult to manage.

Functions help us:

```text
reuse code
```

---

## Example Without Function

```java
public class JavaBasics {
    public static void main(String[] args) {

        // work 1
        System.out.println("hello");

        // work 2
        System.out.println("hello");

        // work 3
        System.out.println("hello");

    }
}
```

### Problem Here

We are repeating:

```java
System.out.println("hello");
```

multiple times.

This is called:

```text
code duplication
```

---

## Example With Function

```java
public class JavaBasics {

    public static void printHello() {
        System.out.println("hello");

        return;
    }

    public static void main(String[] args) {

        printHello();
        printHello();
        printHello();

    }
}
```

## Output

```text
hello
hello
hello
```

---

## How This Works

### Step 1

We create a function:

```java
public static void printHello()
```

named:

```text
printHello
```

---

### Step 2

Inside function:

```java
System.out.println("hello");
```

stores the reusable code.

---

### Step 3

Whenever we write:

```java
printHello();
```

Java:

```text
calls the function
```

and executes code inside it.

---

## Function Reusability

We can call function:

```text
how many times we want
```

Example:

```java
printHello();
printHello();
printHello();
```

This avoids:

```text
writing same code repeatedly
```

---

## Important Understanding

Example:

```java
public static void printHello()
```

Here:

### `public`

Means:

```text
accessible from anywhere
```

---

### `static`

Means:

```text
can be called without creating object
```

---

### `void`

Means:

```text
nothing is returned
```

(khali)

This function does not return any value.

---

### `printHello()`

This is:

```text
function name
```

---

## Your Notes

```java
// Functions and Methods

// introduction of functions

// in java functions are the block of code that performs particular task
// and that can be reusable

// Example--without function

public class JavaBasics {
    public static void main(String[] args) {

        // body
        System.out.println("hello");
        // work 1

        System.out.println("hello");
        // work 2

        System.out.println("hello");

        // like here we want to print hello after some work has done,
        // so instead of copying that every time we use function
    }
}
```

```java
// with function

public class JavaBasics {

    public static void printHello() {

        System.out.println("hello");

        return;

        // here we can use return or remove it.
        // it does not give error because return type is void.
        // but while using another return type
        // we must return otherwise we get error
    }

    public static void main(String[] args) {

        printHello();

        // Function call
        // here we call the function
        // now the code inside function works

        // we can call it how many times we want
    }
}
```

---

## Important Note

A function helps in:

```text
Write Once → Use Multiple Times
```

This is called:

```text
Code Reusability
```
