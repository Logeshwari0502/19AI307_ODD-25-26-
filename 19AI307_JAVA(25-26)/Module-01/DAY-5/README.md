# Ex.No:1(E) STRINGS AND MATH FUNCTION

## QUESTION:
Write a Java program to reverse a given string.

## AIM:
To write a Java program that reads a string from the user and prints its reverse.

## ALGORITHM :
1. Start the program and create a Scanner object to read input.
2. Read a string from the user and store it in a variable.
3. Use StringBuilder and its reverse() method to reverse the string.
4. Convert the reversed value back to a string.
5. Display the reversed string to the user.
6. End the program.

## PROGRAM:
 ```
/*
Program to implement a Strings and Math Function using Java
Developed by: LOGESHWARI R
RegisterNumber: 212223060137
*/
```

## SOURCE CODE:
```
import java.util.Scanner;

public class ReverseString {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        String str = sc.nextLine();

        String reversed = new StringBuilder(str).reverse().toString();

        System.out.println("Reversed string: " + reversed);

        sc.close();
    }
}
```

## OUTPUT:

<img width="719" height="250" alt="image" src="https://github.com/user-attachments/assets/7a7a1f7e-ba10-4ecb-825d-c451d92aa7bf" />

## RESULT:
The program successfully takes a string input from the user and displays its reversed form.

