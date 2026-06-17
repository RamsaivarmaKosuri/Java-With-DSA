# Hollow Rhombus Pattern

The Hollow Rhombus Pattern is a shifted rectangle where only the boundary is made of stars (`*`) and the inside remains empty.

It is created using:

- Nested Loops
- Spaces
- Stars
- Hollow Rectangle Logic

This pattern helps in understanding:

- Space Management
- Boundary Conditions
- Nested Loop Logic
- Pattern Shifting

---

# Why Learn Hollow Rhombus?

The Hollow Rhombus Pattern combines two important concepts:

```text
Solid Rhombus
+
Hollow Rectangle
=
Hollow Rhombus
```

This pattern helps in:

- Building Pattern Logic
- Understanding Boundaries
- Improving Nested Loop Skills

---

# Pattern Output

For:

```java
hollowRhombus(5);
```

Output:

```text
    *****
   *   *
  *   *
 *   *
*****
```

---

# Program

```java
public class JavaBasics{

    public static void hollowRhombus(int n){

        // Outer Loop
        for(int i=1;i<=n;i++){

            // Spaces
            for(int j=1;j<=n-i;j++){
                System.out.print(" ");
            }

            // Hollow Rectangle
            for(int j=1;j<=n;j++){

                if(i==1 || i==n || j==1 || j==n){
                    System.out.print("*");
                }
                else{
                    System.out.print(" ");
                }
            }

            System.out.println();
        }
    }

    public static void main(String[] args) {
        hollowRhombus(5);
    }
}
```

---

# Understanding the Logic

The pattern is divided into two parts:

## Part 1: Print Spaces

```java
for(int j=1;j<=n-i;j++)
```

Formula:

```java
Spaces = n - i
```

For:

```text
n = 5
```

| Row (i) | Spaces |
|----------|---------|
| 1 | 4 |
| 2 | 3 |
| 3 | 2 |
| 4 | 1 |
| 5 | 0 |

Spaces decrease every row.

---

## Part 2: Print Hollow Rectangle

```java
if(i==1 || i==n || j==1 || j==n)
```

Boundary positions print stars.

Everything else prints spaces.

---

# Boundary Logic

| Condition | Meaning |
|------------|----------|
| i == 1 | Top Boundary |
| i == n | Bottom Boundary |
| j == 1 | Left Boundary |
| j == n | Right Boundary |

If any condition becomes true:

```java
System.out.print("*");
```

Otherwise:

```java
System.out.print(" ");
```

---

# Visual Understanding

First create a Hollow Rectangle:

```text
*****
*   *
*   *
*   *
*****
```

Now shift every row using spaces:

```text
    *****
   *   *
  *   *
 *   *
*****
```

This becomes the Hollow Rhombus.

---

# Complete Dry Run

Input:

```java
hollowRhombus(5);
```

---

## Row 1

```text
i = 1
```

### Spaces

```text
5 - 1 = 4
```

### Boundary

Since:

```java
i == 1
```

Entire row becomes stars.

Output:

```text
    *****
```

---

## Row 2

```text
i = 2
```

### Spaces

```text
5 - 2 = 3
```

### Boundary

Only:

```java
j == 1
```

and

```java
j == 5
```

print stars.

Output:

```text
   *   *
```

---

## Row 3

```text
i = 3
```

### Spaces

```text
5 - 3 = 2
```

Output:

```text
  *   *
```

---

## Row 4

```text
i = 4
```

### Spaces

```text
5 - 4 = 1
```

Output:

```text
 *   *
```

---

## Row 5

```text
i = 5
```

### Spaces

```text
5 - 5 = 0
```

Since:

```java
i == n
```

Entire row becomes stars.

Output:

```text
*****
```

---

# Dry Run Summary Table

| Row (i) | Spaces | Boundary Printed | Output |
|----------|---------|------------------|---------|
| 1 | 4 | Top Boundary |     ***** |
| 2 | 3 | Left & Right Boundary |    *   * |
| 3 | 2 | Left & Right Boundary |   *   * |
| 4 | 1 | Left & Right Boundary |  *   * |
| 5 | 0 | Bottom Boundary | ***** |

---

# Pattern Observation

### Spaces

```text
4
3
2
1
0
```

Spaces decrease by:

```text
-1
```

every row.

---

### Boundary Stars

```text
*****
*   *
*   *
*   *
*****
```

Only boundary positions print stars.

---

# Loop Analysis

### Outer Loop

```java
for(int i=1;i<=n;i++)
```

Controls:

```text
Rows
```

---

### First Inner Loop

```java
for(int j=1;j<=n-i;j++)
```

Controls:

```text
Spaces
```

---

### Second Inner Loop

```java
for(int j=1;j<=n;j++)
```

Controls:

```text
Hollow Rectangle
```

---

# Time Complexity

Outer Loop:

```text
n
```

Inner Loops:

```text
n
```

Overall:

```text
O(n²)
```

---

# Easy Memory Trick

Think:

```text
Solid Rhombus
+
Hollow Rectangle
=
Hollow Rhombus
```

or

```text
Spaces ↓

Boundary Stars Only
```

---

# Key Learning

- Hollow Rhombus is a shifted Hollow Rectangle.
- Spaces create the slant effect.
- Boundary Conditions decide where stars are printed.
- Interior positions remain empty.
- Nested loops work together to create the pattern.

---

# Special Note

Remember:

```java
Spaces = n - i
```

and

```java
if(i==1 || i==n || j==1 || j==n)
```

These two ideas create the complete Hollow Rhombus Pattern.
