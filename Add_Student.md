

# Campus Placement Management System

## Overview
Campus Placement Management System is a Java Swing application designed to manage student records for campus placements. It allows users to add, update, and search for student information, including their USN (University Serial Number), names, CGPA (Cumulative Grade Point Average), branch, contact details, and email.

## Installation
1. Clone this repository to your local machine using Git:
   ```bash
   git clone <repository_URL>
   ```
   Replace `<repository_URL>` with the actual URL of the repository. For example:
   ```bash
   git clone https://github.com/yourusername/yourrepository.git
   ```
2. Open the project in your preferred Java IDE.
3. Build and run the `AddStudent.java` file to launch the application.

## Usage
1. **Adding a Student:** Enter the student details in the respective input fields and click the "Save" button.
2. **Updating a Student:** Search for a student using their USN, update the necessary fields, and click the "Update" button.
3. **Searching for a Student:** Enter the student's USN and click the "Search" button to view their details.
4. **Clearing Fields:** Click the "Clear" button to clear all input fields for new data entry.
5. **Back Button (`jButton6`):** Clicking this button navigates back to the main screen of the application.

## Button Functionality:
1. **Save Button (`jButton1`):**
   ```java
   jButton1.addActionListener(new ActionListener() {
       public void actionPerformed(ActionEvent evt) {
           add();
       }
   });
   ```
   - Adds a new student record to the database with the information entered in the input fields.

2. **Clear Button (`jButton2`):**
   ```java
   jButton2.addActionListener(new ActionListener() {
       public void actionPerformed(ActionEvent evt) {
           jButton2ActionPerformed(evt);
       }
   });
   ```
   - Clears all the input fields, allowing the user to enter new data easily.

3. **Update Button (`jButton3`):**
   ```java
   jButton3.addActionListener(new ActionListener() {
       public void actionPerformed(ActionEvent evt) {
           update();
       }
   });
   ```
   - Updates the existing student record with the modified information entered in the input fields.

4. **Search Button (`jButton4`):**
   ```java
   jButton4.addActionListener(new ActionListener() {
       public void actionPerformed(ActionEvent evt) {
           jButton4ActionPerformed(evt);
       }
   });
   ```
   - Searches for a student record based on the entered USN and displays their details in the respective input fields.

5. **Back Button (`jButton6`):**
   ```java
   jButton6.addActionListener(new ActionListener() {
       public void actionPerformed(ActionEvent evt) {
           jButton6ActionPerformed(evt);
       }
   });
   ```
   - Navigates back to the main screen of the application.

## Technologies Used
- **Java Swing for GUI development:** Java Swing is a set of GUI (Graphical User Interface) components that enables developers to create rich and interactive user interfaces for Java applications. It provides a comprehensive library of components such as buttons, text fields, labels, and more, allowing developers to create visually appealing and functional desktop applications.

- **MySQL for database management:** MySQL is an open-source relational database management system that is commonly used for storing and managing structured data. It provides a robust and scalable platform for managing the application's database.

## Contributors
- Vidyashree C N

## License
This project is licensed under the [MIT License](LICENSE).

---

