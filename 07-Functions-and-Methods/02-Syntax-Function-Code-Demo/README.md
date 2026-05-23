# Syntax - Function Code Demo

Before creating functions, we must understand:

```text
function syntax
```

Every function in Java follows a:

```text
specific structure
```

---

## General Syntax of Function

```java
returnType functionName() {

    // body

    return statement;
}
```

---

## Understanding Function Syntax

A function mainly contains:

```text
1. Return Type
2. Function Name
3. Parentheses ()
4. Function Body
5. Return Statement
```

---

## Syntax Breakdown

### 1. Return Type

The:

```text
return type
```

tells Java:

```text
what value function returns
```

Example:

```java
int
float
double
boolean
char
void
```

---

### 2. Function Name

This is the:

```text
name of function
```

used to call it later.

Example:

```java
printHello()
calculateSum()
findAverage()
```

---

### 3. Parentheses `()`

Used for:

```text
parameters
```

If no parameters exist:

we keep:

```java
()
```

empty.

---

### 4. Function Body

The code inside:

```java
{ }
```

is called:

```text
function body
```

This contains:

```text
actual logic
```

of program.

---

### 5. Return Statement

Used to:

```text
return value
```

from function.

Example:

```java
return sum;
```

---

## Example Understanding

```java
public static void printHello() {

    System.out.println("hello");

    return;
}
```

### Breaking It Down

```java
public
```

Means:

```text
function is accessible
```

---

```java
static
```

Means:

```text
function can be called directly
```

without creating object.

---

```java
void
```

Means:

```text
nothing is returned
```

(khali)

---

```java
printHello()
```

This is:

```text
function name
```

---

```java
{
    System.out.println("hello");
}
```

This is:

```text
function body
```

---

## Main Function Example

```java
public class JavaBasics {
    public static void main(String[] args) {

        // here main is a function

    }
}
```

### Understanding Main Function

```java
public static void main(String[] args)
```

is also a:

```text
function
```

Here:

```java
void
```

means:

```text
main function returns nothing
```

---

## Example Program

```java
public class JavaBasics {

    public static void printHello() {

        System.out.println("Hello");

        return;
    }

    public static void main(String[] args) {

        printHello();

    }
}
```

## Output

```text
Hello
```

---

## Flow of Execution

```text
Program Starts
       ↓
main() function executes
       ↓
printHello() called
       ↓
hello printed
       ↓
function ends
```

---

## Your Notes

```java
// SYNTAX - FUNCTION CODE DEMO

// returnType name(){
//      //body
//      return statement;
// }

public class JavaBasics {
    public static void main(String[] args) {

        // here main is a function

        // its return type is void

        // void means khali

        // function kuch return nahi karta
    }
}
```

---

## Important Note

If function return type is:

```java
void
```

then:

```text
return statement is optional
```

But if return type is:

```java
int, float, double, boolean
```

then:

```text
return is compulsory
```

otherwise:

```text
error occurs
```
