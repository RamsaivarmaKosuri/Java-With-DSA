# Relational Operators

Relational operators are used to compare two values.

The result always comes in:

```text
true
false
```

---

## Types of Relational Operators

```text
==
!=
>
<
>=
<=
```

---

## 1. Equal To `==`

Checks whether two values are equal.

Example:

```java
System.out.println(5 == 5);
```

## Output

```text
true
```

---

## 2. Not Equal To `!=`

Checks whether values are different.

Example:

```java
System.out.println(5 != 10);
```

## Output

```text
true
```

---

## 3. Greater Than `>`

Checks whether left value is greater.

Example:

```java
System.out.println(10 > 5);
```

## Output

```text
true
```

---

## 4. Less Than `<`

Checks whether left value is smaller.

Example:

```java
System.out.println(5 < 10);
```

## Output

```text
true
```

---

## 5. Greater Than or Equal To `>=`

Example:

```java
System.out.println(10 >= 10);
```

## Output

```text
true
```

---

## 6. Less Than or Equal To `<=`

Example:

```java
System.out.println(5 <= 10);
```

## Output

```text
true
```

---

## Complete Example Program

```java
public class JavaBasics {
    public static void main(String[] args) {

        int a = 10;
        int b = 5;

        System.out.println(a == b);
        System.out.println(a != b);
        System.out.println(a > b);
        System.out.println(a < b);
        System.out.println(a >= b);
        System.out.println(a <= b);

    }
}
```

## Output

```text
false
true
true
false
true
false
```

## Important Note

Relational operators are mostly used in:

```text
Conditions
if-else
loops
```
