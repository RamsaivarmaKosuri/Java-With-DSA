# Input in Java

## What is Input?

Input means taking data from the user.

In Java, we use **Scanner class** to take input.

---

## Step 1: Import Scanner

```java
import java.util.*;
```

This imports Scanner.

---

## Step 2: Create Scanner Object

```java
Scanner sc = new Scanner(System.in);
```

Here:

- `Scanner` → class name
- `sc` → object name
- `System.in` → takes input from keyboard

---

## Different Input Methods

| Method | Use |
|--------|-----|
| `next()` | Reads only one word |
| `nextLine()` | Reads complete line |
| `nextInt()` | Integer input |
| `nextFloat()` | Float input |
| `nextDouble()` | Double input |
| `nextBoolean()` | Boolean input |
| `nextByte()` | Byte input |
| `nextShort()` | Short input |
| `nextLong()` | Long input |

---

## Example Program

```java
import java.util.*;

public class JavaBasics {
    public static void main(String[] args) {

        Scanner sc = new Scanner(System.in);

        String input = sc.next();
        System.out.println(input);

        String name = sc.nextLine();
        System.out.println(name);

        int num = sc.nextInt();
        System.out.println(num);

        float price = sc.nextFloat();
        System.out.println(price);

    }
}
```

---

## Important Difference

### `next()`

Reads only **one word**.

Example Input:

```text
Ram Sai
```

Output:

```text
Ram
```

---

### `nextLine()`

Reads the **entire sentence**.

Example Input:

```text
Ram Sai
```

Output:

```text
Ram Sai
```

## Important Note

To take input in Java, we mostly use:

```java
Scanner sc = new Scanner(System.in);
```
