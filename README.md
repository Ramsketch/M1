
# EX-01-Datatypes-Operators
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
    char ch1, ch2, ch3;
    scanf(" %c", &ch1); 
    scanf(" %c", &ch2);
    scanf(" %c", &ch3);
    printf("Characters in reverse order: %c %c %c\n", ch3, ch2, ch1);
    return 0;
}

```

## OUTPUT:
<img width="1917" height="1025" alt="Screenshot 2025-10-22 144808" src="https://github.com/user-attachments/assets/ccd6a936-9113-48b0-a721-ddf6320e67bd" />

## RESULT:
Thus the program to read 3 characters one by one and print the characters in a reverse order has been executed successfully.


# EX-02- Conditional-Statements
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
int main() 
{
    int A;
    scanf("%d", &A);
    if (A > 0) 
    {
        printf("%d is a positive number.\n", A);
    }
    else 
    {
        printf("%d is not a positive number.\n", A);
    }
    return 0; 
}

```

# OUTPUT:
<img width="1918" height="1031" alt="Screenshot 2025-10-22 145006" src="https://github.com/user-attachments/assets/0796659a-18ae-447b-8c0e-ebaa49e5b37f" />
<img width="1913" height="1022" alt="Screenshot 2025-10-22 145023" src="https://github.com/user-attachments/assets/130abb98-1d9f-4eaf-8cba-c87a48a0a624" />

# RESULT:
Thus the program to read A values and check whether A is positive number or not has been executed successfully.
 
 
# EX-03- Operators-Expressions
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
int main() 
{
   
    int num1, den1, num2, den2;
    float a,b,min;
    printf("Enter numerator and denominator of first fraction: ");
    scanf("%d %d", &num1, &den1);
    printf("Enter numerator and denominator of second fraction: ");
    scanf("%d %d", &num2, &den2);
    a = (float)num1 / den1;
    b = (float)num2 / den2;
    min = (a < b) ? a : b;
    printf("Minimum fraction value is: %.2f\n", min);
    return 0;
}

```

## OUTPUT:
<img width="1919" height="1032" alt="Screenshot 2025-10-22 150221" src="https://github.com/user-attachments/assets/317d7046-b8eb-43c6-909a-6d122079ed3c" />


## RESULT:
Thus the program to find minimum between two fraction numbers using conditional operator or ternary operator has been executed successfully.


# EX-04- Using Conditional Statements

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
int main() 
{
    int value;
    scanf("%d",&value);
    if (value == 1) 
    {
        printf("The input value is equal to 1.\n");
    } 
    else
    {
        printf("The input value is not equal to 1.\n");
    }
    return 0;
}

```

## OUTPUT:
<img width="1919" height="1031" alt="Screenshot 2025-10-22 150513" src="https://github.com/user-attachments/assets/e6809b96-f754-446d-b611-68818381a1f6" />
<img width="1919" height="1032" alt="Screenshot 2025-10-22 150529" src="https://github.com/user-attachments/assets/2df31385-bb4b-4191-b021-c6f65dbbc2f2" />



## RESULT:
Thus the program to check whether the input value is equal to 1 using simple if statement has been executed successfully



# EX-05- Calculating Total, Percentage, And Division Using Conditional Statements 
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
int main() 
{
    int m1, m2, m3;
    float tot, per;      
    printf("Enter marks of three subjects: ");
    scanf("%d %d %d", &m1, &m2, &m3);
    tot = m1 + m2 + m3;
    per = tot / 3;
    printf("Total Marks = %.2f\n", tot);
    printf("Percentage = %.2f\n", per);
    if (m1 >= 40 && m2 >= 40 && m3 >= 40) 
    {
        if (per >= 60)
        printf("Division = First\n");
        else if (per >= 48)
        printf("Division = Second\n");
        else if (per >= 36)
        printf("Division = Pass\n");
        else
        printf("Division = Fail\n"); 
    } 
    else
    {
        printf("Division = Fail\n");
    }
    return 0;
}

```

## OUTPUT:
<img width="1919" height="1030" alt="Screenshot 2025-10-22 151026" src="https://github.com/user-attachments/assets/f9b838bc-f19b-4ca3-ad60-a77ad53870fa" />
<img width="1919" height="1029" alt="Screenshot 2025-10-22 151123" src="https://github.com/user-attachments/assets/2a7fc0ee-8170-4e5f-b02a-4be5a30ae67e" />
<img width="1919" height="1040" alt="Screenshot 2025-10-22 151213" src="https://github.com/user-attachments/assets/4da3f59f-f40f-462f-afeb-2151e17faa94" />
<img width="1917" height="1037" alt="Screenshot 2025-10-22 151233" src="https://github.com/user-attachments/assets/4a038f8f-f3fe-4ef7-9647-a56346b7ba49" />

## RESULT:
The program successfully takes three subject marks, calculates the total and percentage, and correctly determines the division based on predefined grading logic.

