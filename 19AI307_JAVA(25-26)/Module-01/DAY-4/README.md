# Ex.No:1(D) ARRAYS

## QUESTION:
Write a Java program to reverse an array
## AIM:
To write a Java program that reads an array of integers and prints the elements in reverse order.

## ALGORITHM :
1. Start the program and create a Scanner object to read input.
2. Read the integer n, representing the size of the array.
3. Declare an integer array of size n.
4. Read n integers from the user and store them in the array.
5. Use a for loop that starts from the last index (n − 1) and moves to the first index (0).
6. Print each array element in reverse order.
7. End the program.
## PROGRAM:
 ```
/*
Program to implement a Array concept using Java
Developed by: LOGESHWARI R
RegisterNumber: 212223060137
*/
```

## SOURCE CODE:
```
import java.util.Scanner;

public class ReverseArray {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        int n = sc.nextInt();  
        int[] arr = new int[n];

        for (int i = 0; i < n; i++) {
            arr[i] = sc.nextInt();
        }

        sc.close();

        for (int i = n - 1; i >= 0; i--) {
            System.out.print(arr[i]);
            if (i != 0) {
                System.out.print(" ");
            }
        }
    }
}
```

## OUTPUT:

<img width="768" height="552" alt="image" src="https://github.com/user-attachments/assets/2b0f0fd2-c45b-466c-8d8b-6dea60ce6bac" />


## RESULT:
The Java program successfully reads an array of integers and displays the elements in reverse order.

