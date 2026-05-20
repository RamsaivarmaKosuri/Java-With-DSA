# Arithmetic Operators

Arithmetic operators are used to perform mathematical operations.

## Types of Arithmetic Operators

### 1. Binary Operators

Binary operators need **two operands**.

Operators:

```text
+
-
*
/
%
```

### Example Program

```java
public class JavaBasics {
    public static void main(String[] args) {

        int a = 10;
        int b = 5;

        System.out.println(a + b);
        System.out.println(a - b);
        System.out.println(a * b);
        System.out.println(a / b);
        System.out.println(a % b);

    }
}
```

## Output

```text
15
5
50
2
0
```

---

## Understanding `%` (Modulus)

`%` gives the **remainder**.

Example:

```text
10 % 3 = 1
```

---

## 2. Unary Operators

Unary operators work on only **one operand**.

Operators:

```text
++
--
```

Example:

```java
int a = 10;
a++;

System.out.println(a);
```

Output:

```text
11
```
