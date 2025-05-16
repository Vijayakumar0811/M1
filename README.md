# EX-01-Datatypes-Operators
NAME: VIJAYAKUMAR S

REG NO: 212224040359
## AIM:
Write a C program to read 3 characters one by one and print the characters in a reverse order.

## ALGORITHM:
1.	Declare three character variables to store the input characters.
2.	Use the scanf function to read the characters one by one from the user.
3.	Print the characters in reverse order using the printf function.
4.	End the program.

## PROGRAM:
```
#include <stdio.h>
int main()
{
    char a,b,c;
    scanf("%c%c%c",&a,&b,&c);
    printf("The reverse of %c%c%c is %c%c%c\n",a,b,c,c,b,a);
    return 0;    
}
```
## OUTPUT:

![Screenshot 2025-04-27 102250](https://github.com/user-attachments/assets/496a0e50-850c-4d5e-9c2c-f398e872b02c)


## RESULT:
Thus the program to read 3 characters one by one and print the characters in a reverse order has been executed successfully.


# EX-02- Conditional-Statements
NAME: VIJAYAKUMAR S

REG NO: 212224040359
## AIM:
Write a C program to read A values and check whether A is positive number or not.

# ALGORITHM:
1.	Declare a variable to store the input value A.
2.	Use the scanf function to read the value of A from the user.
3.	Check if the value of A is greater than zero.
4.	If A is greater than zero, print a message indicating that it's a positive number. 
5.	Otherwise, print a message indicating that it's not a positive number.
6.End the program.

# PROGRAM:
```
#include <stdio.h>
int main() {
    int A; 
    printf("Enter a number: ");
    scanf("%d", &A); 
    if (A > 0) {
        printf("%d is a positive number.\n", A);
    } else {
        printf("%d is not a positive number.\n", A);
    }
    return 0;
}
```
# OUTPUT:
<img width="317" alt="image" src="https://github.com/user-attachments/assets/27a1da9d-72ac-4780-a584-51e7aca03faf" />

# RESULT:
Thus the program to read A values and check whether A is positive number or not has been executed successfully.
 
 
 


# EX-03- Operators-Expressions
NAME: VIJAYAKUMAR S

REG NO: 212224040359
## AIM:
Write a program to find minimum between two fraction numbers using conditional operator or ternary operator.

## ALGORITHM:
1.	Declare variables to store the two fraction numbers and the result.
2.	Use the printf function to prompt the user to enter the first fraction number (numerator and denominator separately).
3.	Use the scanf function to read the numerator and denominator of the first fraction.
4.	Repeat steps 2 and 3 to get the second fraction from the user.
5.	Calculate the decimal values of both fractions by dividing the numerators by the denominators.
6.	Use the conditional (ternary) operator to compare the decimal values and store the minimum value in the result variable.
7.	Print the minimum value.

## PROGRAM:
```
#include <stdio.h>
int main() {
    int num1, den1, num2, den2;
    float fraction1, fraction2, min;
    printf("Enter numerator and denominator of first fraction: ");
    scanf("%d%d", &num1, &den1);
    printf("Enter numerator and denominator of second fraction: ");
    scanf("%d%d", &num2, &den2);
    fraction1 = (float)num1 / den1;
    fraction2 = (float)num2 / den2;
    min = (fraction1 < fraction2) ? fraction1 : fraction2;
    printf("Minimum of the two fractions = %.2f\n", min);
    return 0; 
}

```
## OUTPUT:

<img width="239" alt="image" src="https://github.com/user-attachments/assets/b5059cc3-91b1-4d9c-b5fc-58e6daceb3cd" />

## RESULT:
Thus the program to find minimum between two fraction numbers using conditional operator or ternary operator has been executed successfully.




# EX-04- Using Conditional Statements
NAME: VIJAYAKUMAR S

REG NO: 212224040359
## AIM:
Write a C program to check whether the input value is equal to 1 using simple if statement

## ALGORITHM:
1.	Declare a variable to store the input value.
2.	Use the scanf function to read the input value from the user.
3.	Use an if statement to check if the input value is equal to 1.
4.	If the condition in the if statement is true, print a message indicating that the input value is equal to 1.
5.	Otherwise, print a message indicating that it's not equal to 1.
6.	End the program.

## PROGRAM:
```
#include <stdio.h>
int main() {
    int value;
    printf("Enter a number: ");
    scanf("%d", &value);
    if (value == 1) {
        printf("The input value is equal to 1.\n");
    } else {
        printf("The input value is not equal to 1.\n");
    }
    return 0;
}
```
## OUTPUT:

<img width="320" alt="image" src="https://github.com/user-attachments/assets/f190b500-d114-4c16-8241-face2aab1847" />

## RESULT:
Thus the program to check whether the input value is equal to 1 using simple if statement has been executed successfully



# EX-05- Calculating Total, Percentage, And Division Using Conditional Statements 
NAME: VIJAYAKUMAR S

REG NO: 212224040359
## AIM:
To write a C program that reads marks of three subjects, calculates the total and percentage, and then determines the division (First, Second, Pass, or Fail) based on the percentage and minimum marks criteria.
## ALGORITHM:
1.	Start
2.	Declare integer variables m1, m2, m3 for marks, and float variables tot, per.
3.	Input the marks for three subjects.
4.	Calculate total marks: tot = m1 + m2 + m3
5.	Calculate percentage: per = tot / 3
6.	Display total and percentage.
7.	Check if all marks are greater than or equal to 40:
8.	If yes:
a.	If percentage >= 60: Print “Division = First”
b.	Else if percentage >= 48: Print “Division = Second”
c.	Else if percentage >= 36: Print “Division = Pass”
9.	Else: Print “Division = Fail”
10.	End
## PROGRAM:
```
#include <stdio.h>
int main() {
    int m1, m2, m3;
    float tot, per;
    printf("Enter marks for three subjects: ");
    scanf("%d%d%d", &m1, &m2, &m3);
    tot = m1 + m2 + m3;
    per = tot / 3;
    printf("Total Marks = %.2f\n", tot);
    printf("Percentage = %.2f%%\n", per);
    if (m1 >= 40 && m2 >= 40 && m3 >= 40) {
        if (per >= 60) {
            printf("Division = First\n");
        } else if (per >= 48) {
            printf("Division = Second\n");
        } else if (per >= 36) {
            printf("Division = Pass\n");
        }
    } else {
        printf("Division = Fail\n");
    }
    return 0;
}
```

## OUTPUT:
<img width="316" alt="image" src="https://github.com/user-attachments/assets/86b6d40b-8323-4e62-beab-9bb245809d3a" />

## RESULT:
The program successfully takes three subject marks, calculates the total and percentage, and correctly determines the division based on predefined grading logic.

