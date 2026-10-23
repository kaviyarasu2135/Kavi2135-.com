Algorithm
1. Start.
2. Read a and b.
3. Calculate sum = a + b.
4. Calculate difference = a - b.
5. Calculate product = a * b.
6. If b is not zero, calculate quotient = a / b; otherwise report division by zero.
7. Display the results.
8. Stop.
C Program
#include <stdio.h>

int main(void) {
    float a, b;
    printf("Enter two numbers: ");
    scanf("%f %f", &a, &b);

    printf("Sum = %.2f\n", a + b);
    printf("Difference = %.2f\n", a - b);
    printf("Product = %.2f\n", a * b);

    if (b != 0)
        printf("Quotient = %.2f\n", a / b);
    else
        printf("Quotient = Undefined (division by zero)\n");

    return 0;
}
Sample Output
Enter two numbers: 12 4
Sum = 16.00
Difference = 8.00
Product = 48.00
Quotient = 3.00

Experiment 2: Pseudocode for Decision Making
Unit
Unit I – Problem Solving and Algorithmic Thinking
Aim
To write pseudocode for a simple decision-making problem.
Activity / Problem Statement
Write pseudocode and implement a program to determine whether a student is eligible for a scholarship when marks are at least 75.
Learning Outcome
The student should be able to understand the logic, write the algorithm/pseudocode, implement the C program, compile it, test it, and interpret the output.

Algorithm
1. Start.
2. Read marks.
3. If marks >= 75, display Eligible.
4. Otherwise display Not Eligible.
5. Stop.
C Program
#include <stdio.h>

int main(void) {
    float marks;
    printf("Enter marks: ");
    scanf("%f", &marks);

    if (marks >= 75)
        printf("Eligible for scholarship\n");
    else
        printf("Not eligible for scholarship\n");

    return 0;
}
Sample Output
Enter marks: 82
Eligible for scholarship

Experiment 3: Algorithm for Arithmetic and Logical Operations
Unit
Unit I – Problem Solving and Algorithmic Thinking
Aim
To design an algorithm for arithmetic and logical operations.
Activity / Problem Statement
Accept two integers and display the larger value and whether both numbers are even.
Learning Outcome
The student should be able to understand the logic, write the algorithm/pseudocode, implement the C program, compile it, test it, and interpret the output.

Algorithm
1. Start.
2. Read a and b.
3. Compare a and b and display the larger value.
4. Check a % 2 == 0 and b % 2 == 0.
5. Display whether both are even.
6. Stop.
C Program
#include <stdio.h>

int main(void) {
    int a, b;
    printf("Enter two integers: ");
    scanf("%d %d", &a, &b);

    if (a > b)
        printf("Larger = %d\n", a);
    else if (b > a)
        printf("Larger = %d\n", b);
    else
        printf("Both are equal\n");

    if (a % 2 == 0 && b % 2 == 0)
        printf("Both numbers are even\n");
    else
        printf("Both numbers are not even\n");

    return 0;
}
Sample Output
Enter two integers: 18 12
Larger = 18
Both numbers are even

Experiment 4: Convert Flowchart Logic into Pseudocode
Unit
Unit I – Problem Solving and Algorithmic Thinking
Aim
To convert a simple flowchart logic into pseudocode and then into C.
Activity / Problem Statement
For an integer n, determine whether it is positive, negative, or zero.
Learning Outcome
The student should be able to understand the logic, write the algorithm/pseudocode, implement the C program, compile it, test it, and interpret the output.

Algorithm
1. Start.
2. Read n.
3. If n > 0, display Positive.
4. Else if n < 0, display Negative.
5. Else display Zero.
6. Stop.
C Program
#include <stdio.h>

int main(void) {
    int n;
    printf("Enter an integer: ");
    scanf("%d", &n);

    if (n > 0)
        printf("Positive\n");
    else if (n < 0)
        printf("Negative\n");
    else
        printf("Zero\n");

    return 0;
}
Sample Output
Enter an integer: -7
Negative

Experiment 5: Explore Data Types
Unit
Unit II – Overview of C
Aim
To understand common C data types and observe their storage sizes.
Activity / Problem Statement
Declare variables of char, int, float and double types, assign values, and display their values and sizes using sizeof.
Learning Outcome
The student should be able to understand the logic, write the algorithm/pseudocode, implement the C program, compile it, test it, and interpret the output.

Algorithm
1. Start.
2. Declare char, int, float and double variables.
3. Assign sample values.
4. Print each value.
5. Print sizeof each data type.
6. Stop.
C Program
#include <stdio.h>

int main(void) {
    char ch = 'A';
    int n = 25;
    float f = 12.5f;
    double d = 123.456;

    printf("char   : %c, size = %zu bytes\n", ch, sizeof(ch));
    printf("int    : %d, size = %zu bytes\n", n, sizeof(n));
    printf("float  : %.2f, size = %zu bytes\n", f, sizeof(f));
    printf("double : %.3f, size = %zu bytes\n", d, sizeof(d));

    return 0;
}
Sample Output
char   : A, size = 1 bytes
int    : 25, size = 4 bytes
float  : 12.50, size = 4 bytes
double : 123.456, size = 8 bytes

Experiment 6: Formatted Input and Output
Unit
Unit II – Overview of C
Aim
To demonstrate formatted input and output operations in C.
Activity / Problem Statement
Read student name, roll number, age and percentage and display them in a formatted report.
Learning Outcome
The student should be able to understand the logic, write the algorithm/pseudocode, implement the C program, compile it, test it, and interpret the output.

Algorithm
1. Start.
2. Read name, roll number, age and percentage.
3. Print the values using suitable format specifiers.
4. Stop.
C Program
#include <stdio.h>

int main(void) {
    char name[50];
    int roll, age;
    float percentage;

    printf("Enter name: ");
    scanf("%49s", name);
    printf("Enter roll number: ");
    scanf("%d", &roll);
    printf("Enter age: ");
    scanf("%d", &age);
    printf("Enter percentage: ");
    scanf("%f", &percentage);

    printf("\n--- Student Report ---\n");
    printf("%-15s : %s\n", "Name", name);
    printf("%-15s : %d\n", "Roll Number", roll);
    printf("%-15s : %d\n", "Age", age);
    printf("%-15s : %.2f%%\n", "Percentage", percentage);

    return 0;
}
Sample Output
Enter name: Ravi
Enter roll number: 101
Enter age: 18
Enter percentage: 86.5

--- Student Report ---
Name            : Ravi
Roll Number     : 101
Age             : 18
Percentage      : 86.50%

Experiment 7: Selection Statements – Grade Calculator
Unit
Unit II – Overview of C
Aim
To implement if-else-if selection statements.
Activity / Problem Statement
Accept marks and display the grade using a suitable grade classification.
Learning Outcome
The student should be able to understand the logic, write the algorithm/pseudocode, implement the C program, compile it, test it, and interpret the output.

Algorithm
1. Read marks.
2. If marks >= 90, grade A.
3. Else if marks >= 75, grade B.
4. Else if marks >= 60, grade C.
5. Else if marks >= 50, grade D.
6. Otherwise grade F.
7. Stop.
C Program
#include <stdio.h>

int main(void) {
    int marks;
    printf("Enter marks: ");
    scanf("%d", &marks);

    if (marks >= 90)
        printf("Grade A\n");
    else if (marks >= 75)
        printf("Grade B\n");
    else if (marks >= 60)
        printf("Grade C\n");
    else if (marks >= 50)
        printf("Grade D\n");
    else
        printf("Grade F\n");

    return 0;
}
Sample Output
Enter marks: 84
Grade B

Experiment 8: Switch Statement – Simple Calculator
Unit
Unit II – Overview of C
Aim
To implement a selection program using switch.
Activity / Problem Statement
Accept two numbers and an operator (+, -, *, /) and display the result.
Learning Outcome
The student should be able to understand the logic, write the algorithm/pseudocode, implement the C program, compile it, test it, and interpret the output.

Algorithm
1. Read a, operator and b.
2. Use switch on operator.
3. Perform the corresponding operation.
4. Check division by zero for /.
5. Display result.
6. Stop.
C Program
#include <stdio.h>

int main(void) {
    double a, b;
    char op;

    printf("Enter expression (e.g., 10 + 5): ");
    scanf("%lf %c %lf", &a, &op, &b);

    switch (op) {
        case '+': printf("Result = %.2f\n", a + b); break;
        case '-': printf("Result = %.2f\n", a - b); break;
        case '*': printf("Result = %.2f\n", a * b); break;
        case '/':
            if (b != 0) printf("Result = %.2f\n", a / b);
            else printf("Division by zero is not allowed\n");
            break;
        default: printf("Invalid operator\n");
    }
    return 0;
}
Sample Output
Enter expression (e.g., 10 + 5): 10 * 5
Result = 50.00

Experiment 9: Looping Statements – Multiplication Table
Unit
Unit II – Overview of C
Aim
To execute a program using a looping statement.
Activity / Problem Statement
Read an integer and print its multiplication table from 1 to 10 using a for loop.
Learning Outcome
The student should be able to understand the logic, write the algorithm/pseudocode, implement the C program, compile it, test it, and interpret the output.

Algorithm
1. Read n.
2. Set i = 1.
3. Repeat while i <= 10.
4. Print n * i.
5. Increment i.
6. Stop.
C Program
#include <stdio.h>

int main(void) {
    int n;
    printf("Enter a number: ");
    scanf("%d", &n);

    for (int i = 1; i <= 10; i++)
        printf("%d x %d = %d\n", n, i, n * i);

    return 0;
}
Sample Output
Enter a number: 7
7 x 1 = 7
7 x 2 = 14
...
7 x 10 = 70

Experiment 10: Jumping Statements
Unit
Unit II – Overview of C
Aim
To demonstrate break and continue statements.
Activity / Problem Statement
Print numbers from 1 to 20, skip multiples of 3 using continue, and stop when 17 is reached using break.
Learning Outcome
The student should be able to understand the logic, write the algorithm/pseudocode, implement the C program, compile it, test it, and interpret the output.

Algorithm
1. Start loop from 1 to 20.
2. If number is a multiple of 3, continue.
3. If number is 17, break.
4. Otherwise print the number.
5. Stop.
C Program
#include <stdio.h>

int main(void) {
    for (int i = 1; i <= 20; i++) {
        if (i == 17)
            break;
        if (i % 3 == 0)
            continue;
        printf("%d ", i);
    }
    printf("\n");
    return 0;
}
Sample Output
1 2 4 5 7 8 10 11 13 14 16

Experiment 11: Two-Dimensional Array – Matrix Addition
Unit
Unit III – Arrays, Functions and Pointers
Aim
To execute a multidimensional array program.
Activity / Problem Statement
Read two 2×2 matrices and display their sum.
Learning Outcome
The student should be able to understand the logic, write the algorithm/pseudocode, implement the C program, compile it, test it, and interpret the output.

Algorithm
1. Read matrix A.
2. Read matrix B.
3. For each row and column, calculate C[i][j] = A[i][j] + B[i][j].
4. Display C.
5. Stop.
C Program
#include <stdio.h>

int main(void) {
    int a[2][2], b[2][2], c[2][2];

    printf("Enter Matrix A (2x2):\n");
    for (int i = 0; i < 2; i++)
        for (int j = 0; j < 2; j++)
            scanf("%d", &a[i][j]);

    printf("Enter Matrix B (2x2):\n");
    for (int i = 0; i < 2; i++)
        for (int j = 0; j < 2; j++)
            scanf("%d", &b[i][j]);

    printf("Sum Matrix:\n");
    for (int i = 0; i < 2; i++) {
        for (int j = 0; j < 2; j++) {
            c[i][j] = a[i][j] + b[i][j];
            printf("%d ", c[i][j]);
        }
        printf("\n");
    }
    return 0;
}
Sample Output
Enter Matrix A (2x2):
1 2
3 4
Enter Matrix B (2x2):
5 6
7 8
Sum Matrix:
6 8
10 12

Experiment 12: User-Defined Function – Prime Number
Unit
Unit III – Arrays, Functions and Pointers
Aim
To implement a user-defined function.
Activity / Problem Statement
Create a function isPrime() that returns whether a given integer is prime.
Learning Outcome
The student should be able to understand the logic, write the algorithm/pseudocode, implement the C program, compile it, test it, and interpret the output.

Algorithm
1. Read n.
2. Call isPrime(n).
3. In the function, test divisibility from 2 to n/2.
4. Return 0 if divisible; otherwise return 1.
5. Display the result.
C Program
#include <stdio.h>

int isPrime(int n) {
    if (n < 2)
        return 0;

    for (int i = 2; i <= n / i; i++)
        if (n % i == 0)
            return 0;

    return 1;
}

int main(void) {
    int n;
    printf("Enter an integer: ");
    scanf("%d", &n);

    if (isPrime(n))
        printf("%d is prime\n", n);
    else
        printf("%d is not prime\n", n);

    return 0;
}
Sample Output
Enter an integer: 29
29 is prime

Experiment 13: Array and Function – Find Maximum
Unit
Unit III – Arrays, Functions and Pointers
Aim
To develop a program using an array and a function.
Activity / Problem Statement
Read n elements into an array and use a function to find the maximum element.
Learning Outcome
The student should be able to understand the logic, write the algorithm/pseudocode, implement the C program, compile it, test it, and interpret the output.

Algorithm
1. Read n and array elements.
2. Pass the array and n to findMax().
3. Initialize max with the first element.
4. Compare remaining elements.
5. Return max.
6. Display it.
C Program
#include <stdio.h>

int findMax(int a[], int n) {
    int max = a[0];
    for (int i = 1; i < n; i++)
        if (a[i] > max)
            max = a[i];
    return max;
}

int main(void) {
    int a[100], n;
    printf("Enter number of elements: ");
    scanf("%d", &n);

    printf("Enter elements: ");
    for (int i = 0; i < n; i++)
        scanf("%d", &a[i]);

    printf("Maximum = %d\n", findMax(a, n));
    return 0;
}
Sample Output
Enter number of elements: 5
Enter elements: 12 45 7 31 20
Maximum = 45

Experiment 14: String Functions – Length and Copy
Unit
Unit III – Arrays, Functions and Pointers
Aim
To explore standard string manipulation functions.
Activity / Problem Statement
Read a word, find its length using strlen(), copy it using strcpy(), and display both strings.
Learning Outcome
The student should be able to understand the logic, write the algorithm/pseudocode, implement the C program, compile it, test it, and interpret the output.

Algorithm
1. Read a string.
2. Use strlen() to find length.
3. Use strcpy() to copy the string.
4. Display length and copied string.
C Program
#include <stdio.h>
#include <string.h>

int main(void) {
    char str[100], copy[100];

    printf("Enter a word: ");
    scanf("%99s", str);

    strcpy(copy, str);

    printf("Length = %zu\n", strlen(str));
    printf("Copied string = %s\n", copy);

    return 0;
}
Sample Output
Enter a word: programming
Length = 11
Copied string = programming

Experiment 15: Pointers – Swap Two Numbers
Unit
Unit III – Arrays, Functions and Pointers
Aim
To demonstrate pointers and pass-by-reference behavior.
Activity / Problem Statement
Swap two integer values using a function and pointers.
Learning Outcome
The student should be able to understand the logic, write the algorithm/pseudocode, implement the C program, compile it, test it, and interpret the output.

Algorithm
1. Read a and b.
2. Pass their addresses to swap().
3. Inside swap(), use a temporary variable and dereference the pointers.
4. Display values after swapping.
C Program
#include <stdio.h>

void swap(int *x, int *y) {
    int temp = *x;
    *x = *y;
    *y = temp;
}

int main(void) {
    int a, b;
    printf("Enter two numbers: ");
    scanf("%d %d", &a, &b);

    printf("Before swap: a = %d, b = %d\n", a, b);
    swap(&a, &b);
    printf("After swap : a = %d, b = %d\n", a, b);

    return 0;
}
Sample Output
Enter two numbers: 10 25
Before swap: a = 10, b = 25
After swap : a = 25, b = 10

Experiment 16: Pointers in C – Array Traversal
Unit
Unit IV – Strings, Structure and Union
Aim
To reinforce pointer usage with arrays.
Activity / Problem Statement
Read five integers and traverse the array using a pointer.
Learning Outcome
The student should be able to understand the logic, write the algorithm/pseudocode, implement the C program, compile it, test it, and interpret the output.

Algorithm
1. Read five elements.
2. Set pointer p to the first element.
3. Print *p and increment p until all elements are printed.
C Program
#include <stdio.h>

int main(void) {
    int a[5];
    int *p = a;

    printf("Enter 5 integers: ");
    for (int i = 0; i < 5; i++)
        scanf("%d", &a[i]);

    printf("Elements using pointer: ");
    for (int i = 0; i < 5; i++)
        printf("%d ", *(p + i));

    printf("\n");
    return 0;
}
Sample Output
Enter 5 integers: 10 20 30 40 50
Elements using pointer: 10 20 30 40 50

Experiment 17: Structure – Student Record
Unit
Unit IV – Strings, Structure and Union
Aim
To apply the structure concept in C.
Activity / Problem Statement
Create a Student structure with roll number, name and marks, read the details, and display them.
Learning Outcome
The student should be able to understand the logic, write the algorithm/pseudocode, implement the C program, compile it, test it, and interpret the output.

Algorithm
1. Define struct Student.
2. Declare a structure variable.
3. Read roll number, name and marks.
4. Display all members.
C Program
#include <stdio.h>

struct Student {
    int roll;
    char name[50];
    float marks;
};

int main(void) {
    struct Student s;

    printf("Enter roll number: ");
    scanf("%d", &s.roll);
    printf("Enter name: ");
    scanf("%49s", s.name);
    printf("Enter marks: ");
    scanf("%f", &s.marks);

    printf("\nStudent Details\n");
    printf("Roll  : %d\n", s.roll);
    printf("Name  : %s\n", s.name);
    printf("Marks : %.2f\n", s.marks);

    return 0;
}
Sample Output
Enter roll number: 101
Enter name: Priya
Enter marks: 88.5

Student Details
Roll  : 101
Name  : Priya
Marks : 88.50

Experiment 18: Union – Accessing Union Members
Unit
Unit IV – Strings, Structure and Union
Aim
To execute a program using a union and observe shared memory.
Activity / Problem Statement
Define a union containing int, float and char members. Assign and display one member at a time and observe that assigning another member changes the stored representation.
Learning Outcome
The student should be able to understand the logic, write the algorithm/pseudocode, implement the C program, compile it, test it, and interpret the output.

Algorithm
1. Define a union Data with int, float and char.
2. Assign an integer and display it.
3. Assign a float and display it.
4. Assign a character and display it.
5. Note that all members share the same memory.
C Program
#include <stdio.h>

union Data {
    int i;
    float f;
    char c;
};

int main(void) {
    union Data d;

    d.i = 100;
    printf("Integer = %d\n", d.i);

    d.f = 12.5f;
    printf("Float   = %.2f\n", d.f);

    d.c = 'A';
    printf("Char    = %c\n", d.c);

    printf("Size of union = %zu bytes\n", sizeof(d));
    return 0;
}
Sample Output
Integer = 100
Float   = 12.50
Char    = A
Size of union = 4 bytes

Experiment 19: String Operations – Compare and Concatenate
Unit
Unit IV – Strings, Structure and Union
Aim
To demonstrate common string operations.
Activity / Problem Statement
Read two words, compare them using strcmp(), and concatenate them using strcat().
Learning Outcome
The student should be able to understand the logic, write the algorithm/pseudocode, implement the C program, compile it, test it, and interpret the output.

Algorithm
1. Read two strings.
2. Compare using strcmp().
3. Copy the first string into a result buffer.
4. Concatenate the second string using strcat().
5. Display comparison and result.
C Program
#include <stdio.h>
#include <string.h>

int main(void) {
    char a[100], b[50];

    printf("Enter first word: ");
    scanf("%99s", a);
    printf("Enter second word: ");
    scanf("%49s", b);

    if (strcmp(a, b) == 0)
        printf("Strings are equal\n");
    else
        printf("Strings are different\n");

    strcat(a, b);
    printf("Concatenated string = %s\n", a);

    return 0;
}
Sample Output
Enter first word: hello
Enter second word: world
Strings are different
Concatenated string = helloworld

Experiment 20: Array of Structures – Student Records
Unit
Unit IV – Strings, Structure and Union
Aim
To examine an array of structures in C.
Activity / Problem Sta
