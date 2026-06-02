# Sum of Even and Odd Numbers

In this problem, we take:

```text
n integers
```

from the user and calculate:

- Sum of all even numbers
- Sum of all odd numbers

This problem helps us understand:

```text
Loops + Conditions + Variables + User Input
```

---

## Problem Statement

Take:

```text
n integers
```

from the user.

Calculate:

```text
Sum of Even Numbers
Sum of Odd Numbers
```

and print the result.

---

## Approach

1. Take the number of integers from the user.
2. Run a loop `n` times.
3. Take each number as input.
4. Check whether the number is even or odd.
5. Add even numbers to the even sum.
6. Add odd numbers to the odd sum.
7. Print both sums.

---

## Program

```java
import java.util.*;

public class JavaBasics {
    public static void main(String[] args) {

        int even = 0;
        int odd = 0;

        Scanner sc = new Scanner(System.in);

        System.out.println("ENTER THE NUMBER OF INTEGERS :");
        int n = sc.nextInt();

        System.out.println("ENTER " + n + " INTEGERS :");

        for(int i = 0; i < n; i++) {

            int num = sc.nextInt();

            if(num % 2 == 0) {
                even = even + num;
            }
            else {
                odd = odd + num;
            }
        }

        System.out.println("EVEN SUM : " + even);
        System.out.println("ODD SUM : " + odd);
    }
}
```

---

## Example Input

```text
5
1
2
3
4
5
```

---

## Output

```text
EVEN SUM : 6
ODD SUM : 9
```

---

## Code Explanation

### Step 1

Create two variables:

```java
int even = 0;
int odd = 0;
```

These variables store:

```text
sum of even numbers
sum of odd numbers
```

---

### Step 2

Take:

```java
int n = sc.nextInt();
```

Number of integers to be entered.

---

### Step 3

Run loop:

```java
for(int i = 0; i < n; i++)
```

This loop runs:

```text
n times
```

---

### Step 4

Take input:

```java
int num = sc.nextInt();
```

---

### Step 5

Check:

```java
num % 2 == 0
```

If true:

```text
Number is Even
```

Otherwise:

```text
Number is Odd
```

---

### Step 6

Update sums:

```java
even = even + num;
```

or

```java
odd = odd + num;
```

---

## Dry Run

```text
Input:

1 2 3 4 5

even = 0
odd = 0

Number = 1
odd = 0 + 1 = 1

Number = 2
even = 0 + 2 = 2

Number = 3
odd = 1 + 3 = 4

Number = 4
even = 2 + 4 = 6

Number = 5
odd = 4 + 5 = 9

Final Output:

EVEN SUM = 6
ODD SUM = 9
```

---

## Flow Diagram

```text
User Enters n
        ↓
Loop Runs n Times
        ↓
Take Number
        ↓
Even ?
   ↙       ↘
 Yes       No
  ↓         ↓
Add to    Add to
Even Sum  Odd Sum
    ↓
Print Results
```

---

## Your Notes

```java
import java.util.*;

public class JavaBasics {
    public static void main(String[] args) {

        int even = 0;
        int odd = 0;

        Scanner sc = new Scanner(System.in);

        System.out.println("ENTER THE NUMBER OF INTEGERS :");

        int n = sc.nextInt();

        System.out.println("ENTER " + n + " INTEGERS :");

        for(int i = 0; i < n; i++) {

            int num = sc.nextInt();

            if(num % 2 == 0) {
                even = even + num;
            }
            else {
                odd = odd + num;
            }
        }

        System.out.println("EVEN SUM :" + even);
        System.out.println("ODD SUM : " + odd);
    }
}
```

---

## Key Learning

```text
Using Loops
Using Conditions
User Input Handling
Maintaining Multiple Sums
Problem Solving with Loops
```
