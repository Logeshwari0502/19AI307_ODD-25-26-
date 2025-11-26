# Ex.No:4(B)  IMPLEMENT SOLID PRINCIPLES IN JAVA PROGRAM 

## QUESTION:
At an international airport, only one Radar Control Tower exists. This tower is responsible for handling all flight communications regardless of how many flights are coming in. Each incoming flight must contact this tower to register its approach.To ensure safety and consistency, all flights must communicate with the same instance of the tower. If multiple towers are created, it may lead to inconsistent instructions — a huge risk in aviation.Your task is to simulate this system using the Singleton pattern.

## AIM:
To simulate an airport Radar Control Tower system using the Singleton Design Pattern,

## ALGORITHM :
1. Start the program
2. Import required package: java.util.*
3. Define a Singleton class RadarControlTower
4. Create a private static instance of the class, Create a private constructor
5. Create a public static getInstance() method
6. Inside the class, maintain a counter to track registered flights.
7. Define method registerFlight() that: Increments the counter ,Returns the updated count
8. Stop THE PROGRAM

## PROGRAM:
 ```
/*
Program to implement a SOLID Principles in Java Program
Developed by: LOGESHWARI R
RegisterNumber: 212223060137
*/
```

## SOURCE CODE:
```
import java.util.*;

class RadarControlTower {
    private static RadarControlTower instance;
    private int flightCount = 0;

    private RadarControlTower() {}

    public static RadarControlTower getInstance() {
        if (instance == null) {
            instance = new RadarControlTower();
        }
        return instance;
    }

    public int registerFlight(String flightName) {
        flightCount++;
        return flightCount;
    }
}

public class prog {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int n = sc.nextInt();
        sc.nextLine();  // consume newline

        for (int i = 0; i < n; i++) {
            String flight = sc.nextLine();
            RadarControlTower tower = RadarControlTower.getInstance();
            int total = tower.registerFlight(flight);
            System.out.println(flight + " registered with Radar Control Tower. Total Flights: " + total);
        }
    }
}
```


## OUTPUT:

<img width="1247" height="242" alt="image" src="https://github.com/user-attachments/assets/92b54926-f9e2-48bb-8fb2-38aed08a1bdb" />


## RESULT:
The program successfully implements the Singleton pattern by ensuring only one instance of the Radar Control Tower exists

