# Code - Decimal to Binary

In the previous topic, we learned the mathematical logic behind Decimal to Binary conversion.

Now let's implement the same logic using Java.

---

## Program

```java
public class JavaBasics{

    public static void decNum(int n){

        int number = n;
        int power = 0;
        int binNum = 0;

        while(n > 0){

            int lastdigit = n % 2;

            binNum = binNum +
                     (lastdigit * (int)Math.pow(10,power));

            power++;

            n = n / 2;
        }

        System.out.println("The Binary number of " +
                           number +
                           " is :" +
                           binNum);
    }

    public static void main(String[] args) {

        decNum(5);

    }
}
```

---

## Output

```text
The Binary number of 5 is :101
```

---

## How the Logic Works

Input:

```text
5
```

Initially:

```text
number = 5

power = 0

binNum = 0
```

Algorithm:

```text
1. Divide number by 2.
2. Store remainder.
3. Multiply remainder with 10^power.
4. Add to Binary Number.
5. Increase power.
6. Continue until n becomes 0.
```

---

## Dry Run Table

Input:

```text
n = 5
```

| Iteration | n | Remainder (n%2) | Power | Calculation | binNum |
|------------|---|----------------|--------|-------------|---------|
| Start | 5 | - | 0 | - | 0 |
| 1 | 5 | 1 | 0 | 1 × 10⁰ = 1 | 1 |
| 2 | 2 | 0 | 1 | 0 × 10¹ = 0 | 1 |
| 3 | 1 | 1 | 2 | 1 × 10² = 100 | 101 |

Loop ends because:

```text
n = 0
```

Final Answer:

```text
101
```

---

## Variable Flow

### Iteration 1

```text
n = 5

remainder = 5 % 2

remainder = 1

binNum = 0 + (1 × 10⁰)

binNum = 1
```

Update:

```text
power = 1

n = 2
```

---

### Iteration 2

```text
n = 2

remainder = 0

binNum = 1 + (0 × 10¹)

binNum = 1
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

remainder = 1

binNum = 1 + (1 × 10²)

binNum = 101
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
5 ÷ 2 = 2 remainder 1

2 ÷ 2 = 1 remainder 0

1 ÷ 2 = 0 remainder 1


Read Bottom to Top

1 0 1

Binary = 101
```

---

## Understanding Variables

| Variable | Purpose |
|-----------|---------|
| number | Stores original decimal number |
| power | Stores current power of 10 |
| lastdigit | Stores remainder after division by 2 |
| binNum | Stores binary answer |

---

## Time Complexity

```text
O(log₂ n)
```

Because the number is repeatedly divided by 2.

---

## Easy Remembering Trick

### Binary → Decimal

Think:

```text
Take Digit
      ↓
Multiply by Power of 2
      ↓
Add to Decimal
```

Formula:

```java
decNum = decNum +
         (lastdigit * 2^power)
```

---

### Decimal → Binary

Think:

```text
Take Remainder
       ↓
Multiply by Power of 10
       ↓
Add to Binary
```

Formula:

```java
binNum = binNum +
         (remainder * 10^power)
```

---

## Difference Between Both Programs

| Binary to Decimal | Decimal to Binary |
|------------------|-------------------|
| Extract digit using `% 10` | Extract remainder using `% 2` |
| Divide by 10 | Divide by 2 |
| Multiply by `2^power` | Multiply by `10^power` |
| Build Decimal Number | Build Binary Number |
| Input = Binary | Input = Decimal |

---

## Comparison Diagram

```text
BINARY → DECIMAL

101

Take Digit
    ↓
Multiply by 2^power
    ↓
Add
    ↓
5


DECIMAL → BINARY

5

Take Remainder
    ↓
Multiply by 10^power
    ↓
Add
    ↓
101
```

---

## Key Learning

- Use `% 2` to get binary digits.
- Use `/ 2` to move to the next step.
- Binary digits are stored using powers of 10.
- Decimal to Binary is the reverse process of Binary to Decimal.
- Understanding both conversions strengthens number system concepts.

---

## Special Note

From my notes:

```java
while(n > 0){

    int lastdigit = n % 2;

    binNum = binNum +
             (lastdigit *
             (int)Math.pow(10,power));

    power++;

    n = n/2;
}
```

### Quick Memory Hack

```text
Binary → Decimal

%10
÷10
2^power


Decimal → Binary

%2
÷2
10^power
```

If you remember this pattern, you can easily write both programs in an interview without memorizing the complete code.
