# Arrays - Input, Output & Update

After creating an array, the next step is:

1. Input (Store Values)
2. Output (Print Values)
3. Update (Modify Values)

These are the most common operations performed on arrays.

---

# Program

```java
import java.util.*;

public class JavaBasics{
    public static void main(String[] args) {

        int marks[] = new int[100];

        Scanner sc = new Scanner(System.in);

        marks[0] = sc.nextInt();
        marks[1] = sc.nextInt();
        marks[2] = sc.nextInt();

        System.out.println("phy : " + marks[0]);
        System.out.println("chem : " + marks[1]);
        System.out.println("math : " + marks[2]);

        marks[2] = marks[2] + 2;

        System.out.println("math updated : " + marks[2]);

        float percentage = (marks[0] + marks[1] + marks[2]) / 3;

        System.out.println("percentage : " + percentage);

        System.out.println("Length of an array : " + marks.length);
    }
}
```

---

# Understanding the Program

The program demonstrates:

- Array Creation
- Taking Input
- Printing Output
- Updating Values
- Percentage Calculation
- Array Length

---

# Step 1 : Create an Array

```java
int marks[] = new int[100];
```

Meaning:

```text
Create an integer array
named marks
with size 100.
```

Memory:

```text
Index

0    1    2    3    4    ... 99
---------------------------------
0 | 0 | 0 | 0 | 0 | ... 0
---------------------------------
```

Initially:

```text
All values are 0.
```

---

# Important Observation

We created:

```java
int marks[] = new int[100];
```

but used only:

```java
marks[0]
marks[1]
marks[2]
```

Java does NOT give an error.

Reason:

```text
We can use as many positions as we need
as long as they are within the array size.
```

---

# Step 2 : Taking Input

```java
marks[0] = sc.nextInt();
marks[1] = sc.nextInt();
marks[2] = sc.nextInt();
```

Sample Input:

```text
90
95
98
```

Memory becomes:

```text
Index

0    1    2
--------------
90 | 95 | 98
--------------
```

---

# Dry Run Table (Input)

| Statement | Value Stored |
|------------|--------------|
| marks[0] = 90 | 90 |
| marks[1] = 95 | 95 |
| marks[2] = 98 | 98 |

Final Array:

```text
[90, 95, 98]
```

---

# Step 3 : Printing Output

```java
System.out.println("phy : " + marks[0]);
System.out.println("chem : " + marks[1]);
System.out.println("math : " + marks[2]);
```

Output:

```text
phy : 90
chem : 95
math : 98
```

This is called:

```text
Accessing Array Elements
```

Syntax:

```java
arrayName[index]
```

Example:

```java
marks[2]
```

returns:

```text
98
```

---

# Step 4 : Updating Values

```java
marks[2] = marks[2] + 2;
```

Current value:

```text
98
```

Calculation:

```text
98 + 2 = 100
```

Updated Memory:

```text
Index

0    1    2
---------------
90 | 95 | 100
---------------
```

Output:

```text
math updated : 100
```

---

# Dry Run Table (Update)

| Before | Operation | After |
|----------|------------|---------|
| 98 | 98 + 2 | 100 |

---

# Step 5 : Percentage Calculation

```java
float percentage =
(marks[0] + marks[1] + marks[2]) / 3;
```

Values:

```text
90 + 95 + 100
```

Sum:

```text
285
```

Percentage:

```text
285 / 3 = 95
```

Output:

```text
percentage : 95.0
```

---

# Dry Run Table (Percentage)

| Subject | Marks |
|----------|---------|
| Physics | 90 |
| Chemistry | 95 |
| Maths | 100 |

Total:

```text
285
```

Percentage:

```text
95.0
```

---

# Step 6 : Length Property

```java
marks.length
```

Output:

```text
100
```

Reason:

```java
int marks[] = new int[100];
```

Array size is:

```text
100
```

Therefore:

```java
marks.length
```

returns:

```text
100
```

---

# Important Difference

### Length Property

```java
marks.length
```

returns:

```text
Size of Array
```

### Index

Last index:

```text
length - 1
```

Example:

```java
int marks[] = new int[100];
```

| Property | Value |
|------------|---------|
| Length | 100 |
| First Index | 0 |
| Last Index | 99 |

---

# Complete Dry Run

Input:

```text
90
95
98
```

Array after input:

```text
[90,95,98]
```

After update:

```text
[90,95,100]
```

Percentage:

```text
95.0
```

Length:

```text
100
```

---

# Final Output

```text
phy : 90
chem : 95
math : 98

math updated : 100

percentage : 95.0

Length of an array : 100
```

---

# Real-Life Analogy

Think of a student's mark sheet.

```text
Index 0 → Physics
Index 1 → Chemistry
Index 2 → Maths
```

Input:

```text
Store Marks
```

Output:

```text
Display Marks
```

Update:

```text
Correct Marks
```

This is exactly how arrays work.

---

# Interview Notes

### Can we create an array of size 100 and use only 3 elements?

Answer:

```text
Yes.
Unused positions remain with default values.
```

---

### How do we update an element?

```java
marks[index] = newValue;
```

Example:

```java
marks[2] = 100;
```

---

### How do we find array size?

```java
arrayName.length
```

---

# Key Takeaways

- Arrays support Input, Output, and Update operations.
- Values are accessed using indexes.
- Array indexing starts from 0.
- Elements can be updated anytime.
- `.length` returns the total array size.
- Unused positions store default values.
- Arrays make storing and managing multiple values easy.
