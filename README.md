
## Author

- [@Akshay G Gouda](https://github.com/akshaygouda0707)
---

# Campus Placement Management System

Welcome to the Campus Placement Management System README! This system is designed to streamline the campus placement process, allowing students and companies to interact efficiently.

## Overview

This system consists of a database schema with tables for managing student and company information, placement records, and user authentication.

### Database Schema Overview:

#### Tables:
1. **`company`**: Stores information about recruiting companies participating in campus placements.
   - Columns: `cname` (Company Name), `seatoffer` (Number of Seats Offered), `CGPA` (Minimum CGPA Requirement).

2. **`login`**: Contains login credentials for system access.
   - Columns: `id` (User ID), `username` (Username), `password` (Password).

3. **`placement`**: Records placement details of students.
   - Columns: `student_usn` (Student USN), `fname` (First Name), `lname` (Last Name), `cgpa` (CGPA), `phone` (Phone Number), `email` (Email), `cname` (Company Name), `package` (Offered Package), `year` (Year of Placement).

4. **`student`**: Stores student information.
   - Columns: `student_usn` (Student USN), `fname` (First Name), `lname` (Last Name), `branch` (Branch of Study), `cgpa` (CGPA), `email` (Email), `phone` (Phone Number), `dob` (Date of Birth).

### System Functionality:

1. **Student Module**:
   - Students can register in the system by providing their personal information (`student` table).
   - They can view their own placement details and update personal information if needed.

2. **Company Module**:
   - Companies can register in the system by providing details such as name, seat offers, and minimum CGPA requirement (`company` table).
   - They can view and manage placement records of students who have been placed in their company (`placement` table).

3. **Placement Module**:
   - Facilitates recording and managing placement details of students (`placement` table).
   - Allows administrators to track placement statistics, such as the number of students placed in each company and the overall placement rate.

4. **Authentication Module**:
   - Manages user authentication using the `login` table.
   - Only authorized users with valid login credentials can access the system.

## System Workflow:

1. **Student Registration**:
   - Students register by providing personal information (`student` table).
   - Upon successful registration, they receive login credentials stored in the `login` table.

2. **Company Registration**:
   - Companies register by providing company details (`company` table).
   - Upon registration, they can access placement records of students (`placement` table) relevant to their recruitment process.

3. **Placement Process**:
   - Placement coordinators record placement details of students (`placement` table) after the recruitment process.
   - Details include student information, company details, offered package, and year of placement.

4. **Authentication and Access Control**:
   - Only authorized users with valid login credentials (stored in the `login` table) can access the system.
   - Different access levels may be implemented, allowing administrators, students, and companies to access relevant modules.

## Sample Queries:

1. Retrieve all placement records:
   ```sql
   SELECT * FROM placement;
   ```

2. Retrieve student information along with their placement details:
   ```sql
   SELECT s.*, p.cname, p.package, p.year 
   FROM student s
   JOIN placement p ON s.student_usn = p.student_usn;
   ```

3. Update student information:
   ```sql
   UPDATE student
   SET cgpa = '9.0'
   WHERE student_usn = '4mc19is004';
   ```

4. Authenticate user login:
   ```sql
   SELECT * FROM login
   WHERE username = 'test' AND password = 'test';
   ```

## Conclusion

The Campus Placement Management System simplifies the campus placement process, providing a platform for students and companies to interact effectively. It ensures data integrity, access control, and efficient management of placement activities.

---

