# Print Largest of 2 Numbers

This program checks which number is larger between two numbers.

We use:

```text
if-else
```

statement to compare values.

---

## Logic

If:

```text
a > b
```

then:

```text
a is larger
```

Otherwise:

```text
b is larger
```

---

## Example Program

```java
public class JavaBasics {
    public static void main(String[] args) {

        int a = 10;
        int b = 20;

        if(a > b) {
            System.out.println("A is largest");
        }
        else {
            System.out.println("B is largest");
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

Condition:

```java
a > b
```

checks whether `a` is greater than `b`.

If condition becomes:

```text
true
```

then:

```text
A is largest
```

gets printed.

Otherwise:

```text
B is largest
```

gets printed.

---

## Another Example

```java
int a = 50;
int b = 30;
```

Output:

```text
A is largest
```
