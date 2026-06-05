# Code - Binary to Decimal

In the previous topic, we learned the mathematical logic behind Binary to Decimal conversion.

Now let's implement the same logic using Java.

---

## Program

```java
public class JavaBasics {

    public static void binNum(int n){

        int number = n;
        int power = 0;
        int decNum = 0;

        while(n > 0){

            int lastdigit = n % 10;

            decNum = decNum + (lastdigit * (int)Math.pow(2, power));

            power++;

            n = n / 10;
        }

        System.out.println("The Decimal number of " + number + " is :" + decNum);
    }

    public static void main(String[] args) {

        binNum(111);

    }
}
```

---

## Output

```text
The Decimal number of 111 is :7
```

---

## How the Logic Works

Input:

```text
111
```

Initially:

```text
number = 111
power = 0
decNum = 0
```

The algorithm:

```text
1. Take the last digit.
2. Multiply it with 2^power.
3. Add the result to decNum.
4. Increase power.
5. Remove the last digit.
6. Repeat until n becomes 0.
```

---

## Dry Run Table

Input:

```text
n = 111
```

| Iteration | n | Last Digit (n % 10) | Power | Calculation | decNum |
|------------|-----|------------|--------|-------------|--------|
| Start | 111 | - | 0 | - | 0 |
| 1 | 111 | 1 | 0 | 1 × 2⁰ = 1 | 1 |
| 2 | 11 | 1 | 1 | 1 × 2¹ = 2 | 3 |
| 3 | 1 | 1 | 2 | 1 × 2² = 4 | 7 |

Loop ends because:

```text
n = 0
```

Final Answer:

```text
7
```

---

## Variable Flow

### Iteration 1

```text
n = 111

lastdigit = 1

decNum = 0 + (1 × 2⁰)

decNum = 1
```

Update:

```text
power = 1

n = 11
```

---

### Iteration 2

```text
n = 11

lastdigit = 1

decNum = 1 + (1 × 2¹)

decNum = 3
```

Update:

```text
power = 2

n = 1
```

---

### Iteration 3

```text
n = 1

lastdigit = 1

decNum = 3 + (1 × 2²)

decNum = 7
```

Update:

```text
power = 3

n = 0
```

Loop Stops.

---

## Visual Representation

```text
111

1 × 2⁰ = 1
        ↓

1 × 2¹ = 2
        ↓

1 × 2² = 4
        ↓

1 + 2 + 4
        ↓

7
```

---

## Understanding Variables

| Variable | Purpose |
|-----------|---------|
| number | Stores original binary number |
| power | Stores current power of 2 |
| lastdigit | Extracts last binary digit |
| decNum | Stores decimal answer |

---

## Time Complexity

```text
O(number of digits)
```

For a binary number containing `d` digits:

```text
O(d)
```

---

## Key Learning

- Extract digits using `% 10`.
- Remove digits using `/ 10`.
- Use `Math.pow()` to calculate powers of 2.
- Build the decimal number step by step.
- Convert Binary to Decimal efficiently using loops.

---

## Special Note

From my notes:

```java
int lastdigit = n % 10;

decNum = decNum +
(lastdigit * (int)Math.pow(2,power));

power++;

n = n / 10;
```

The key idea is:

```text
Last Digit
     ↓
Multiply with 2^power
     ↓
Add to Decimal Number
     ↓
Increase Power
     ↓
Move to Next Digit
```

This is exactly the same logic used in the mathematical Binary to Decimal conversion.
