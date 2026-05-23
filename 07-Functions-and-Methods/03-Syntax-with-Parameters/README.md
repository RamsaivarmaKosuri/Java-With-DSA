# Syntax with Parameters

Sometimes functions need:

```text
input values
```

to perform tasks.

These input values are called:

```text
Parameters
```

Parameters help functions become:

```text
dynamic
```

instead of working with fixed values.

---

## General Syntax with Parameters

```java
returnType functionName(type param1, type param2) {

    // body

    return statement;
}
```

---

## Understanding Syntax

Example:

```java
public static int calSum(int a, int b)
```

Here:

### `int`

This is:

```text
return type
```

Function will return an:

```text
integer value
```

---

### `calSum`

This is:

```text
function name
```

---

### `int a, int b`

These are:

```text
parameters
```

used to receive values.

---

## Why Parameters?

Without parameters:

function works only for:

```text
fixed values
```

But with parameters:

function can work for:

```text
different values
```

every time.

Example:

```text
2 + 3
10 + 20
50 + 100
```

using same function.

---

## Example Program

Here we take:

```text
a and b
```

from user and return:

```text
their sum
```

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

Function created:

```java
public static int Calsum(int a, int b)
```

This function receives:

```text
2 numbers
```

---

### Step 2

```java
return a + b;
```

Calculates:

```text
sum
```

and returns it.

---

### Step 3

User enters:

```java
int a = sc.nextInt();
int b = sc.nextInt();
```

---

### Step 4

Function call:

```java
Calsum(a, b);
```

sends values to function.

Example:

```text
a = 10
b = 20
```

---

### Step 5

Returned value stored in:

```java
int sum
```

Then printed.

---

## Flow of Execution

```text
User enters numbers
        ↓
Calsum(a,b) called
        ↓
Values go to parameters
        ↓
a + b calculated
        ↓
Result returned
        ↓
Printed on screen
```

---

## Your Notes

```java
// SYNTAX WITH PARAMETERS

// returnType name(type param1,type param2){
//      //body
//      return statement;
// }

// Example
// here we input a,b and return their sum

import java.util.*;

public class JavaBasics {

    public static int Calsum(int a, int b) {
        return a + b;
    }

    public static void main(String[] args) {

        Scanner sc = new Scanner(System.in);

        int a = sc.nextInt();
        int b = sc.nextInt();

        Calsum(a, b);

        System.out.println(a + b);
    }
}
```

---

## Important Note

Parameters are written:

```text
inside function definition
```

and are used to:

```text
receive values
```

Example:

```java
(int a, int b)
```
