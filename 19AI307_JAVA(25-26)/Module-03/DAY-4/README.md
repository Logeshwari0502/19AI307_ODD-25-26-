# Ex.No:3(D)    INTERFACE 

## QUESTION:
You are programming bots that analyze weather data. Each bot must implement a common interface and give a prediction.
SunBot: Predicts "HOT" if temperature > 30, else "MODERATE".
RainBot: Predicts "COLD" if temperature < 20, else "WARM".

## AIM:
To develop a Java program that uses interfaces to predict weather based on temperature and bot type.

## ALGORITHM :
1. Start the program
2. Read the input temperature.
3. Read the bot type (1 for SunBot, 2 for RainBot).
4. Based on the temperature predict the bot
5. Display the prediction.
6. Stop the program


## PROGRAM:
 ```
/*
Program to implement a Interface using Java
Developed by: LOGESHWARI R
RegisterNumber: 212223060137
*/
```

## SOURCE CODE:
```
import java.util.Scanner;

interface WeatherBot {
    String predict(int temperature);
}

class SunBot implements WeatherBot {
    public String predict(int temperature) {
        return (temperature > 30) ? "HOT" : "MODERATE";
    }
}


class RainBot implements WeatherBot {
    public String predict(int temperature) {
        return (temperature < 20) ? "COLD" : "WARM";
    }
}

public class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        int temperature = sc.nextInt();
        int botType = sc.nextInt();
        sc.close();

        WeatherBot bot;

        if (botType == 1) {
            bot = new SunBot();
        } else {
            bot = new RainBot();
        }

        System.out.println(bot.predict(temperature));
    }
}
```



## OUTPUT:

<img width="465" height="187" alt="image" src="https://github.com/user-attachments/assets/437fcdee-7f7a-4a5f-8ba8-eb382ed07fed" />


## RESULT:

Thus, the Java program was successfully implemented using an interface.


