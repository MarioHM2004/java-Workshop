# Introduction To Java

Hello programmers!! Welcome to this "Introduction to Java" workshop. This workshop is designed to provide you with hands-on experience and practical knowledge of Java programming concepts. The workshop is suitable for beginners who are new to programming or those who have limited experience with Java. But If you already know java, don't worry!  It is also useful to review the basics of the language.

# What is Java?

![image](https://github.com/MarioHM2004/java-Workshop/assets/114911961/b9ce410a-9b0e-4999-aefb-c36f2d43a5a1)

Java is a widely-used, high-level programming language known for its portability, versatility, and robustness. It is commonly used for developing various types of applications, including web applications, mobile apps (Android), desktop GUI applications, enterprise software, and more. Java is an object-oriented programming language, meaning it focuses on creating objects that contain both data and methods to manipulate that data.

##  prerequisites - Install Java

Installing Java is very easy! You just need to install the Java Development Kit (JDK) on your computer. You can download the latest version from the official Oracle website:

[https://www.java.com/en/download/help/linux_install.html](https://www.oracle.com/java/technologies/downloads/#jdk22-linux)

## exercise 1 - Print your first message

Create a new file called ex01.java

In order to output a message you will need to create a "Main" class and a "main" method as follows. 

```java
public class Main {
    public static void main(String[] args) {
        System.out.println("Java is working!!");
    }
}
```

## exercise 2 - methods and attributes

Congratulations!! You know how to simply output a message. Now you will have to implement a class called "Rectangle" with attributes "length" and "width". Write methods to calculate the area and perimeter of the rectangle and create instances of the Rectangle class in order to test this methods.

We will do it together step by step:

### step 1 - Create the Rectangle Class

Create a ex02.java file

First, we will create a Java class named Rectangle. This class will have two private attributes: length and width.

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
    // need to implement
}

public double calculatePerimeter() {
    // need to implement
}
```

## step 4 - time to test!!

Finally, you need to create a main method, as you did in exercise1, to test our Rectangle class. Create an instance of the Rectangle class, calculate its area and perimeter, and print the results.

You should output like this:

```
Area of the rectangle: 50.0
Perimeter of the rectangle: 30.0
```
