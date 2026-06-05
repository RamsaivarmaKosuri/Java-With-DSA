# Practice Questions

These questions helped me practice Functions and Methods concepts such as:

- Parameters
- Return Types
- Boolean Functions
- Loops
- Number Manipulation
- Problem Solving

---

# Question 1

## Write a Java method to compute the average of three numbers.

### Program

```java
public class JavaBasics {

    public static int average(int a,int b,int c){

        int avg = (a+b+c)/3;

        System.out.println(
        "The Average of Three Numbers are : "
        + avg);

        return avg;
    }

    public static void main(String[] args) {

        average(3,4,5);

    }
}
```

### Output

```text
The Average of Three Numbers are : 4
```

### Dry Run

| Variable | Value |
|-----------|--------|
| a | 3 |
| b | 4 |
| c | 5 |

Calculation:

```text
(3 + 4 + 5) / 3

12 / 3

4
```

Output:

```text
4
```

### Key Learning

- Functions can return values.
- Parameters help pass data.
- Arithmetic operations can be performed inside methods.

---

# Question 2

## Write a method named isEven that accepts an int argument.

The method should return:

```text
true  -> Even Number

false -> Odd Number
```

### Program

```java
public class JavaBasics {

    public static boolean isEven(int n){

        if(n%2==0){

            System.out.println(
            "The given integer "
            + n +
            " is EVEN ");

            return true;
        }

        else{

            System.out.println(
            "The given integer "
            + n +
            " is ODD ");

            return false;
        }
    }

    public static void main(String[] args) {

        isEven(47);

    }
}
```

### Output

```text
The given integer 47 is ODD
false
```

### Dry Run

Input:

```text
47
```

Calculation:

```text
47 % 2 = 1
```

Condition:

```java
n % 2 == 0
```

becomes:

```text
1 == 0
```

Result:

```text
false
```

Output:

```text
ODD
```

### Key Learning

- Boolean functions return true or false.
- Even numbers have remainder 0 when divided by 2.

---

# Question 3

## Write a Java program to check whether a number is a Palindrome.

### Program

```java
public class JavaBasics {

    public static boolean palindrome(int n){

        if(n<0){
            return false;
        }

        int originalNumber = n;

        int reverse = 0;

        while(n>0){

            int lastdigit = n%10;

            reverse =
            (reverse*10)+lastdigit;

            n=n/10;
        }

        return originalNumber==reverse;
    }

    public static void main(String[] args) {

        System.out.println(
        palindrome(151));

    }
}
```

### Output

```text
true
```

---

### Dry Run

Input:

```text
151
```

| Iteration | n | Last Digit | Reverse |
|------------|---|------------|----------|
| Start | 151 | - | 0 |
| 1 | 151 | 1 | 1 |
| 2 | 15 | 5 | 15 |
| 3 | 1 | 1 | 151 |

Final Check:

```text
originalNumber = 151

reverse = 151
```

Comparison:

```text
151 == 151
```

Result:

```text
true
```

---

### Visual Representation

```text
151

1 → 15 → 151

Original = 151

Reverse = 151

Palindrome
```

---

### Key Learning

- Reverse a number using loops.
- Compare original and reversed values.
- Boolean methods can solve logical problems.

---

## Overall Learning

After solving these questions, I practiced:

- Function Creation
- Parameters
- Return Values
- Boolean Methods
- Loops
- Number Logic
- Problem Solving
- Dry Run Analysis
