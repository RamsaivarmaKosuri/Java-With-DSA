# Cost of 3 Items from User

## Problem Statement

Take the cost of:

- Pencil
- Pen
- Eraser

from the user and print the total bill.

**Add-on:** Add 18% GST to the total bill.

---

## Example Program

```java
import java.util.*;

public class JavaBasics {
    public static void main(String[] args) {

        Scanner sc = new Scanner(System.in);

        float pencil = sc.nextFloat();
        float pen = sc.nextFloat();
        float eraser = sc.nextFloat();

        float total = pencil + pen + eraser;

        System.out.println("THE BILL IS : " + total);

        float gst = total + (0.18f * total);

        System.out.println("AFTER GST : " + gst);
    }
}
```

---

## Example Input

```text
10
20
5
```

## Output

```text
THE BILL IS : 35.0
AFTER GST : 41.3
```

---

## Understanding

### Take Input

```java
float pencil = sc.nextFloat();
float pen = sc.nextFloat();
float eraser = sc.nextFloat();
```

Takes prices from user.

---

### Calculate Total

```java
float total = pencil + pen + eraser;
```

Adds all item costs.

---

### Add GST

```java
0.18f * total
```

Calculates **18% GST**.

---

## Why Float?

We use:

```java
float
```

because prices can contain decimal values.

Example:

```text
10.50
20.75
```
