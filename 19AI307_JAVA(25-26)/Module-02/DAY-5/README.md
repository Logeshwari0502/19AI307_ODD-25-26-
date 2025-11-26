# Ex.No:2(E) ACCESS MODIFIERS

## QUESTION:
Create a class Calculator with: One non-static method add(int a, int b) that returns the sum, One static method info() that says "Calculator is ready".
## AIM:
To write a Java program that demonstrates the use of static and non-static methods in a class called Calculator. The program should use a non-static add() method to compute the sum of two numbers and a static info() method to display a message.

## ALGORITHM :
1. Start the program by defining a class Calculator.
2. Inside the class, define a non-static method add(int a, int b) that returns the sum of two numbers.
3. Define a static method info() that prints "Calculator is ready".
4. In the prog class, create a Scanner object to read two integers from the user.
5. Call the static method Calculator.info() directly using the class name.
6. Create an object of the Calculator class.
7. Call the non-static method add(a, b) using the object and store the result.
8. End the program.


## PROGRAM:
 ```
/*
Program to implement a Access Modifiers using Java
Developed by: LOGESHWARI R
RegisterNumber: 212223060137
*/
```

## SOURCE CODE:
```
import java.util.Scanner;

class Calculator {
    int add(int a, int b) {
        return a + b;
    }

    static void info() {
        System.out.println("Calculator is ready");
    }
}

class prog {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int a = sc.nextInt();
        int b = sc.nextInt();

        Calculator.info();

        Calculator c = new Calculator();
        int result = c.add(a, b);

        System.out.println("Sum: " + result);
    }
}
```

## OUTPUT:
<img width="708" height="319" alt="image" src="https://github.com/user-attachments/assets/08969023-956c-4394-99d6-974b20e9e2ba" />


## RESULT:
The program successfully demonstrates accessing a static method using the class name and calling a non-static method using an object. It correctly displays the message and computes the sum of two numbers.

