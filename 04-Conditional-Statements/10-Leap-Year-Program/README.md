# Leap Year Program

This program checks whether a given year is:

```text
Leap Year
```

or

```text
Not a Leap Year
```

using:

```text
if-else statement
```

---

## Logic of Leap Year

A year is a leap year if:

### Condition 1

Year is divisible by:

```text
4
```

AND not divisible by:

```text
100
```

OR

### Condition 2

Year is divisible by:

```text
400
```

---

## Formula Used

```java
(year % 4 == 0 && year % 100 != 0) || (year % 400 == 0)
```

---

## Example Program

```java
import java.util.*;

public class JavaBasics {
    public static void main(String[] args) {

        Scanner sc = new Scanner(System.in);

        System.out.print("Enter year: ");
        int year = sc.nextInt();

        if((year % 4 == 0 && year % 100 != 0) || (year % 400 == 0)) {
            System.out.println(year + " is leap year");
        }
        else {
            System.out.println(year + " is not leap year");
        }

    }
}
```

---

## Example Input

```text
2024
```

## Output

```text
2024 is leap year
```

---

## Another Example

### Input

```text
2023
```

### Output

```text
2023 is not leap year
```

---

## Understanding

Example:

```text
2024
```

### Check 1

```text
2024 % 4 == 0
```

✔ True

### Check 2

```text
2024 % 100 != 0
```

✔ True

So:

```text
Leap Year
```

---

## Your Notes

```java
if((year%4==0 && year%100!=0) || (year%400==0)){
    System.out.println(year +"is leap year");
}
else{
    System.out.println(year +"is not leap year");
}
```

---

## Important Note

We use:

```text
&& (AND)
|| (OR)
```

to combine multiple conditions.
