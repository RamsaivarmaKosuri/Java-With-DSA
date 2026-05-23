# Parameters vs Arguments

Many beginners get confused between:

```text
Parameters
```

and:

```text
Arguments
```

But understanding this is actually:

```text
very easy
```

---

## Simple Difference

### Parameters

Values written inside:

```text
function definition
```

are called:

```text
Parameters
```

Also called:

```text
Formal Parameters
```

---

### Arguments

Values passed during:

```text
function call
```

are called:

```text
Arguments
```

Also called:

```text
Actual Parameters
```

---

## Syntax Understanding

```java
public static int Calsum(int a, int b)
```

Here:

```java
int a, int b
```

are:

```text
Parameters
```

because they are written in:

```text
function definition
```

---

Now:

```java
Calsum(a, b);
```

Here:

```java
a, b
```

are:

```text
Arguments
```

because values are passed during:

```text
function call
```

---

## Example Program

```java
import java.util.*;

public class JavaBasics {

    public static int Calsum(int a, int b) {

        return a + b;

    }

    public static void main(String[] args) {

        Scanner sc = new Scanner(System.in);

        int a = sc.nextInt();
        int b = sc.nextInt();

        int sum = Calsum(a, b);

        System.out.println(sum);

    }
}
```

## Example Input

```text
10
20
```

## Output

```text
30
```

---

## Code Understanding

### Step 1

Function Definition:

```java
public static int Calsum(int a, int b)
```

Here:

```java
int a, int b
```

are:

```text
Parameters (Formal Parameters)
```

because function is:

```text
receiving values
```

---

### Step 2

User enters:

```text
10
20
```

stored in:

```java
a = 10
b = 20
```

---

### Step 3

Function call:

```java
Calsum(a, b);
```

passes values to function.

These passed values are called:

```text
Arguments (Actual Parameters)
```

---

### Step 4

Function receives values:

```text
10 and 20
```

then calculates:

```text
10 + 20 = 30
```

and returns answer.

---

## Visual Understanding

```text
Function Definition
        ↓
Calsum(int a, int b)
        ↓
     Parameters


Function Call
        ↓
Calsum(10, 20)
        ↓
     Arguments
```

---

## Easy Trick to Remember

### Parameters

```text
P = Placeholders
```

They wait for values.

---

### Arguments

```text
A = Actual Values
```

They send real data.

---

## Your Notes

```java
// PARAMETERS VS ARGUMENTS

// jo parameters hum function ki definition me likhte hai
// usko parameters or formal parameters kehte hai

// jo value calling statement or function call ke time use karte
// usko arguments or actual parameters kehte hai

import java.util.*;

public class JavaBasics {

    public static int Calsum(int a, int b) {

        // parameters or formal parameters

        return a + b;
    }

    public static void main(String[] args) {

        Scanner sc = new Scanner(System.in);

        int a = sc.nextInt();
        int b = sc.nextInt();

        Calsum(a, b);

        // arguments or actual parameters

        System.out.println(a + b);
    }
}
```

---

## Important Note

```text
Function Definition → Parameters

Function Call → Arguments
```

This is one of the:

```text
most asked beginner interview concepts
```
