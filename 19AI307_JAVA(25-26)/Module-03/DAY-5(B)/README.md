# Ex.No:3(F) WRAPPER CLASS

## QUESTION:
Write a Java program to check if a number is an Armstrong number using Math.pow() and the Integer wrapper class. Take input from the user.

## AIM:
To write a Java program that checks whether a number is an Armstrong number using wrapper class

## ALGORITHM :
Step 1: Start.

Step 2: Read a number from the user.

Step 3: Store the number in another variable for later comparison.

Step 4: Count how many digits the number has.

Step 5: Set a variable to hold the sum of powered digits and initialize it to zero.

Step 6: Repeat the following steps until the number becomes zero:
    • Take the last digit of the number.
    • Raise this digit to the power equal to the total number of digits.
    • Add the result to the sum variable.
    • Remove the last digit from the number.

Step 7: Compare the calculated sum with the original number.

Step 8: If both are equal, display that the number is an Armstrong number.
Otherwise, display that it is not an Armstrong number.

Step 9: Stop the program.

## PROGRAM:
 ```
/*
Program to implement a Wrapper Class using Java
Developed by: LOGESHWARI R
RegisterNumber: 212223060137
*/
```

## SOURCE CODE:
```
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        int num = scanner.nextInt();
        scanner.close();

        int originalNum = num;
        int sum = 0;
        int digitCount = String.valueOf(num).length();

        while (num > 0) {
            int digit = num % 10;
            sum += (int) Math.pow(digit, digitCount);
            num /= 10;
        }

        if (sum == originalNum) {
            System.out.println(originalNum + " is an Armstrong number.");
        } else {
            System.out.println(originalNum + " is not an Armstrong number.");
        }
    }
}
```


## OUTPUT:
<img width="852" height="250" alt="image" src="https://github.com/user-attachments/assets/24ec1316-6f89-4924-ab2c-ac0ee721e434" />



## RESULT:
The program successfully checks whether the given number is an Armstrong number  wrapper class.

