# Check Pass or Fail Using Ternary Operator

This program checks whether a student is:

```text
Pass
```

or

```text
Fail
```

using:

```text
Ternary Operator
```

---

## Logic

If marks are:

```text
greater than or equal to 33
```

student is:

```text
Pass
```

Otherwise:

```text
Fail
```

---

## Example Program

```java
public class JavaBasics {
    public static void main(String[] args) {

        int marks = 75;

        String result = (marks >= 33) ? "PASS" : "FAIL";

        System.out.println(result);

    }
}
```

## Output

```text
PASS
```

---

## Another Example

```java
int marks = 20;
```

## Output

```text
FAIL
```

---

## Understanding

Condition:

```java
marks >= 33
```

If condition becomes:

```text
true
```

then:

```text
"PASS"
```

gets selected.

Otherwise:

```text
"FAIL"
```

gets selected.

---

## Ternary Syntax Used

```java
variable = (condition) ? statement1 : statement2;
```

In this example:

```java
String result = (marks >= 33) ? "PASS" : "FAIL";
```

---

## Important Note

Ternary operator helps write:

```text
if-else
```

in a shorter and cleaner way.
