# Inverted Half Pyramid with Numbers

This pattern is a number-based variation of the Inverted Half Pyramid.

Instead of printing stars (`*`), we print numbers.

This pattern helps in understanding:

- Nested Loops
- Number Patterns
- Row and Column Relationships
- Pattern Visualization

---

## Pattern Output

For:

```java
inverted_half_pyramid_withNumbers(5);
```

Output:

```text
12345
1234
123
12
1
```

---

## Program

```java
public class JavaBasics {

    public static void inverted_half_pyramid_withNumbers(int n){

        for(int i=1;i<=n;i++){

            for(int j=1;j<=n-i+1;j++){

                System.out.print(j);

            }

            System.out.println();
        }
    }

    public static void main(String[] args) {

        inverted_half_pyramid_withNumbers(5);

    }
}
```

---

## Logic

Observe the pattern:

```text
Row 1 → 12345
Row 2 → 1234
Row 3 → 123
Row 4 → 12
Row 5 → 1
```

Notice:

```text
Numbers decrease in every row.
```

Number of digits:

```text
5
4
3
2
1
```

The inner loop runs:

```java
j <= n - i + 1
```

which decreases every row.

---

## Formula Used

```java
n - i + 1
```

For:

```text
n = 5
```

| Row (i) | n-i+1 | Numbers Printed |
|----------|--------|----------------|
| 1 | 5 | 12345 |
| 2 | 4 | 1234 |
| 3 | 3 | 123 |
| 4 | 2 | 12 |
| 5 | 1 | 1 |

---

## Dry Run

Input:

```text
n = 5
```

### Row 1

| i | j Values | Output |
|---|----------|---------|
| 1 | 1 2 3 4 5 | 12345 |

---

### Row 2

| i | j Values | Output |
|---|----------|---------|
| 2 | 1 2 3 4 | 1234 |

---

### Row 3

| i | j Values | Output |
|---|----------|---------|
| 3 | 1 2 3 | 123 |

---

### Row 4

| i | j Values | Output |
|---|----------|---------|
| 4 | 1 2 | 12 |

---

### Row 5

| i | j Values | Output |
|---|----------|---------|
| 5 | 1 | 1 |

---

## Final Output

```text
12345
1234
123
12
1
```

---

## Visual Representation

```text
12345
1234
123
12
1
```

or

```text
5 digits
4 digits
3 digits
2 digits
1 digit
```

---

## Easy Understanding Trick

Think:

```text
Rows Increase

1
2
3
4
5
```

but

```text
Numbers Printed Decrease

5
4
3
2
1
```

Formula:

```text
n - i + 1
```

This tells us:

```text
How many numbers to print in each row.
```

---

## Pattern Building

Start with:

```text
12345
```

Remove one number from the end every row:

```text
12345
1234
123
12
1
```

Pattern Complete.

---

## Key Learning

- Number patterns use the same nested loop concepts as star patterns.
- The outer loop controls rows.
- The inner loop controls numbers printed.
- `n - i + 1` is a common formula in inverted patterns.
- Understanding this pattern helps in solving more advanced number patterns.

---

## Special Note

Remember:

```text
Rows ↑

Numbers Printed ↓
```

Formula:

```java
j <= n - i + 1
```

This single formula creates the entire Inverted Half Pyramid with Numbers.
