# Arrays as Function Arguments

In Java, arrays can be passed to functions just like normal variables.

However, arrays behave differently from primitive data types like:

```java
int
float
double
char
boolean
```

This topic is very important because many beginners get confused about:

```text
Why does the array change?

But the normal variable does not change?
```

Let's understand it step by step.

---

# Program

```java
public class JavaBasics{

    public static void update(int marks[], int number){

        number = 10;

        for(int i=0; i<marks.length; i++){
            marks[i] = marks[i] + 1;
        }
    }

    public static void main(String[] args) {

        int marks[] = {97,98,99};
        int number = 5;

        update(marks, number);

        System.out.println("number : " + number);

        for(int i=0; i<marks.length; i++){
            System.out.print(marks[i] + " ");
        }

        System.out.println();
    }
}
```

---

# Output

```text
number : 5
98 99 100
```

---

# What Are We Learning?

In this program we pass:

```java
marks
```

and

```java
number
```

to the function:

```java
update(marks, number);
```

Inside the function:

```java
number = 10;
```

and

```java
marks[i] = marks[i] + 1;
```

are executed.

But after the function finishes:

```text
number : 5
98 99 100
```

is printed.

Let's understand why.

---

# Initial Values

Before calling the function:

```java
int marks[] = {97,98,99};
int number = 5;
```

Memory:

```text
marks

Index

0    1    2
--------------
97 | 98 | 99
--------------
```

```text
number = 5
```

---

# Function Call

```java
update(marks, number);
```

Control moves to:

```java
update(int marks[], int number)
```

---

# What Happens to number?

Inside the function:

```java
number = 10;
```

Now many beginners think:

```text
number should become 10
```

But output is:

```text
number : 5
```

Why?

Because Java uses:

```text
Call By Value
```

for primitive data types.

Java sends a copy of the value.

Original:

```text
number = 5
```

Copy sent to function:

```text
number = 5
```

Function changes copy:

```text
5 → 10
```

Original remains:

```text
5
```

---

# Dry Run Table (number)

| Step | Value |
|--------|--------|
| Original number | 5 |
| Copy sent to function | 5 |
| number = 10 | 10 |
| Function ends | Copy destroyed |
| Original number | 5 |

Therefore:

```text
number : 5
```

is printed.

---

# What Happens to marks Array?

Inside the function:

```java
for(int i=0;i<marks.length;i++){
    marks[i] = marks[i] + 1;
}
```

The loop increases every element by 1.

---

# Iteration 1

```java
marks[0] = 97 + 1;
```

Array:

```text
[98,98,99]
```

---

# Iteration 2

```java
marks[1] = 98 + 1;
```

Array:

```text
[98,99,99]
```

---

# Iteration 3

```java
marks[2] = 99 + 1;
```

Array:

```text
[98,99,100]
```

---

# Dry Run Table (Array Update)

| Iteration | Index | Old Value | New Value |
|------------|---------|------------|------------|
| 1 | 0 | 97 | 98 |
| 2 | 1 | 98 | 99 |
| 3 | 2 | 99 | 100 |

Final Array:

```text
[98,99,100]
```

---

# Why Does Array Change?

This is the most important part.

When an array is passed to a function, both:

```java
main()
```

and

```java
update()
```

work on the same array.

Visual Representation:

```text
main()
   |
   v

[97,98,99]

   ^
   |
update()
```

Both are connected to the same array.

Therefore if update() changes:

```java
marks[0]
```

the original array also changes.

That's why:

```text
98 99 100
```

is printed.

---

# Easy Trick to Remember

Imagine two situations.

---

## Case 1 : Normal Variable

```java
int number = 5;
```

You give your friend a photocopy.

Friend changes:

```text
5 → 10
```

Your original paper still has:

```text
5
```

So original value does not change.

---

## Case 2 : Array

```java
int marks[] = {97,98,99};
```

Instead of a photocopy,

both people get access to the same house.

If one person paints the house,

everyone sees the change.

Similarly:

```java
marks[0] = 98;
```

changes the original array.

---

# Important Note

Many students say:

```text
Arrays use Call By Reference.
```

This is not completely correct.

Java always uses:

```text
Call By Value
```

But for arrays, Java passes a copy of the reference.

Because both references point to the same array,

changes become visible outside the function.

For beginners, simply remember:

```text
Primitive Variable → Original does not change

Array → Original changes
```

---

# Comparison Table

| Primitive Variable | Array |
|-------------------|--------|
| int, float, char etc. | int[], String[] etc. |
| Copy of value is sent | Access to same array |
| Original doesn't change | Original changes |
| Example: number | Example: marks[] |

---

# Common Beginner Mistake

Many beginners expect:

```java
number = 10;
```

to change the original variable.

But it does not.

Because:

```text
Only a copy was modified.
```

---

# Key Takeaways

- Arrays can be passed as function arguments.
- Primitive variables follow Call By Value.
- Changes made to primitive variables inside a function do not affect the original variable.
- Changes made to array elements inside a function are visible outside the function.
- Arrays and functions are commonly used together in DSA.
- Understanding this concept is important before learning sorting and searching algorithms.

---

# Interview Questions

### 1. Can arrays be passed to functions?

Yes.

```java
update(marks);
```

Arrays can be passed as arguments just like normal variables.

---

### 2. Why does the original array change?

Because both functions work on the same array.

Changes made inside the function are reflected outside.

---

### 3. Does Java support Call By Reference?

No.

Java always uses:

```text
Call By Value
```

---

### 4. Why doesn't number change?

Because Java passes a copy of the value.

The original variable remains unchanged.

---

### 5. Why are arrays important in DSA?

Because most searching, sorting, and problem-solving algorithms work on arrays.

---

### 6. Which changes after function execution?

| Variable Type | Changes? |
|--------------|----------|
| Primitive Variable | ❌ No |
| Array Elements | ✅ Yes |

---

### 7. What is the output of this program?

```java
int arr[] = {1,2,3};

update(arr);
```

If update() adds 1 to every element:

Output:

```text
2 3 4
```

because the original array gets modified.

# Easy Note to Remember

If you ever get confused in exams or interviews, remember this simple rule:

```text
Normal Variables → Changes stay inside the function

Arrays → Changes are visible outside the function
```

Example:

```java
int number = 5;
```

Inside function:

```java
number = 10;
```

Outside function:

```text
Still 5
```

because only a copy of the value was changed.

---

Example:

```java
int marks[] = {97,98,99};
```

Inside function:

```java
marks[0] = 98;
```

Outside function:

```text
98 99 100
```

because the function is working on the same array.

---

### Quick Revision Trick

Remember this sentence:

```text
If it is a normal variable,
the original value stays safe.

If it is an array,
the original array can be modified.
```

---

### One-Line Exam Revision

```text
Primitive Variables → Original Value Doesn't Change

Arrays → Original Elements Can Change
```

This single line is enough to remember the entire concept.
