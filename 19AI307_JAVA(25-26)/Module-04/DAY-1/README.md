# Ex.No:4(A) EXCEPTION HANDLING

## QUESTION:
Write a program that reads two integers and divides the first by the second. Handle the case when division by zero occurs.

## AIM:
To write a Java program that reads two integers from the user and performs division, while handling the exception

## ALGORITHM :
1.	Start the program.
2.	Import the necessary package 'java.util'. Read two integers from the user

Step 3: Try to divide the first integer by the second.

Step 4: If the second integer is not zero:
    • Perform the division.
    • Display the result.

Step 5: If division by zero occurs:
    • Display an error message saying that division by zero is not allowed.

Step 6: Stop the program



## PROGRAM:
 ```
/*
Program to implement a Exception Handling using Java
Developed by: LOGESHWARI R
RegisterNumber: 212223060137
*/
```

## SOURCE CODE:
```
import java.util.*;
class prog{
    public static void main(String args[]){
        Scanner in=new Scanner(System.in);
        int a,b;
        try{
            a=in.nextInt();
            b=in.nextInt();
            System.out.println("Result: "+a/b);
        }
        catch(Exception e){
            System.out.println("Error: Division by zero");
        }
    }
}
```

## OUTPUT:

<img width="692" height="309" alt="image" src="https://github.com/user-attachments/assets/0ee3fbc6-decc-4341-bc8a-48dee91d7238" />


## RESULT:
The program successfully reads two integers, performs division, and correctly handles division-by-zero errors

