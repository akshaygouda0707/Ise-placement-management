# Database Connection Utility for Campus Placement Management System

## Overview
The `DBConnection` class provides a utility for establishing a database connection to the Campus Placement Management System. It uses JDBC (Java Database Connectivity) to connect to a MySQL database hosted locally.

## Usage
To use the `DBConnection` class in your project, follow these steps:
1. Ensure that you have the MySQL JDBC driver installed in your project dependencies.
2. Import the `campus_placement_mgt.DBConnection` class into your project.
3. Call the `getConnection()` method to establish a connection to the database.

Example:
```java
import java.sql.Connection;
import campus_placement_mgt.DBConnection;

public class YourClass {
    public static void main(String[] args) {
        Connection con = DBConnection.getConnection();
        // Use the 'con' object to perform database operations
    }
}
