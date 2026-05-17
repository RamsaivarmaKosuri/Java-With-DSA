# Data Types in Java

## What are Data Types?

Data types tell Java what type of data will be stored in a variable.

Example:

```java
int age = 20;
```

Here `int` tells Java that only integer values can be stored.

---

## Types of Data Types

Java has **2 types of Data Types**:

### 1. Primitive Data Types

These already exist in Java.

We don't need to create them.

| Data Type | Size |
|------------|------|
| byte | 1 byte |
| short | 2 bytes |
| char | 2 bytes |
| boolean | 1 byte |
| int | 4 bytes |
| long | 8 bytes |
| float | 4 bytes |
| double | 8 bytes |

---

### 2. Non Primitive Data Types

Need to be created or used as reference types.

Examples:

```text
String
Array
Class
Object
Interface
```

---

## Example Program

```java
public class JavaBasics {
    public static void main(String[] args) {

        byte b = 8;
        System.out.println(b);

        char ch = 'a';
        System.out.println(ch);

        boolean var = true;
        System.out.println(var);

        float price = 10.5f;

        int num = 23;

        short n = 240;

    }
}
```

---

## Important Notes

### `char`

Stores only **one character**.

Correct:

```java
char ch = 'a';
```

Wrong:

```java
char ch = 'ab';
```

---

### `boolean`

Used for checking:

```text
true
false
```

---

## Memory Concept

Smaller datatype → less memory

Bigger datatype → more memory

Memory is measured in **Bytes**.

```text
1 Byte = 8 Bits
```

Bit means:

```text
0 or 1
```
