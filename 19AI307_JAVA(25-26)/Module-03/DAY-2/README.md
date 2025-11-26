# Ex.No:3(b) POLYMORPHISM

## QUESTION:
Write a Java program that calculates the area of different shapes using method overloading. Create a class AreaCalculator with area(int side) for square area(int length, int breadth) for rectangle area(double radius) for circle
## AIM:
To write a Java program that demonstrates method overloading by calculating the area of a square, rectangle, and circle using overloaded area() methods.

## ALGORITHM :
1. Start the program by defining a class AreaCalculator.
2. Implement an overloaded method area(int side) to calculate the area of a square.
3. Implement another overloaded method area(int length, int breadth) to calculate the area of a rectangle.
4. Implement a third overloaded method area(double radius) to calculate the area of a circle.
5. In the Main class, create a Scanner object to read inputs from the user.
6. Read the side of a square , length and breadth of a rectangle , radius of a circle and  to display the area.
7. Display all the calculated areas.
8. End the program.


## PROGRAM:
 ```
/*
Program to implement a Polymorphism using Java
Developed by: LOGESHWARI R
RegisterNumber: 212223060137
*/
```

## SOURCE CODE:
```
import java.util.Scanner;

class AreaCalculator {
    public int area(int side) {
        return side * side;
    }
    public int area(int length, int breadth) {
        return length * breadth;
    }
    public double area(double radius) {
        return Math.PI * radius * radius;
    }
}

public class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        AreaCalculator calc = new AreaCalculator();

        int side = sc.nextInt();
        System.out.println("Area of square: " + calc.area(side));

        int length = sc.nextInt();
        int breadth = sc.nextInt();
        System.out.println("Area of rectangle: " + calc.area(length, breadth));

        double radius = sc.nextDouble();
        System.out.println("Area of circle: " + calc.area(radius));

        sc.close();
    }
}
```


## OUTPUT:
<img width="844" height="376" alt="image" src="https://github.com/user-attachments/assets/b6160238-2c34-4329-8614-045fd5c9f543" />


## RESULT:
The program successfully demonstrates method overloading by using different versions of the area() method to compute and display the area of a square, rectangle, and circle based on user input.

