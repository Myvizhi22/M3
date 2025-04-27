# EX-11-EMI-CALCULATOR

## AIM

To write a program to prepare EMI calculator using function without return type and with arguments.

## ALGORITHM

1.	Start the program.
2.	Read principal amount, rate of interest and months.
3.	Pass these values as arguments to function.
4.	Calculate EMI using the formula, amt=(prpow(1+r,t))/(pow(1+r,t)-1)
5.	Display the result.
6.	Stop the program.

## PROGRAM
```c
#include <stdio.h>
#include <math.h>
void calculateEMI(float principal, float annualInterestRate, int months) {
    float R = annualInterestRate / (12 * 100);
    float EMI = (principal * R * pow(1 + R, months)) / (pow(1 + R, months) - 1);
    printf("The EMI is: %.2f\n", EMI);
}

int main() {
    float principal, annualInterestRate;
    int months;
    printf("Enter the loan amount (Principal): ");
    scanf("%f", &principal);
    printf("Enter the annual interest rate (in percentage): ");
    scanf("%f", &annualInterestRate);
    printf("Enter the number of months: ");
    scanf("%d", &months);
    calculateEMI(principal, annualInterestRate, months);

    return 0;
}

```

## OUTPUT
![image](https://github.com/user-attachments/assets/2360be59-2741-46ff-96bd-79ed1607668c)





## RESULT

Thus the program to prepare EMI calculator using function without return type with arguments has been executed successfully
 
 


# EX-12-FIBONACCI-SERIES
## AIM
To write a C program to generate the Fibonacci series for the value 6.

## ALGORITHM
1.	Start the program.
2.	Read number of terms to display.
3.	Add the previous two terms and store it in new term.
4.	Assign 2nd term to 1st term and 3rd term to 2nd term.
5.	Repeat steps 3 and 4 n number of times.
6.	Display the result.
7.	Stop the program.

## PROGRAM
```c
#include <stdio.h>
int main() {
    int n = 6, first = 0, second = 1, next, i;
    printf("Fibonacci Series for %d terms: \n", n);
    printf("%d, ", first);
    printf("%d, ", second);
    for (i = 3; i <= n; i++) {
        next = first + second;
        printf("%d", next);
        first = second;
        second = next;
        if (i < n) {
            printf(", ");
        }
    }

    printf("\n"); 
    return 0;
}

```
## OUTPUT

![image](https://github.com/user-attachments/assets/a28996f4-7599-480e-b8ce-86cc281132b4)







## RESULT
Thus the program to generate the Fibonacci series for the value 6 has been executed successfully.
 
 


# EX-13-ONE-DIMENSIONAL-ARRAY
## AIM
To write a C program to read n elements as input and print the last element of the array.

## ALGORITHM
1.	Start the program.
2.	Read a variable.
3.	Read the array values n number of times.
4.	Print the last element.
5.	Stop the program.

## PROGRAM
```c
#include <stdio.h>
int main() {
    int n;
    printf("Enter the number of elements: ");
    scanf("%d", &n);
    int arr[n];
    printf("Enter %d elements:\n", n);
    for (int i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
    }
    printf("The last element of the array is: %d\n", arr[n - 1]);

    return 0;
}

```
## OUTPUT

![image](https://github.com/user-attachments/assets/5219ed39-e66c-4e68-b16c-4ac48df3f713)








## RESULT
Thus the program to read n elements as input and print the last element of the array has been executed successfully.
 
 


# EX-14-POSITIVE-ARRAY-ELEMENTS
## AIM
To write a C Program to count total number of positive elements in an array.

## ALGORITHM
1.	Start the program.
2.	Read a variable.
3.	Read the array values n number of times.
4.	If the array value can be divided by 2 then increment count by 1.
5.	Display result.
6.	Stop the program.

## PROGRAM
```c
#include <stdio.h>

int main() {
    int n, count = 0;
    printf("Enter the number of elements: ");
    scanf("%d", &n);
    int arr[n];
    printf("Enter %d elements:\n", n);
    for (int i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
    }
    for (int i = 0; i < n; i++) {
        if (arr[i] > 0) {
            count++;
        }
    }

    printf("Total number of positive elements: %d\n", count);

    return 0;
}

```

## OUTPUT
![image](https://github.com/user-attachments/assets/ac71a91c-f07f-4465-8c75-c47ccb3db348)





## RESULT
Thus the program to count total number of positive elements in an array has been executed successfully.





 
 


# EX -15 - Replace All Even Elements With 'E' In One Dimensional Array

## Aim:
To write a C program to replace all even elements with 'E' in one dimensional array

## Algorithm:
1.	Input the array:
  Read the size of the array.
  Input the elements of the array.
2.	Iterate through the array:
 	For each element of the array, check if the element is even (i.e., if the element modulo 2 equals 0).
3.	Replace even elements with 'E':
     If an element is even, replace that element with the character 'E'.
4.	Output the updated array:
 Print the updated array after replacements.

## Program:
```c
#include <stdio.h>
int main() {
    int n;
    printf("Enter the number of elements: ");
    scanf("%d", &n);
    int arr[n];
    printf("Enter %d elements:\n", n);
    for (int i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
    }
    printf("Modified array with even elements replaced by 'E':\n");
    for (int i = 0; i < n; i++) {
        if (arr[i] % 2 == 0) {
            printf("E ");
        } else {
            printf("%d ", arr[i]);
        }
    }

    printf("\n");
    return 0;
}

```
## Output:
 ![image](https://github.com/user-attachments/assets/73c703ad-f999-418c-b268-be2a53c3079c)



## Result:

Thus, the program to replace all even elements with 'E' in one dimensional array was verified successfully.



