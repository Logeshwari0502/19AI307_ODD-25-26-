# Ex.No:2(D) VARIABLE SCOPE AND CONSTRUCTOR

## QUESTION:
Write a program to access a static variable using both class name and object.
## AIM:
To write a Java program that demonstrates how to access a static variable using both the class name and an object.
## ALGORITHM :
1. Start the program by creating a class Demo with a static integer variable staticVar.
2. In the Main class, create a Scanner object to read an integer from the user.
3. Assign the input value to the static variable using the class name (Demo.staticVar).
4. Display the value of the static variable using the class name.
5. Create an object of the Demo class.
6. Access and display the same static variable using the object reference.
7. Close the Scanner and end the program.

## PROGRAM:
 ```
/*
Program to implement a Variable scope and Constructor using Java
Developed by: LOGESHWARI R
RegisterNumber: 212223060137
*/
```

## SOURCE CODE:
```
import java.util.Scanner;

class Demo {
    public static int staticVar = 0;
}

public class Main {
    public static void main(String[] args) {
        Scanner input = new Scanner(System.in);
        Demo.staticVar = input.nextInt();

        System.out.println("Accessing using class name: " + Demo.staticVar);

        Demo obj = new Demo();
        System.out.println("Accessing using object: " + obj.staticVar);

        input.close();
    }
}
```

## OUTPUT:

<img width="791" height="309" alt="image" src="https://github.com/user-attachments/assets/2a2a2bf6-1c99-46f2-9fbb-78d1489acb79" />


## RESULT:

The program successfully accesses the static variable using both the class name and an object, demonstrating that static variables belong to the class and can be accessed in both ways.

