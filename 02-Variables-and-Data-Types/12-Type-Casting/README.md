# Type Casting in Java

Type Casting is also called:

- Narrowing Conversion
- Explicit Casting

In Type Casting, Java converts a **bigger datatype into a smaller datatype manually**.

## Why Do We Need Type Casting?

Sometimes we want to store a bigger datatype into a smaller datatype.

Example:

```text
float → int
double → int
long → int
```

Java does not do this automatically.

So we use **Type Casting**.

---

## Example Program

```java
public class JavaBasics {
    public static void main(String[] args) {

        float number = 99.8989f;

        int number2 = (int) number;

        System.out.println(number2);

    }
}
```

## Output

```text
99
```

---

## Understanding

```java
(int) number
```

This converts float into integer.

Since `int` cannot store decimal values:

```text
99.8989 → 99
```

Decimal part gets removed.

---

## Important Note

Type Casting happens when:

```text
Bigger datatype → Smaller datatype
```

Example:

```text
float → int
double → int
long → int
```

This is called:

```text
Narrowing Conversion
```
