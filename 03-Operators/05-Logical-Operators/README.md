# Logical Operators

Logical operators are used to combine conditions.

The answer always comes in:

```text
true
false
```

## Types of Logical Operators

```text
&&  → Logical AND
||  → Logical OR
!   → Logical NOT
```

---

# 1. Logical AND `&&`

Returns:

```text
true
```

only when **both conditions are true**.

## Truth Table

| st1 | st2 | Ans |
|------|------|-----|
| T | T | T |
| T | F | F |
| F | T | F |
| F | F | F |

### Example Program

```java
public class JavaBasics {
    public static void main(String[] args) {

        System.out.println((5 > 3) && (10 > 5));

    }
}
```

## Output

```text
true
```

Because both conditions are true.

---

# 2. Logical OR `||`

Returns:

```text
false
```

only when **both conditions are false**.

## Truth Table

| st1 | st2 | Ans |
|------|------|-----|
| T | T | T |
| T | F | T |
| F | T | T |
| F | F | F |

### Example Program

```java
public class JavaBasics {
    public static void main(String[] args) {

        System.out.println((5 > 10) || (10 > 5));

    }
}
```

## Output

```text
true
```

Because one condition is true.

---

# 3. Logical NOT `!`

Logical NOT reverses the result.

```text
true → false
false → true
```

## Truth Table

| st1 | Ans |
|------|-----|
| T | F |
| F | T |

### Example Program

```java
public class JavaBasics {
    public static void main(String[] args) {

        System.out.println(!(5 > 3));

    }
}
```

## Output

```text
false
```

Because:

```text
5 > 3 = true
```

then NOT reverses it:

```text
true → false
```

---

## Important Note

Logical operators are mostly used in:

```text
if-else
loops
conditions
```
