# Ex.No:2(B) METHODS

## QUESTION:
Write a method named displayMessage() that prints "Welcome to Java Methods!". Call this method from the main() method.

## AIM:
To write a Java program that defines a method to print a welcome message and calls this method from the main() function.

## ALGORITHM :
1. Start the program and define a class
2. Inside the class, define a method displayMessage() that prints "Welcome to Java Methods!".
3. In the main() method, create an object of the class using new.
4. Call the displayMessage() method using the created object.
5. End the program.

## PROGRAM:
 ```
/*
Program to implement a Methods using Java
Developed by: LOGESHWARI R
RegisterNumber: 212223060137
*/
```

## SOURCE CODE:
```
class prog {
    void displayMessage() {
        System.out.println("Welcome to Java Methods!");
    }

    public static void main(String[] args) {
        prog obj = new prog();
        obj.displayMessage();
    }
}
```

## OUTPUT:
<img width="787" height="166" alt="image" src="https://github.com/user-attachments/assets/2f506f6f-0f5a-459a-bb77-6e5f21c8f4b8" />

## RESULT:
The program successfully displays the message "Welcome to Java Methods!" by calling the method through an object.

