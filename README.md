# Introduction To Java

Hello programmers!! Welcome to this "Introduction to Java" workshop. This workshop is designed to provide you with hands-on experience and practical knowledge of Java programming concepts. The workshop is suitable for beginners who are new to java or those who have limited experience with the language. But If you already know java, don't worry! It is also useful to review the basics of the language.

## What is Java?

![image](https://github.com/MarioHM2004/java-Workshop/assets/114911961/b9ce410a-9b0e-4999-aefb-c36f2d43a5a1)

Java is a widely-used, high-level programming language known for its portability, versatility, and robustness. It is commonly used for developing various types of applications, including web applications, mobile apps (Android), desktop GUI applications, enterprise software, and more. Java is an object-oriented programming language, meaning it focuses on creating objects that contain both data and methods to manipulate that data.

##  prerequisites - Install Java

Installing Java is very easy! You just need to install the Java Development Kit (JDK) on your computer. You can download the latest version from the official Oracle website:

[https://www.java.com/en/download/help/linux_install.html](https://www.oracle.com/java/technologies/downloads/#jdk22-linux)

## exercise 1 - Print your first message

Create a new file called Print.java

In order to output a message you will need to create a ***Print*** class and a ***main*** method as follows. 

```java
public class Print {
    public static void main(String[] args) {
        System.out.println("Java is working!!");
    }
}
```

## exercise 2 - methods and attributes

Congratulations!! You know how to simply output a message. Now you will have to implement a class called ***Rectangle*** with attributes ***length*** and ***width***. Write methods to calculate the area and perimeter of the rectangle and create instances of the Rectangle class in order to test this methods.

We will do it together step by step:

### step 1 - Create the Rectangle Class

Create a ***Rectangle.java*** file

First, we will create a class named Rectangle. This class will have two private attributes: length and width.

```java
public class Rectangle {
    private double length;
    private double width;
}

```

### step 2 - Constructor

Next, we'll create a constructor for the Rectangle class. The constructor will initialize the length and width attributes.

```java
public Rectangle(double length, double width) {
    this.length = length;
    this.width = width;
}
```

### step 3 - Area and Perimeter calculation methods

Now is your turn! Try to easily implement the provided methods on the code below

```java
public double calculateArea() {
    // your code goes here
}

public double calculatePerimeter() {
    // your code goes here
}
```

### step 4 - time to test!!

Finally, you need to create a main method, as you did in exercise1, to test our Rectangle class. Create an instance of the Rectangle class, calculate its area and perimeter, and print the results.

You should output like this:

```
Area of the rectangle: 50.0
Perimeter of the rectangle: 30.0
```

## exercise 3 - Exception Handling

Now you will learn how to handle exceptions. For this exercise you will need to do two different programs. 

- First write a program that takes user input for two numbers and divides them. Handle the potential "ArithmeticException"·
- Then write a program that prompts the user to enter an integer. Handle the potential "InputMismatchException".

### step 1 - Import Necessary Packages

Create a new file called ***ExceptionHandling.java***

First, we need to import the required packages for handling exceptions and for user input.

```java
import java.util.InputMismatchException;
import java.util.Scanner;
```

### step 2 - Write the Main Method

Create the main method where we'll handle the user input and exceptions. We will use ***scanner*** class to read input from various sources like keyboard, files, etc. In the context of our exercise, we use Scanner to read input from the user via the keyboard. 

```java
public class ExceptionHandling {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        // Code for handling exceptions will go here

        scanner.close();
    }
}
```

### step 3 -  Handle InputMismatchException

Inside the main method, we will handle the InputMismatchException that may occur when the user enters a non-integer value. In order to achieve this we will use escanner.nextInt(), this method reads an integer input entered by the user. Scanner simplifies the process of reading user input and parsing it into appropriate data types.

```java
try {
    System.out.print("Enter an integer: ");
    int number = scanner.nextInt();
    System.out.println("You entered: " + number);
} catch (InputMismatchException e) {
    System.out.println("Error: Input is not an integer");
}
```

### step 4 - Handle ArithmeticException

Now we will handle the ArithmeticException that may occur during division by zero. Try to do it by yourself! 

With previous steps all together it should output something like this:

```
Enter an integer: 28.5
Error: Input is not an integer
Enter dividend: 32
Enter divisor: 2
Result of division: 16
```

## Exercise 4 - File I/O

In this exercise you will have to code two programs as before. You need to create a input.txt and put whatever you want inside.

- Write a program that reads from a text file and prints its content to the console.
- Write a program that writes user input to a ***output.txt*** file. If the data was written successfully to the file, It should print a message in the terminal.

This exercise you will do it completely by your own!! You will also need to manage error with exception as before. Here is a tip! Search about ***File*** and ***PrintWriter*** classes.

## exercise 5 - Vehicle Inheritance

For this last exercise, You have to create a program that models different types of vehicles. We'll have a base class ***Vehicle*** and two subclasses ***Car*** and ***Bike***. Each class will have a method displayInfo() to print information about the vehicle.

Create a ***Main.java*** file.

### Vehicle class

This class will have the following attributes that must be initialized within the constructor, you should search about what a constructor is.

- make (String)
- model (String)
- year (int)
- fuelType (String)

Implement a method displayInfo() in the Vehicle class to display the information about the vehicle.

Use the ***final*** keyword to prevent overriding the displayInfo() method in the Vehicle class.

### Car class

The Car class will be a subclass of Vehicle and will additionally have an attribute numDoors (int) and its own displayCarInfo() that should display displayInfo() method and numDoors.

### Bike class

The Bike class will also be a subclass of Vehicle and will additionally have an attribute engineType (String) and also its own displayBikeInfo() that should display displayInfo() method and engineType.


As a tip, I recommend you to search about ***super*** and ***extends*** keywords.

Your code should output like this:

```
Car Information:
Make: Toyota
Model: Camry
Year: 2022
Fuel Type: Gasoline
Number of Doors: 4

Bike Information:
Make: Honda
Model: CBR1000RR
Year: 2021
Fuel Type: Gasoline
Engine Type: Inline Four
```

## Ending

If you have reached this point it means that you have done everything satisfactorily. Thank you for attending my workshop! I hope it has been useful to you.
