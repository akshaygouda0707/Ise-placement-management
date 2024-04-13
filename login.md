# Login Form for Campus Placement Management System

## Overview
The `Login_Form` class provides a graphical user interface (GUI) for users to log in to the Campus Placement Management System. It allows users to enter their username and password and validates them against the database entries.

## Usage
To use the `Login_Form` class in your project, follow these steps:
1. Ensure that you have the necessary Swing components imported into your project.
2. Import the `campus_placement_mgt.Login_Form` class into your project.
3. Instantiate an object of the `Login_Form` class and call its `setVisible(true)` method to display the login form.

Example:
```java
public class YourClass {
    public static void main(String[] args) {
        java.awt.EventQueue.invokeLater(new Runnable() {
            public void run() {
                new Login_Form().setVisible(true);
            }
        });
    }
}
