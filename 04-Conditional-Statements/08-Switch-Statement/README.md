# Switch Statement in Java

`switch` statement is used when we have multiple choices or cases.

Instead of writing many:

```text
if-else if
```

conditions, we can use:

```text
switch
```

for cleaner code.

---

## Syntax

```java
switch(variable) {

    case 1:
        // code
        break;

    case 2:
        // code
        break;

    case 3:
        // code
        break;

    default:
        // code

}
```

---

## Understanding

### `switch(variable)`

Java checks the value of the variable.

---

### `case`

Each case checks a possible value.

Example:

```java
case 1:
```

means:

```text
If variable value is 1
```

then that block executes.

---

### `break`

`break` is used to stop execution.

Without:

```java
break;
```

Java continues executing next cases also.

---

### `default`

`default` runs when no case matches.

It works like:

```text
else
```

in `if-else`.

---

## Example Program

```java
public class JavaBasics {
    public static void main(String[] args) {

        int number = 2;

        switch(number) {

            case 1:
                System.out.println("One");
                break;

            case 2:
                System.out.println("Two");
                break;

            case 3:
                System.out.println("Three");
                break;

            default:
                System.out.println("Invalid Number");

        }

    }
}
```

## Output

```text
Two
```

---

## Another Example

```java
int number = 5;
```

## Output

```text
Invalid Number
```

because no case matched.

---

## Your Notes

```java
switch(variable){

    case 1:

    case 2:

    case 3:

    default:

}
```

We use:

```java
break;
```

to stop execution after each case.

---

## Important Note

`switch` works best when checking:

```text
multiple fixed values
```
