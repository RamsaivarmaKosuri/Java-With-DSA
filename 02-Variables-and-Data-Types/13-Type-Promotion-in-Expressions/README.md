# Type Promotion in Expressions

Java automatically converts smaller datatypes while evaluating expressions.

This is called:

```text
Type Promotion
```

---

## Rule 1

Java automatically promotes:

```text
byte
short
char
```

to:

```text
int
```

while evaluating expressions.

---

## Example 1

```java
public class JavaBasics {
    public static void main(String[] args) {

        char a = 'a';
        char b = 'b';

        System.out.println(b - a);

    }
}
```

## Output

```text
1
```

---

## Understanding

Java converts characters into ASCII values.

```text
a = 97
b = 98
```

So:

```text
98 - 97 = 1
```

This is type promotion because Java automatically converted `char` into `int`.

---

## Rule 2

If one operand is:

```text
long
float
double
```

then whole expression becomes:

```text
long
float
double
```

respectively.

---

## Example 2

```java
public class JavaBasics {
    public static void main(String[] args) {

        int a = 10;
        float b = 20.25f;
        long c = 25;
        double d = 40;

        double ans = a + b + c + d;

        System.out.println(ans);

    }
}
```

## Output

```text
95.25
```

---

## Important Note

Java promotes expression to the biggest datatype present.

Example:

```text
int + float = float
int + double = double
```
