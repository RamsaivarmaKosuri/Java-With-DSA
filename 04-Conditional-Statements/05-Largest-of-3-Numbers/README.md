# Print Largest of 3 Numbers

This program checks which number is the largest among three numbers.

We use:

```text
if - else if - else
```

statement.

---

## Logic

If:

```text
a > b && a > c
```

then:

```text
a is largest
```

Else if:

```text
b > c
```

then:

```text
b is largest
```

Otherwise:

```text
c is largest
```

---

## Example Program

```java
public class JavaBasics {
    public static void main(String[] args) {

        int a = 10;
        int b = 20;
        int c = 15;

        if(a > b && a > c) {
            System.out.println("A is largest");
        }
        else if(b > c) {
            System.out.println("B is largest");
        }
        else {
            System.out.println("C is largest");
        }

    }
}
```

## Output

```text
B is largest
```

---

## Understanding

### First Condition

```java
a > b && a > c
```

Checks whether `a` is greater than both `b` and `c`.

Result:

```text
false
```

So Java moves to next condition.

---

### Second Condition

```java
b > c
```

Checks whether `b` is greater than `c`.

Result:

```text
true
```

So:

```text
B is largest
```

gets printed.

---

## Another Example

```java
a = 50
b = 30
c = 20
```

## Output

```text
A is largest
```

---

## Important Note

We use:

```text
&& (Logical AND)
```

to check multiple conditions together.
