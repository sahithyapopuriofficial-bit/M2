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
<img width="1016" height="620" alt="image" src="https://github.com/user-attachments/assets/b18c7559-cea1-41a2-b06d-587cefaab723" />

## OUTPUT:
<img width="577" height="257" alt="image" src="https://github.com/user-attachments/assets/c2996da8-0bfa-451e-9b20-ce61952d6f6e" />










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
<img width="841" height="825" alt="image" src="https://github.com/user-attachments/assets/0fb5a5c6-5589-405c-ba13-3aef3d1e6f68" />

## OUTPUT:
<img width="411" height="346" alt="image" src="https://github.com/user-attachments/assets/6ba778bc-2069-452a-b6d6-92d682baddc9" />





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
<img width="1280" height="705" alt="image" src="https://github.com/user-attachments/assets/6bb3f2c7-a76c-4d6d-a498-f280ab00456b" />

## OUTPUT:
<img width="581" height="273" alt="image" src="https://github.com/user-attachments/assets/844b09ef-8a1f-427b-b2b4-23b8d53b2ce9" />






## RESULT:

Thus the program to perform addition and subtraction of two numbers using functions has been executed successfully
 
 


# EX-09-Use For Loop

## AIM:

Write a c program to find the sum of digits using for loop

## ALGORITHM:

1.	Declare variables to store the input number and the sum of digits.
2.	Initialize the sum of digits to 0.
3.	Use a for loop to iterate through each digit of the input number.
4.	Inside the loop, extract the rightmost digit of the number (using the modulo operator % and division by 10).
5.	If the digit is odd, add it to the sum of digits.
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
<img width="739" height="667" alt="image" src="https://github.com/user-attachments/assets/dba0f54f-1a28-480e-90ca-409fdcbdabe4" />


## OUTPUT:
<img width="409" height="285" alt="image" src="https://github.com/user-attachments/assets/8216f8f4-c7c5-4816-8923-e80ece1520ac" />




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
<img width="1145" height="623" alt="image" src="https://github.com/user-attachments/assets/61c1382a-00ec-4126-a024-75781233e7aa" />


## OUTPUT:
<img width="692" height="266" alt="image" src="https://github.com/user-attachments/assets/2fb40ad6-0568-46ec-9415-cd9ddf935bc1" />

## RESULT:
The program correctly computes the factorial of a given number using a separate function and displays the result.
 
