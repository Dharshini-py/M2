# EX-06 - Looping
## AIM:
Write a C program to print even numbers ranging from M to N (including M and N values).

## ALGORITHM:
1.	Declare two integer variables to store the values of M and N.
2.	Use the printf function to prompt the user to enter the values of M and N.
3.	Use the scanf function to read the values of M and N from the user.
4.	Use a loop (for or while) to iterate from M to N.
5.	Inside the loop, check if the current number is even.
6.	If the current number is even, print it.
7.	Continue the loop until you have iterated through all numbers from M to N.

## PROGRAM:
```
#include<stdio.h>
int main()
{
    int A,B;
    scanf("%d%d",&A,&B);
    for(int i=A;i<=B;i++){
        if(i%2==0){
            printf("%d ",i);
        }
    }
    return 0;
}
```
<img width="1016" height="620" alt="image" src="https://github.com/user-attachments/assets/0184a2b9-2e30-41bc-9d90-33aae3234e07" />


## OUTPUT:
<img width="577" height="257" alt="image" src="https://github.com/user-attachments/assets/2b289499-901e-4405-bcec-e5e16cf363b8" />










## RESULT:
Thus the program to print even numbers ranging from M to N (including M and N values) has been executed successfully
 
 


# EX-07-Nested-loop

## AIM:

Write a C program to print the given triangular pattern using loop.

## ALGORITHM:

1.	Declare a variable to store the number of rows in the triangle.
2.	Use the printf function to prompt the user to enter the number of rows.
3.	Use a loop (for or while) to iterate through each row.
4.	Inside the loop, use another loop to print the desired number of asterisks for each row.
5.	Continue the loop until you have printed the entire triangular pattern.

## PROGRAM:
```
#include <stdio.h>
int main()
{
    int A;
    scanf("%d",&A);
    for(int i=A;i>=1;i--){
        for(int j=i;j>=1;j--){
            printf("$");
        }
        printf("\n");
    }
    return 0;
}
```
<img width="841" height="825" alt="image" src="https://github.com/user-attachments/assets/b013891e-d675-44f2-82f2-2dd81b797a0e" />



## OUTPUT:
<img width="411" height="346" alt="image" src="https://github.com/user-attachments/assets/17380221-6138-421e-82eb-5bd109e72f5a" />





## RESULT:

Thus the program to print the given triangular pattern using loop has been executed successfully
 
 


# EX-08-Functions

## AIM:

Write a C program to perform addition and subtraction of two numbers using functions (with argument and without return type).

## ALGORITHM:

1.	Declare two functions, one for addition and one for subtraction. Both functions should take two integer arguments.
2.	Inside the addition & subtraction function, add & subtract the two numbers and print the result.
3.	In the main function, declare two integer variables and read their values from the user.
4.	Call the addition and subtraction functions, passing the two numbers as arguments.

## PROGRAM:
```
#include <stdio.h>
int add(int n1,int n2){
    int a=n1+n2;
    return a;
}
int sub(int n1,int n2){
    int s=n1-n2;
    return s;
}
int main(){
    int n1,n2;
    scanf("%d",&n1);
    scanf("%d",&n2);
    printf("Addition: %d\n",add(n1,n2));
    printf("Subtraction: %d\n",sub(n1,n2));
    return 0;
}
```
<img width="1280" height="705" alt="image" src="https://github.com/user-attachments/assets/c4795ac4-922b-4bb2-b17d-5ca4f2b9f918" />


## OUTPUT:

<img width="581" height="273" alt="image" src="https://github.com/user-attachments/assets/328a2dd0-8188-47c0-a17c-c32d9af18b09" />





## RESULT:

Thus the program to perform addition and subtraction of two numbers using functions has been executed successfully
 
 


# EX-09-Use For Loop

## AIM:

Write a c program to find the sum of odd digits using for loop

## ALGORITHM:

1.	Declare variables to store the input number and the sum of odd digits.
2.	Initialize the sum of odd digits to 0.
3.	Use a for loop to iterate through each digit of the input number.
4.	Inside the loop, extract the rightmost digit of the number (using the modulo operator % and division by 10).
5.	If the digit is odd, add it to the sum of odd digits.
6.	Print the sum of odd digits.

## PROGRAM:
```
#include <stdio.h>
int main() {
    int num, sum = 0;

    scanf("%d", &num);
    for (; num != 0; num = num / 10) {
        sum += num % 10;
    }
    printf("%d", sum);
    return 0;
}
```
<img width="739" height="667" alt="image" src="https://github.com/user-attachments/assets/69035042-51f7-4911-9303-fe99fd58659e" />

## OUTPUT:
<img width="409" height="285" alt="image" src="https://github.com/user-attachments/assets/63d24c98-07ec-44c9-af3e-13aa3c684d84" />




## RESULT:

Thus the program to find the sum of odd digits using for loop has been executed successfully.




# EX – 10 - Factorial of a Number Using a Function
## AIM:
To write a C program that calculates the factorial of a given number using a user-defined function.
## ALGORITHM:
1.	Start
2.	Declare the function fact().
3.	In the main() function, call the fact() function.
4.	In fact() function:
a.	Declare variables i, N, and fact (initialized to 1).
b.	Read an integer N from the user.
c.	Use a for loop from 1 to N:
i.	Multiply fact by i in each iteration.
d.	After the loop, print the factorial value.
5.	End

## PROGRAM:
```
#include <stdio.h>
void factorial(int n) {
    int i;
    long long fact = 1;
    for(i = 1; i <= n; i++) {
        fact = fact * i;
    }
    printf("Factorial value is: %lld", fact);
}
int main() {
    int num;
    scanf("%d", &num);   
    factorial(num);     
    return 0;
}
```
<img width="1145" height="623" alt="image" src="https://github.com/user-attachments/assets/795ae029-3a0d-4e83-ab93-c3bda5be5ab2" />


## OUTPUT:
<img width="692" height="266" alt="image" src="https://github.com/user-attachments/assets/5e595d89-ca13-4046-b9a3-ee02344b6904" />


## RESULT:
The program correctly computes the factorial of a given number using a separate function and displays the result.

 
