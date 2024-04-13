
# Main Screen for Campus Placement Management System

## Overview
The `MainScreen` class provides the main user interface for the Campus Placement Management System. It contains a menu bar with options to navigate through various functionalities of the system, such as managing students, companies, and placement details.

## Usage
To use the `MainScreen` class in your project, follow these steps:
1. Import the `campus_placement_mgt.MainScreen` class into your project.
2. Instantiate an object of the `MainScreen` class and call its `setVisible(true)` method to display the main screen.

Example:
```java
public class YourClass {
    public static void main(String[] args) {
        java.awt.EventQueue.invokeLater(new Runnable() {
            public void run() {
                new MainScreen().setVisible(true);
            }
        });
    }
}
```

## Dependencies
- Icons: Ensure that the icons used in the `MainScreen` class are available in the appropriate directory. You may need to adjust the paths if the icons are located elsewhere.

## Features
- Menu options for adding students, companies, and placement details.
- Menu options for viewing lists of students, companies, and placement results.
- Clicking on menu items opens corresponding GUI forms for data entry or viewing.

## Contributors
- vidyashree c n

## License
This component is provided under the [MIT License](LICENSE).
```
