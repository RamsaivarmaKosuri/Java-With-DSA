# Floyd's Triangle

Floyd's Triangle is a number pattern where numbers are printed continuously in increasing order.

Unlike previous patterns where numbers restart from `1` in every row, Floyd's Triangle uses:

```text
One continuous counter
```

This pattern helps in understanding:

- Nested Loops
- Number Patterns
- Counters
- Pattern Visualization
- Sequential Number Generation

---

## Pattern Output

For:

```java
floyds_triangle(5);
```

Output:

```text
1
2 3
4 5 6
7 8 9 10
11 12 13 14 15
```

---

## Program

```java
public class JavaBasics {

    public static void floyds_triangle(int n){

        int count = 1;

        for(int i=1;i<=n;i++){

            for(int j=1;j<=i;j++){

                System.out.print(count + " ");

                count++;
            }

            System.out.println();
        }
    }

    public static void main(String[] args) {

        floyds_triangle(5);

    }
}
```

---

## Logic

Observe the pattern:

```text
Row 1 → 1

Row 2 → 2 3

Row 3 → 4 5 6

Row 4 → 7 8 9 10

Row 5 → 11 12 13 14 15
```

Notice:

```text
Numbers never restart from 1.
```

Instead:

```text
1 → 2 → 3 → 4 → 5 → ...
```

continue throughout the pattern.

---

## Important Variable

```java
int count = 1;
```

This variable stores the next number to print.

After printing:

```java
count++;
```

moves to the next number.

---

## Dry Run

Input:

```text
n = 5
```

Initially:

```text
count = 1
```

---

### Row 1

| j | Printed Value | Next Count |
|---|--------------|------------|
| 1 | 1 | 2 |

Output:

```text
1
```

---

### Row 2

| j | Printed Value | Next Count |
|---|--------------|------------|
| 1 | 2 | 3 |
| 2 | 3 | 4 |

Output:

```text
2 3
```

---

### Row 3

| j | Printed Value | Next Count |
|---|--------------|------------|
| 1 | 4 | 5 |
| 2 | 5 | 6 |
| 3 | 6 | 7 |

Output:

```text
4 5 6
```

---

### Row 4

| j | Printed Value | Next Count |
|---|--------------|------------|
| 1 | 7 | 8 |
| 2 | 8 | 9 |
| 3 | 9 | 10 |
| 4 | 10 | 11 |

Output:

```text
7 8 9 10
```

---

### Row 5

| j | Printed Value | Next Count |
|---|--------------|------------|
| 1 | 11 | 12 |
| 2 | 12 | 13 |
| 3 | 13 | 14 |
| 4 | 14 | 15 |
| 5 | 15 | 16 |

Output:

```text
11 12 13 14 15
```

---

## Final Output

```text
1
2 3
4 5 6
7 8 9 10
11 12 13 14 15
```

---

## Visual Representation

```text
                1

             2     3

          4     5     6

       7     8     9     10

   11    12    13    14    15
```

---

## Easy Understanding Trick

Think:

```text
Normal Number Pattern

1
12
123
1234
```

Numbers restart every row.

But in Floyd's Triangle:

```text
1
23
456
78910
1112131415
```

Numbers never restart.

They keep increasing continuously.

---

## Pattern Building

Start with:

```text
count = 1
```

Print it.

Increase:

```text
count++
```

Print again.

Keep repeating.

Result:

```text
1
2 3
4 5 6
7 8 9 10
11 12 13 14 15
```

---

## Key Learning

- Floyd's Triangle uses a continuous counter.
- Numbers do not restart in each row.
- Outer loop controls rows.
- Inner loop controls how many numbers are printed.
- `count++` is the key idea behind this pattern.

---

## Special Note

Remember:

```text
Stars Pattern
      ↓
Print *

Number Pattern
      ↓
Print j

Floyd's Triangle
      ↓
Print count
      ↓
count++
```

The entire pattern is built using:

```java
System.out.print(count + " ");
count++;
```
