# Ex.No:1(A) INTRODUCTION TO JAVA PROGRAMMING, DATA TYPES, VARIABLES AND OPERATORS

## QUESTION:
Lovely is learning java basics, can you teach her the different types of datatypes in java? Write a program that uses all datatypes and print them all.

## AIM:
To write a Java program to declare, initialize, and print variables of all primitive data types (byte, short, int, long, float, double, boolean, char) and the String class.

## ALGORITHM :
```
1.Start the program by defining a public class, for example, DataTypesDemo.
2.Inside the class, define the main method (public static void main(String[] args)).
3.Declare and initialize variables for each data type using the specified values. (Note: Commas in numbers like 1,34,500 must be removed and written as 134500).
4.Use System.out.println() statements to print the value of each variable to the console, prefixed with a descriptive label (e.g., "Byte Value: ").
5.Compile and run the Java program to observe the output.
```

## PROGRAM:
 ```
/*
Program to implement variables and Operators using Java
Developed by: LOGESHWARI R
RegisterNumber:  212223060137
*/
```

## Sourcecode.java:
```
import java.util.Scanner;
class prog{
    public static void main(String[] args){
        System.out.println("Hey Lovely, let's print all types of data received from user using different data types");
        Scanner sc=new Scanner(System.in);
        byte mybyte=sc.nextByte();
        System.out.println("This is byte datatype "+mybyte);
        short myshort=sc.nextShort();
        System.out.println("This is short datatype "+myshort);
        int myint=sc.nextInt();
        System.out.println("This is int datatype "+myint);
        long mylong=sc.nextLong();
        System.out.println("This is long datatype "+mylong);
        float myfloat=sc.nextFloat();
        System.out.println("This is float datatype "+myfloat);
        double mydouble=sc.nextDouble();
        System.out.println("This is double datatype "+mydouble);
        boolean myboolean=sc.nextBoolean();
        System.out.println("This is boolean datatype "+myboolean);
        char mychar=sc.next().charAt(0);
        System.out.println("This is char datatype "+mychar);
        String mystring=sc.next();
        System.out.println("This is string datatype "+mystring);
        sc.close();
    }
}


```


## OUTPUT:
<img width="1273" height="645" alt="Screenshot 2025-11-10 140114" src="https://github.com/user-attachments/assets/bc584a61-8fdd-493a-bf29-36ed8b0645f2" />



## RESULT:
Thus, the Java program to demonstrate all data types by declaring, initializing, and printing them was successfully compiled and executed.


