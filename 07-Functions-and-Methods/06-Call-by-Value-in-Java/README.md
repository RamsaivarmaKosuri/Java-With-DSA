# Call by Value in Java

Java always uses **Call by Value**.

When we pass variables to a function, Java sends a **copy of the value** instead of the original variable.

Because of this, any changes made inside the function do not affect the original variables.

---

## Why Learn Call by Value?

Understanding Call by Value helps us understand:

- How functions receive data
- How memory works during function calls
- Why changes inside functions do not affect original variables
- Difference between Call by Value and Call by Reference

This is one of the most important Java interview concepts.

---

## What is Call by Value?

In Java, when a function is called, a copy of the variable's value is passed to the function.

This means:

- The function works on the copied value.
- The original variable remains unchanged.
- Any modification inside the function affects only the local copy.

From my notes:

```text
Here in Java, functions ke andar variables ki copy jaati hai rather than original variable value.

That is why we call it Call by Value.
```

---

## Program

```java
public class JavaBasics {

    public static void swap(int a, int b) {

        // swap
        int temp = a;
        a = b;
        b = temp;

        System.out.println("a : " + a);
        System.out.println("b : " + b);
    }

    public static void main(String[] args) {

        int a = 5;
        int b = 10;

        swap(a, b);
    }
}
```

---

## Output

```text
a : 10
b : 5
```

---

## Easy Understanding

Initially:

```text
a = 5
b = 10
```

Function Call:

```java
swap(a, b);
```

Java does not send the original variables.

Instead, it creates copies:

```text
a(copy) = 5
b(copy) = 10
```

The swap operation is performed on these copies.

Therefore, the original variables inside `main()` remain unchanged.

---

## Dry Run

### Initial Values

| Variable | Value |
|----------|--------|
| a | 5 |
| b | 10 |

---

### Function Call

```java
swap(a, b);
```

Copies are passed to the function.

| Variable | Value |
|----------|--------|
| a | 5 |
| b | 10 |

---

### After

```java
int temp = a;
```

| Variable | Value |
|----------|--------|
| temp | 5 |
| a | 5 |
| b | 10 |

---

### After

```java
a = b;
```

| Variable | Value |
|----------|--------|
| temp | 5 |
| a | 10 |
| b | 10 |

---

### After

```java
b = temp;
```

| Variable | Value |
|----------|--------|
| temp | 5 |
| a | 10 |
| b | 5 |

---

### Final Output

| Variable | Value |
|----------|--------|
| a | 10 |
| b | 5 |

Output:

```text
a : 10
b : 5
```

---

## Memory Diagram

### Before Function Call

```text
main()

a = 5
b = 10
```

---

### During Function Call

```text
main()                swap()

a = 5                 a = 5
b = 10                b = 10
```

---

### After Swapping

```text
main()                swap()

a = 5                 a = 10
b = 10                b = 5
```

---

### After Function Ends

```text
main()

a = 5
b = 10
```

The memory used by the `swap()` function is removed from the call stack.

---

## Call by Value vs Call by Reference

| Call by Value | Call by Reference |
|--------------|------------------|
| Copy of value is passed | Actual variable/reference is passed |
| Original variable remains unchanged | Original variable can change |
| Java uses this approach | Commonly discussed in C++ |

---

## Key Learning

- Java always uses Call by Value.
- Functions receive copies of values.
- Changes inside a function do not affect original variables.
- Local variables exist only inside the function.
- Understanding Call by Value helps in learning memory management and function calls.

---

## Special Note

From my notes:

```text
Here in Java functions ke andar variables ki copy jaati hai rather than original variable value.

That is why we call it Call by Value.

Agar direct variable ki value/reference pass hoti hai to use Call by Reference kehte hai.

Ye concept commonly C++ mein discuss kiya jata hai.
```

Even though the swap happens successfully inside the function, the original variables inside `main()` remain unchanged because Java passes copies of values, not the actual variables.
