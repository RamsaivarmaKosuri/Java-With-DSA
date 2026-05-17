# Variables in Java

## What are Variables?

Variables are containers used to store data.

When a variable is created, memory is reserved for it and value is stored inside it.

Each memory block has its own memory address.

We can also change variable values later.

## Java has Two Units

1. Literals → Fixed values

Example:

```java
10
20
"Hello"
true
```

2. Variables → Values stored using names

Example:

```java
int age = 20;
```

Here:
- `int` → datatype
- `age` → variable name
- `20` → value

## Example Program

```java
public class JavaBasics {
    public static void main(String[] args) {

        int age = 20;

        System.out.println(age);

    }
}
```

## Variable Rules (Identifiers)

Variable names are called **Identifiers** in Java.

Identifiers can start with:

- alphabet (`a-z`, `A-Z`)
- underscore (`_`)
- dollar (`$`)

Correct:

```java
age
_age
$salary
```

Wrong:

```java
1age
@name
```

## Important Note

Variable values can be changed.

Example:

```java
int age = 20;
age = 25;
```
