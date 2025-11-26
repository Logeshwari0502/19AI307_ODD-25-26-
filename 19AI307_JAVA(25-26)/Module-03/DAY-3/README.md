# Ex.No:3(C) ABSTRACTION

## QUESTION:
Create an abstract class TaxPayer with method calculateTax(). Create subclasses SalariedPerson and BusinessPerson.
## AIM:
To write a Java program that demonstrates abstraction by creating an abstract class TaxPayer with an abstract method calculateTax(), and implementing it in subclasses SalariedPerson and BusinessPerson to compute tax based on income.

## ALGORITHM :
1. Create an abstract class TaxPayer with an abstract method calculateTax().
2. Create SalariedPerson class that returns 10% of income as tax.
3. Create BusinessPerson class that returns 15% of income as tax.
4. In main(), read choice and income from the user.
5. If choice = 1, create a SalariedPerson object; otherwise create a BusinessPerson object.
6. Call the calculateTax() method.Print the calculated tax.
7. End the program.

## PROGRAM:
 ```
/*
Program to implement a Abstraction using Java
Developed by: LOGESHWARI R
RegisterNumber: 212223060137
*/
```

## SOURCE CODE:
```
import java.util.*;

abstract class TaxPayer {
    abstract double calculateTax();
}

class SalariedPerson extends TaxPayer {
    double income;

    SalariedPerson(double income) {
        this.income = income;
    }

    double calculateTax() {
        return income * 0.10; // 10% tax
    }
}

class BusinessPerson extends TaxPayer {
    double income;

    BusinessPerson(double income) {
        this.income = income;
    }

    double calculateTax() {
        return income * 0.15; // 15% tax
    }
}

public class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int choice = sc.nextInt(); 
        double income = sc.nextDouble();

        TaxPayer person;
        if (choice == 1) {
            person = new SalariedPerson(income);
        } else {
            person = new BusinessPerson(income);
        }

        System.out.printf("%.2f\n", person.calculateTax());
    }
}
```

## OUTPUT:
<img width="447" height="380" alt="image" src="https://github.com/user-attachments/assets/78efdcd1-a68f-4250-97d5-dc1a2c998bbf" />



## RESULT:
The program successfully demonstrates the concept of abstraction and method overriding. 

