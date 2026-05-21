# Print Reverse of a Number

This program prints the digits of a number in:

```text
reverse order
```

using:

```text
while loop
```

---

## Example

Given number:

```text
10899
```

Reverse printing:

```text
99801
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

and:

```text
/
```

to remove the last digit.

---

## Example Understanding

For number:

```text
10899
```

### Step 1

```java
10899 % 10
```

Output:

```text
9
```

(last digit)

Then:

```java
10899 / 10
```

becomes:

```text
1089
```

---

### Step 2

```java
1089 % 10
```

Output:

```text
9
```

Then:

```java
1089 / 10
```

becomes:

```text
108
```

This process continues until:

```text
number becomes 0
```

---

## Example Program

```java
public class JavaBasics {
    public static void main(String[] args) {

        int n = 10899;

        while(n > 0) {

            int lastDigit = n % 10;

            System.out.print(lastDigit);

            n = n / 10;
        }

    }
}
```

## Output

```text
99801
```

---

## Code Understanding

### Step 1

```java
int n = 10899;
```

We take a number.

---

### Step 2

Condition:

```java
n > 0
```

Loop runs until number becomes:

```text
0
```

---

### Step 3

```java
int lastDigit = n % 10;
```

Gets the:

```text
last digit
```

Example:

```text
10899 % 10 = 9
```

---

### Step 4

```java
System.out.print(lastDigit);
```

Prints digit.

---

### Step 5

```java
n = n / 10;
```

Removes last digit.

Example:

```text
10899 → 1089
1089 → 108
108 → 10
10 → 1
1 → 0
```

Loop stops when:

```text
n = 0
```

---

## Dry Run

```text
n = 10899 → print 9
n = 1089 → print 9
n = 108 → print 8
n = 10 → print 0
n = 1 → print 1
n = 0 → stop
```

---

## Your Notes

```java
public class JavaBasics {
    public static void main(String[] args) {

        int n = 10899;

        while(n > 0) {

            int lastdigit = n % 10;
            System.out.print(lastdigit);

            n = n / 10;
        }
    }
}
```

---

## Important Note

```text
%
```

gives:

```text
last digit
```

and

```text
/
```

removes:

```text
last digit
```
