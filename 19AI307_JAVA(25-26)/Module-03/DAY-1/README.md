# Ex.No:3(A) INHERITANCE AND AGGREGATION

## QUESTION:
Create a Super class Person with fields name and age. Create a subclass Student that inherits from Person and adds a field marks (integer). Implement a method in Student called calculateGrade() which returns the grade based on the marks:

Marks ≥ 90: Grade A

Marks ≥ 75 and < 90: Grade B

Marks ≥ 50 and < 75: Grade C

Marks < 50: Grade F

## AIM:
To write a Java program that demonstrates inheritance by creating a superclass Person and a subclass Student. The Student class should include marks and a method calculateGrade() to determine the grade based on the marks.

## ALGORITHM :
1. Start the program by defining a superclass Person with fields name and age.
2. Create a constructor in Person to initialize these fields.
3. Define a subclass Student that extends Person and adds an integer field marks.
4. Create a constructor in Student that calls the superclass constructor using super() and initializes marks.
5. Implement a method calculateGrade() in Student that returns:"A" if marks ≥ 90"B" if marks ≥ 75 and < 90"C" if marks ≥ 50 and < 75"F" if marks < 50
6. Define a method displayStudent() to print the student details and grade.
7. In the prog class, read name, age, and marks from the user.
8. Create a Student object using the input values.
9. Call displayStudent() to show all details and the calculated grade.
10. End the program.

## PROGRAM:
 ```
/*
Program to implement a Inheritance and Aggregation using Java
Developed by: LOGESHWARI R
RegisterNumber: 212223060137
*/
```

## SOURCE CODE:
```

import java.util.Scanner;

class Person {
    String name;
    int age;

    Person(String name, int age) {
        this.name = name;
        this.age = age;
    }
}

class Student extends Person {
    int marks;

    Student(String name, int age, int marks) {
        super(name, age);
        this.marks = marks;
    }

    String calculateGrade() {
        if (marks >= 90) return "A";
        else if (marks >= 75) return "B";
        else if (marks >= 50) return "C";
        else return "F";
    }

    void displayStudent() {
        System.out.println("Name: " + name);
        System.out.println("Age: " + age);
        System.out.println("Marks: " + marks);
        System.out.println("Grade: " + calculateGrade());
    }
}W

class prog {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        String name = sc.nextLine();
        int age = sc.nextInt();
        int marks = sc.nextInt();
        Student s = new Student(name, age, marks);
        s.displayStudent();
    }
}
```

## OUTPUT:

<img width="705" height="583" alt="image" src="https://github.com/user-attachments/assets/d8cd6e74-6050-41bd-a2cd-34432e94c2e2" />


## RESULT:
The program successfully demonstrates inheritance by extending the Person class into the Student class. It correctly reads student details, calculates the grade based on marks, and displays the complete student information.

