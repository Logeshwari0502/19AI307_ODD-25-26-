# Ex.No:2(C) ACCESS SPECIFIERS

## QUESTION:
Write a Java program to create a class called Circle with a private instance variable radius. Provide public getter and setter methods to access and modify the radius variable. However, provide two methods called calculateArea() and calculatePerimeter() that return the calculated area and perimeter based on the current radius value. 

## AIM:
To write a Java program that defines a Circle class with a private radius variable, provides getter and setter methods for accessing and modifying the radius, and includes methods to calculate and return the area and perimeter of the circle.

## ALGORITHM :
1. Start the program by defining a class named Circle.
2. Declare a private double variable radius.
3. Create a public getter method getRadius() to return the value of radius.
4. Create a public setter method setRadius(double radius) to update the radius.
5. Define a method calculateArea() that returns the area 
6. Define a method calculatePerimeter() that returns the perimeter 
7. In the Main class, create a Scanner object to read input from the user.
8. Read the radius value and set it using the setter method.
9. Call getRadius(), calculateArea(), and calculatePerimeter() to display the results.
10. End the program.

## PROGRAM:
 ```
/*
Program to implement a Access Specifiers using Java
Developed by: LOGESHWARI R
RegisterNumber: 212223060137
*/
```

## SOURCE CODE:
```
import java.util.Scanner;

class Circle {
    private double radius;

    public double getRadius() {
        return radius;
    }

    public void setRadius(double radius) {
        this.radius = radius;
    }

    public double calculateArea() {
        return Math.PI * radius * radius;
    }

    public double calculatePerimeter() {
        return 2 * Math.PI * radius;
    }
}

public class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        double r = sc.nextDouble();  
        Circle c = new Circle();
        c.setRadius(r);

        System.out.printf("Radius: %.2f\n", c.getRadius());
        System.out.printf("Area: %.2f\n", c.calculateArea());
        System.out.printf("Perimeter: %.2f\n", c.calculatePerimeter());

        sc.close();
    }
}
```


## OUTPUT:

<img width="658" height="312" alt="image" src="https://github.com/user-attachments/assets/c034cfaa-73bc-4b8f-916f-4926b73d9385" />


## RESULT:
The program successfully reads the radius from the user, stores it using setter and getter methods, and correctly calculates and displays the area and perimeter of the circle.

