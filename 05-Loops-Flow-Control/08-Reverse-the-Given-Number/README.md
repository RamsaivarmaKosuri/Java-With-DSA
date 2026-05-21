# Reverse the Given Number

This program reverses a number and stores it in another variable.

Unlike:

```text
Print Reverse of a Number
```

here we create a new reversed number using:

```text
rev
```

variable.

---

## Example

Given number:

```text
10898
```

Reversed number:

```text
89801
```

---

## Logic

We use:

```text
%
```

to get the:

```text
last digit
```

Then build reverse number using:

```java
rev = (rev * 10) + lastDigit
```

---

## Example Understanding

Suppose:

```text
n = 10898
```

Initially:

```text
rev = 0
```

### Step 1

Last digit:

```text
10898 % 10 = 8
```

Formula:

```java
rev = (0 * 10) + 8
```

Output:

```text
8
```

---

### Step 2

Remaining number:

```text
1089
```

Last digit:

```text
9
```

Formula:

```java
rev = (8 * 10) + 9
```

Output:

```text
89
```

---

### Step 3

Continue same process:

```text
89 → 898 → 8980 → 89801
```

---

## Example Program

```java
public class JavaBasics {
    public static void main(String[] args) {

        int n = 10898;
        int rev = 0;

        while(n > 0) {

            int lastDigit = n % 10;

            rev = (rev * 10) + lastDigit;

            n = n / 10;
        }

        System.out.print(rev);

    }
}
```

## Output

```text
89801
```

---

## Code Understanding

### Step 1

```java
int rev = 0;
```

Used to store reversed number.

Initially:

```text
0
```

---

### Step 2

```java
int lastDigit = n % 10;
```

Gets last digit.

Example:

```text
10898 % 10 = 8
```

---

### Step 3

```java
rev = (rev * 10) + lastDigit;
```

Builds reversed number.

Example:

```text
0 → 8 → 89 → 898 → 8980 → 89801
```

---

### Step 4

```java
n = n / 10;
```

Removes last digit.

Example:

```text
10898 → 1089 → 108 → 10 → 1 → 0
```

Loop stops when:

```text
n = 0
```

---

## Dry Run

```text
n = 10898

rev = 0

lastDigit = 8 → rev = 8
lastDigit = 9 → rev = 89
lastDigit = 8 → rev = 898
lastDigit = 0 → rev = 8980
lastDigit = 1 → rev = 89801
```

---

## Your Notes

```java
public class JavaBasics {
    public static void main(String[] args) {

        int n = 10898;
        int rev = 0;

        while(n > 0) {

            int lastdigit = n % 10;

            rev = (rev * 10) + lastdigit;

            n = n / 10;
        }

        System.out.print(rev);
    }
}
```

---

## Important Note

```text
Print Reverse
```

only prints digits.

But:

```text
Reverse Number
```

stores reversed value in:

```text
rev variable
```
