This challenge requires you to use variables, operators, and if statements to store, analyze, and output weather-related data.

## Challenge Description

You have been asked to write a Java program to analyze the following weather stats:

| Day   | Conditions         | Temperature |
|-------|--------------------|-------------|
| Day 1 | Sun                | 15.5        |
| Day 2 | clouds and rain    | 10.5        |
| Day 3 | Sun and large cloud| 16.0        |
| Day 4 | Sun small cloud    | 12.5        |
| Day 5 | clouds and rain    | 17.0        |

Your program should output the following format:

```
Weather analysis
____________________________________
Day 1
Temp     : 15.5
Sun      : true
Above average Temp
____________________________________
Day 2
Temp     : 10.5
Sun      : false
____________________________________
Day 3
Temp     : 16.0
Sun      : true
Above average Temp
____________________________________
Day 4
Temp     : 12.5
Sun      : true
____________________________________
Day 5
Temp     : 17.0
Sun      : false
Above average Temp
____________________________________
Overall stats
Average temp              : 14.3
Number of days of sun     : 3
```

---

## Solution

```java
public class WeatherAnalyzer {
    public static void main(String[] args) {
        // Weather data
        String[] conditions = {
            "Sun",
            "clouds and rain",
            "Sun and large cloud",
            "Sun small cloud",
            "clouds and rain"
        };

        double[] temperatures = {15.5, 10.5, 16.0, 12.5, 17.0};

        // Calculate average temperature
        double sum = 0;
        for (double temp : temperatures) {
            sum += temp;
        }
        double averageTemp = sum / temperatures.length;

        // Count sunny days
        int sunnyDays = 0;

        // Print header
        System.out.println("Weather analysis");
        System.out.println("____________________________________");

        // Process each day
        for (int i = 0; i < 5; i++) {
            // Check if day had sun
            boolean hasSun = conditions[i].contains("Sun");
            if (hasSun) sunnyDays++;

            // Print day info
            System.out.println("Day " + (i + 1));
            System.out.printf("Temp     : %.1f%n", temperatures[i]);
            System.out.println("Sun      : " + hasSun);

            // Check if above average
            if (temperatures[i] > averageTemp) {
                System.out.println("Above average Temp");
            }

            System.out.println("____________________________________");
        }

        // Print overall stats
        System.out.println("Overall stats");
        System.out.printf("Average temp              : %.1f%n", averageTemp);
        System.out.println("Number of days of sun     : " + sunnyDays);
    }
}
```

---

## Expected Output

```
Weather analysis
____________________________________
Day 1
Temp     : 15.5
Sun      : true
Above average Temp
____________________________________
Day 2
Temp     : 10.5
Sun      : false
____________________________________
Day 3
Temp     : 16.0
Sun      : true
Above average Temp
____________________________________
Day 4
Temp     : 12.5
Sun      : true
____________________________________
Day 5
Temp     : 17.0
Sun      : false
Above average Temp
____________________________________
Overall stats
Average temp              : 14.3
Number of days of sun     : 3
```

---
## Keywords
#Java #Challenge #WeatherData #Conditionals #Arrays #ProblemSolving #Variables #Operators #IfStatements

### [[Home Page]] | [[Week 1 Topic Summary]] | [[Week 2 Topic Summary]]

### Challenge: Weather Analysis: 
- [[Challenge 1 - Weather Analysis (Primitive Solution)]]
- [[Challenge 1 - Weather Analysis (Advanced Solution)]]
### Lab Exercises:
- [[Lab Exercise 1 - Output to Console]]
- [[Lab Exercise 2 - String Manipulation]]
- [[Lab Exercise 3 - Declaring and Using Variables]]
