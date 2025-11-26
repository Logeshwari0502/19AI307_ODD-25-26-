# Ex.No:1(C) LOOPING STATEMENT

## QUESTION:
Write a Java program to calculate the factorial of a number using a for loop. The factorial of n is the product of all positive integers less than or equal to n.

## AIM:
To write a Java program that calculates the factorial of a given number using a for loop.

## ALGORITHM :
1.	Start the program.
2.	Import the necessary package 'java.util'
3.	Initialize fact = 1.
4. Use a for loop from i = n down to 1.
5. Multiply fact = fact * i in each iteration.
6. After the loop, print the value of fact.
7. End the program.
## PROGRAM:
 ```
/*
Program to implement a Looping Statement using Java
Developed by: Harini S
RegisterNumber: 212223240048
*/
```

## SOURCE CODE:
```
import java.util.*;
public class Main{
    public static void main(String args[]){
        int n,fact = 1;
        Scanner in = new Scanner(System.in);
        n = in.nextInt();
        for(int i=n;i>0;i--){
            fact=fact*i;
        }
        System.out.println("Factorial of "+n+" is: "+fact);
    }
}
```
## OUTPUT:
<img width="728" height="264" alt="image" src="https://github.com/user-attachments/assets/9dd32131-ac68-4ac8-9d76-c3dea0034481" />

## RESULT:
The Java program successfully reads a number from the user and correctly calculates its factorial using a for loop.

