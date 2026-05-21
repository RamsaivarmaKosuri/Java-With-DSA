# If Else in Java

`if-else` statement is used to make decisions.

It checks a condition.

If condition is:

```text
true
```

then `if` block executes.

Otherwise:

```text
else
```

block executes.

---

## Syntax

```java
if(condition) {

    // code executes if condition is true

}
else {

    // code executes if condition is false

}
```

---

## Example Program

```java
public class JavaBasics {
    public static void main(String[] args) {

        int age = 18;

        if(age >= 18) {
            System.out.println("Adult");
        }
        else {
            System.out.println("Not Adult");
        }

    }
}
```

## Output

```text
Adult
```

---

## Understanding

Condition:

```java
age >= 18
```

checks whether age is greater than or equal to `18`.

If condition is:

```text
true
```

prints:

```text
Adult
```

Otherwise prints:

```text
Not Adult
```

---

## Important Note

`if` works when condition is:

```text
true
```

`else` executes when condition becomes:

```text
false
```
