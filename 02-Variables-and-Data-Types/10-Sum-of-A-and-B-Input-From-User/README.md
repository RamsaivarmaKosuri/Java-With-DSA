# Sum of A and B (Input from User)

## Problem Statement

Take two numbers from the user and print their sum.

---

## Example Program

```java
import java.util.*;

public class JavaBasics {
    public static void main(String[] args) {

        Scanner sc = new Scanner(System.in);

        int a = sc.nextInt();
        int b = sc.nextInt();

        System.out.println(a + b);

    }
}
```

---

## Understanding the Code

### Create Scanner Object

```java
Scanner sc = new Scanner(System.in);
```

Used to take input from the keyboard.

---

### Take First Input

```java
int a = sc.nextInt();
```

Stores first number.

---

### Take Second Input

```java
int b = sc.nextInt();
```

Stores second number.

---

### Print Sum

```java
System.out.println(a + b);
```

Adds and prints result.

---

## Example Input

```text
10
20
```

## Output

```text
30
```

## Important Note

`nextInt()` is used to take integer input.
