# Calculator Using Switch Statement

This program performs basic mathematical operations using:

```text
switch statement
```

Operations:

```text
+
-
*
/
%
```

---

## Logic

User enters:

- First number
- Second number
- Operator

Program checks operator using:

```text
switch
```

and performs calculation.

---

## Example Program

```java
import java.util.*;

public class JavaBasics {
    public static void main(String[] args) {

        Scanner sc = new Scanner(System.in);

        System.out.print("Enter first number: ");
        int a = sc.nextInt();

        System.out.print("Enter second number: ");
        int b = sc.nextInt();

        System.out.print("Enter operator (+, -, *, /, %): ");
        char operator = sc.next().charAt(0);

        switch(operator) {

            case '+':
                System.out.println(a + b);
                break;

            case '-':
                System.out.println(a - b);
                break;

            case '*':
                System.out.println(a * b);
                break;

            case '/':
                System.out.println(a / b);
                break;

            case '%':
                System.out.println(a % b);
                break;

            default:
                System.out.println("Invalid Operator");

        }
    }
}
```

---

## Example Input

```text
Enter first number: 10
Enter second number: 5
Enter operator (+, -, *, /, %): +
```

## Output

```text
15
```

---

## Understanding

### `switch(operator)`

Checks operator entered by user.

Example:

```text
+
```

goes to:

```java
case '+'
```

and performs:

```java
a + b
```

---

## Why `charAt(0)`?

```java
sc.next().charAt(0)
```

is used to take a single character input.

Example:

```text
+
*
/
```

---

## Important Note

Always use:

```java
break;
```

otherwise Java executes the next cases also.
