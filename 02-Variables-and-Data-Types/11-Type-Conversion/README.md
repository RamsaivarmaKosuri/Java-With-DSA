# Type Conversion in Java

Type Conversion is also called:

- Implicit Conversion
- Widening Conversion

It means Java automatically converts one datatype into another datatype.

---

## When Type Conversion Happens?

Type conversion happens when:

### 1. Types are Compatible

Example:

```java
int
float
double
```

These numeric datatypes are compatible.

---

### 2. Destination Type > Source Type

The destination datatype should have bigger size than source datatype.

Example:

```java
int a = 25;
long b = a;
```

Here:

```text
int → long
```

Java automatically converts it.

---

## Flow of Type Conversion

```text
byte → short → int → float → long → double
```

Smaller datatype converts into bigger datatype.

---

## Example Program

```java
public class JavaBasics {
    public static void main(String[] args) {

        int a = 25;
        long b = a;

        System.out.println(b);

    }
}
```

## Output

```text
25
```

---

## Example 2

```java
public class JavaBasics {
    public static void main(String[] args) {

        char ch = 'a';
        int number = ch;

        System.out.println(number);

    }
}
```

## Output

```text
97
```

Because Java converts character into ASCII value.

---

## Important Note

Type conversion happens automatically only when:

```text
Destination type > Source type
```

Example:

```text
int → long ✅
float → double ✅
```

Wrong:

```text
long → int ❌
double → float ❌
```

This gives error because smaller datatype cannot hold bigger data.
