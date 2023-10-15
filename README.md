# JavaSE-Passing primitives or objects

In Java, when you pass parameters to methods, you can pass both primitive data types and objects. Let me provide you with examples for both cases.

## 1. Passing Primitives:

```java
public class PrimitiveExample {

    // Method that takes two integers as parameters and prints their sum
    public static void add(int a, int b) {
        int sum = a + b;
        System.out.println("Sum: " + sum);
    }

    public static void main(String[] args) {
        int num1 = 5;
        int num2 = 10;

        // Calling the add method and passing primitive integers
        add(num1, num2);
    }
}
```

In this example, add method takes two int parameters (a and b), and the main method calls add by passing two primitive integers (num1 and num2).

## 2. Passing Objects:

```java
public class ObjectExample {

    // Simple class representing a Point with x and y coordinates
    public static class Point {
        int x;
        int y;

        public Point(int x, int y) {
            this.x = x;
            this.y = y;
        }
    }

    // Method that takes a Point object as a parameter and prints its coordinates
    public static void printPoint(Point point) {
        System.out.println("Coordinates: (" + point.x + ", " + point.y + ")");
    }

    public static void main(String[] args) {
        // Creating a Point object
        Point myPoint = new Point(3, 7);

        // Calling the printPoint method and passing the Point object
        printPoint(myPoint);
    }
}
```

In this example, printPoint method takes a Point object as a parameter, and the main method creates a Point object (myPoint) and passes it to the printPoint method.

I hope these examples help clarify how to pass parameters in Java, both for primitives and objects
