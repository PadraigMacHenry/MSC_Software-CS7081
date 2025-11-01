This solution uses only variables, operators, and if statements to analyze weather data, as taught in Week 1.

Advanced solution using Arrays, see: [[Challenge 1 - Weather Analysis (Advanced Solution)]]

---

## Solution

```java
public class WeatherAnalyzerPrimitive {
    public static void main(String[] args) {
        // Weather data for each day
        String day1Condition = "Sun";
        double day1Temp = 15.5;

        String day2Condition = "clouds and rain";
        double day2Temp = 10.5;

        String day3Condition = "Sun and large cloud";
        double day3Temp = 16.0;

        String day4Condition = "Sun small cloud";
        double day4Temp = 12.5;

        String day5Condition = "clouds and rain";
        double day5Temp = 17.0;

        // Calculate average temperature
        double totalTemp = day1Temp + day2Temp + day3Temp + day4Temp + day5Temp;
        double averageTemp = totalTemp / 5;

        // Count sunny days
        int sunnyDays = 0;

        // Print header
        System.out.println("Weather analysis");
        System.out.println("____________________________________");

        // Day 1
        boolean day1HasSun = day1Condition.contains("Sun");
        if (day1HasSun) sunnyDays++;
        System.out.println("Day 1");
        System.out.printf("Temp     : %.1f%n", day1Temp);
        System.out.println("Sun      : " + day1HasSun);
        if (day1Temp > averageTemp) {
            System.out.println("Above average Temp");
        }
        System.out.println("____________________________________");

        // Day 2
        boolean day2HasSun = day2Condition.contains("Sun");
        if (day2HasSun) sunnyDays++;
        System.out.println("Day 2");
        System.out.printf("Temp     : %.1f%n", day2Temp);
        System.out.println("Sun      : " + day2HasSun);
        if (day2Temp > averageTemp) {
            System.out.println("Above average Temp");
        }
        System.out.println("____________________________________");

        // Day 3
        boolean day3HasSun = day3Condition.contains("Sun");
        if (day3HasSun) sunnyDays++;
        System.out.println("Day 3");
        System.out.printf("Temp     : %.1f%n", day3Temp);
        System.out.println("Sun      : " + day3HasSun);
        if (day3Temp > averageTemp) {
            System.out.println("Above average Temp");
        }
        System.out.println("____________________________________");

        // Day 4
        boolean day4HasSun = day4Condition.contains("Sun");
        if (day4HasSun) sunnyDays++;
        System.out.println("Day 4");
        System.out.printf("Temp     : %.1f%n", day4Temp);
        System.out.println("Sun      : " + day4HasSun);
        if (day4Temp > averageTemp) {
            System.out.println("Above average Temp");
        }
        System.out.println("____________________________________");

        // Day 5
        boolean day5HasSun = day5Condition.contains("Sun");
        if (day5HasSun) sunnyDays++;
        System.out.println("Day 5");
        System.out.printf("Temp     : %.1f%n", day5Temp);
        System.out.println("Sun      : " + day5HasSun);
        if (day5Temp > averageTemp) {
            System.out.println("Above average Temp");
        }
        System.out.println("____________________________________");

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
#Java #Challenge #WeatherData #Conditionals #Variables #Operators #IfStatements #Week1 #PrimitiveSolution
### [[Home Page]] | [[Week 1 Topic Summary]] | [[Week 2 Topic Summary]]

### Challenge: Weather Analysis: 
- [[Challenge 1 - Weather Analysis (Primitive Solution)]]
- [[Challenge 1 - Weather Analysis (Advanced Solution)]]
### Lab Exercises:
- [[Lab Exercise 1 - Output to Console]]
- [[Lab Exercise 2 - String Manipulation]]
- [[Lab Exercise 3 - Declaring and Using Variables]]