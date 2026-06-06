# Butterfly Pattern

The Butterfly Pattern is one of the most important advanced star patterns.

It combines:

- Nested Loops
- Stars (`*`)
- Spaces (` `)
- Symmetry

The pattern resembles a butterfly with two wings.

---

# Why Learn Butterfly Pattern?

This pattern helps us understand:

- Nested Loop Mastery
- Space Management
- Symmetric Pattern Design
- Row and Column Relationships
- Logic Building

Many advanced patterns such as:

- Diamond Pattern
- Hollow Diamond
- Sandglass Pattern

use similar concepts.

---

# Pattern Output

For:

```java
butterfly(5);
```

Output:

```text
*        *
**      **
***    ***
****  ****
**********
**********
****  ****
***    ***
**      **
*        *
```

---

# Pattern Breakdown

The Butterfly Pattern consists of:

```text
First Half
+
Second Half
```

Think of it as:

```text
Upper Wing
+
Lower Wing
```

---

# Structure of Each Row

Every row contains:

```text
Left Stars
+
Middle Spaces
+
Right Stars
```

Example:

```text
***    ***
```

contains:

| Part | Count |
|--------|--------|
| Left Stars | 3 |
| Spaces | 4 |
| Right Stars | 3 |

---

# Visualizing the Butterfly

```text
*        *
**      **
***    ***
****  ****
**********
**********
****  ****
***    ***
**      **
*        *
```

Notice:

```text
Stars move outward
Spaces move inward
```

until the center is reached.

After that:

```text
Stars move inward
Spaces move outward
```

creating the lower wing.

---

# Program

```java
public class JavaBasics {

    public static void butterfly(int n){

        // First Half
        for(int i=1;i<=n;i++){

            // Left Stars
            for(int j=1;j<=i;j++){
                System.out.print("*");
            }

            // Spaces
            for(int j=1;j<=2*(n-i);j++){
                System.out.print(" ");
            }

            // Right Stars
            for(int j=1;j<=i;j++){
                System.out.print("*");
            }

            System.out.println();
        }

        // Second Half
        for(int i=n;i>=1;i--){

            // Left Stars
            for(int j=1;j<=i;j++){
                System.out.print("*");
            }

            // Spaces
            for(int j=1;j<=2*(n-i);j++){
                System.out.print(" ");
            }

            // Right Stars
            for(int j=1;j<=i;j++){
                System.out.print("*");
            }

            System.out.println();
        }
    }

    public static void main(String[] args) {
        butterfly(5);
    }
}
```

---

# Understanding the Logic

The pattern is built using:

```text
Stars
Spaces
Stars
```

For every row:

```text
Left Wing
Center Gap
Right Wing
```

The number of stars depends on:

```java
i
```

The number of spaces depends on:

```java
2 * (n - i)
```

---

# First Half Analysis

For:

```text
n = 5
```

### Formula

```java
Stars = i

Spaces = 2 * (n-i)
```

---

## Row-wise Analysis

| Row (i) | Left Stars | Spaces | Right Stars | Output |
|----------|------------|---------|------------|---------|
| 1 | 1 | 8 | 1 | *        * |
| 2 | 2 | 6 | 2 | **      ** |
| 3 | 3 | 4 | 3 | ***    *** |
| 4 | 4 | 2 | 4 | ****  **** |
| 5 | 5 | 0 | 5 | ********** |

---

## Pattern Observation

### Stars

```text
1
2
3
4
5
```

Stars increase by:

```text
+1
```

every row.

---

### Spaces

```text
8
6
4
2
0
```

Spaces decrease by:

```text
-2
```

every row.

---

# Dry Run (First Half)

## Row 1

| Component | Value |
|------------|--------|
| Stars | 1 |
| Spaces | 8 |
| Stars | 1 |

Output:

```text
*        *
```

---

## Row 2

| Component | Value |
|------------|--------|
| Stars | 2 |
| Spaces | 6 |
| Stars | 2 |

Output:

```text
**      **
```

---

## Row 3

| Component | Value |
|------------|--------|
| Stars | 3 |
| Spaces | 4 |
| Stars | 3 |

Output:

```text
***    ***
```

---

## Row 4

| Component | Value |
|------------|--------|
| Stars | 4 |
| Spaces | 2 |
| Stars | 4 |

Output:

```text
****  ****
```

---

## Row 5

| Component | Value |
|------------|--------|
| Stars | 5 |
| Spaces | 0 |
| Stars | 5 |

Output:

```text
**********
```

---

# Why 2 × (n - i)?

The center gap is controlled by:

```java
2 * (n - i)
```

For:

```text
n = 5
```

| Row | Calculation | Spaces |
|------|------------|---------|
| 1 | 2 × (5−1) | 8 |
| 2 | 2 × (5−2) | 6 |
| 3 | 2 × (5−3) | 4 |
| 4 | 2 × (5−4) | 2 |
| 5 | 2 × (5−5) | 0 |

This gradually closes the gap between the two wings.

---

# Second Half Analysis

The second half is simply the reverse of the first half.

---

## Row-wise Analysis

| Row (i) | Left Stars | Spaces | Right Stars | Output |
|----------|------------|---------|------------|---------|
| 5 | 5 | 0 | 5 | ********** |
| 4 | 4 | 2 | 4 | ****  **** |
| 3 | 3 | 4 | 3 | ***    *** |
| 2 | 2 | 6 | 2 | **      ** |
| 1 | 1 | 8 | 1 | *        * |

---

## Pattern Observation

### Stars

```text
5
4
3
2
1
```

Stars decrease by:

```text
-1
```

every row.

---

### Spaces

```text
0
2
4
6
8
```

Spaces increase by:

```text
+2
```

every row.

---

# Complete Pattern Construction

```text
Step 1 → Print Left Stars

Step 2 → Print Spaces

Step 3 → Print Right Stars

Step 4 → Repeat until center

Step 5 → Reverse the process
```

---

# Easy Memory Trick

Remember:

```text
Butterfly = Mirror + Mirror
```

First Half:

```text
Stars ↑
Spaces ↓
```

Second Half:

```text
Stars ↓
Spaces ↑
```

That's the entire Butterfly Pattern.

---

# Key Learning

- Outer loop controls rows.
- Inner loops control stars and spaces.
- Symmetry is the core idea.
- Space management is extremely important.
- Butterfly Pattern is a foundation for many advanced DSA patterns.

---

# Special Note

Always remember:

```java
Stars = i

Spaces = 2 * (n - i)
```

These two formulas create the complete Butterfly Pattern.
