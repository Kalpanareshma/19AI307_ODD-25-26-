# Ex.No:3(b) POLYMORPHISM

## QUESTION:
Write a Java program that calculates the area of different shapes using method overloading.
Create a class AreaCalculator with the following methods:

    - area(int side) → area of a square

    - area(int length, int breadth) → area of a rectangle

    - area(double radius) → area of a circle


## AIM:
To implement method overloading in Java by defining multiple area() methods with different parameter lists to compute areas of square, rectangle, and circle.

## ALGORITHM :
1. Start the program.

2. Create a class AreaCalculator.

3. Overload the method area() as:

     - area(int side) returns area of a square.

     - area(int length, int breadth) returns area of a rectangle.

     - area(double radius) returns area of a circle.

4. In the main method:

     - Read side, length, breadth, and radius from the user.

     - Call each overloaded method.

     - Display the results.

5. Stop the program.




## PROGRAM:
 ```
/*
Program to implement a Polymorphism using Java
Developed by: KALPANA S
Register Number:212222040069
*/
```

## SOURCE CODE:
```
import java.util.Scanner;

public class AreaCalculator {

    void area(int side) {
        System.out.println("Area of square: " + (side * side));
    }

    void area(int length, int breadth) {
        System.out.println("Area of rectangle: " + (length * breadth));
    }

    void area(double radius) {
        System.out.println("Area of circle: " + (Math.PI * radius * radius));
    }

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        AreaCalculator a = new AreaCalculator();

        int side = sc.nextInt();
        a.area(side);

        int length = sc.nextInt();
        int breadth = sc.nextInt();
        a.area(length, breadth);

        double radius = sc.nextDouble();
        a.area(radius);
    }
}
```






## OUTPUT:
<img width="714" height="412" alt="Screenshot 2025-11-20 at 10 29 00 AM" src="https://github.com/user-attachments/assets/c34b8b58-3a03-4638-9381-1c39196e6ebb" />



## RESULT:
Thus, the Java program using method overloading to calculate areas of square, rectangle, and circle was executed successfully.
