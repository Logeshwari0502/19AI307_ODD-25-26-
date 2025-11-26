# Ex.No:1(B) CONDITIONAL STATEMENT

## QUESTION:
A pirate ship has a code lock that only opens if:
The input code is even, and
If it is less than 100, say "Weak Code".
If it is between 100 and 999, say "Strong Code".
If the code is odd, deny access.

## AIM:
To write a Java program that checks an input number and displays whether it is a Weak Code, Strong Code, or Access Denied.

## ALGORITHM :
1.	Start the program.
2.	Import the necessary package 'java.util'
3.	Inside the class, define the main method (public static void main(String[] args)).
4. Create a Scanner object to read an integer input from the user.
5. Check whether the number is even using the condition a % 2 == 0.
6. If the number is even:
   Check if the number is less than 100; if true, print “Weak Code”.
   Else, check if the number is between 100 and 999; if true, print “Strong Code”.
7. Otherwise, print “Access Denied”.
8. If the number is odd, directly print “Access Denied”.
9. End the program.

## PROGRAM:
 ```
/*
Program to implement a conditional statement using Java
Developed by: LOGESHWARI R
RegisterNumber: 212223060137
*/
```

## SOURCE CODE:
```
import java.util.*;

public class ship{
    public static void main(String[] args){
        Scanner sc=new Scanner(System.in);
        int a=sc.nextInt();
        if (a%2==0){
            if (a<100){
                System.out.println("Weak Code");
            }
            else if(100<a && a<999){
                System.out.println("Strong Code");
            }
            else{
                System.out.println("Access Denied");
            }
        }
        else{
            System.out.println("Access Denied");
        }
    }
}
```
## OUTPUT:
<img width="829" height="308" alt="image" src="https://github.com/user-attachments/assets/3eabec33-0cd8-468e-98a2-8433177b8584" />

## RESULT:
The Java program successfully reads an integer input and correctly identifies it as Weak Code, Strong Code, or Access Denied based on the given conditions.

