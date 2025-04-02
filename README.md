# Movie Ticket Booking System

## Overview
This project is a **Movie Ticket Booking System** developed in **C++** with **MySQL** as the backend database. It allows users to view available seats, reserve tickets, and manage bookings efficiently. The system ensures real-time updates and database synchronization.

## Features
- Connects to a MySQL database
- Displays available seats in a 5-row, 10-seat layout
- Allows users to reserve a seat
- Updates seat availability dynamically
- Prevents double booking of seats
- Handles invalid inputs and database errors

## Technologies Used
- **Programming Language:** C++
- **Database:** MySQL
- **Libraries:**
  - `<mysql.h>` for MySQL connectivity
  - `<windows.h>` for system operations
  - `<sstream>` for data conversion

## Installation and Setup
1. **Install MySQL Server**
   - Ensure MySQL is installed and running on your system.
2. **Set Up the Database**
   - Create a database named `mydb`.
   - Create a table named `Ticket` using the following SQL schema:
   
   ```sql
   CREATE TABLE Ticket (
       RowNumber INT,
       SeatNumber INT,
       Seat INT
   );
   ```
3. **Update Database Credentials**
   - Modify the `HOST`, `USER`, `PW`, and `DB` variables in the code to match your MySQL configuration.
4. **Compile and Run the Program**
   - Compile the program using a C++ compiler with MySQL support.
   - Run the executable.

## How to Use
1. Upon execution, the program connects to the MySQL database.
2. It initializes the seating arrangement if not already present in the database.
3. Users are presented with options to:
   - View available seats
   - Reserve a seat
   - Exit the program
4. When a seat is reserved, the database updates the seat status dynamically.
5. The program exits upon user request.

## Future Enhancements
- Implement user authentication for booking verification.
- Add a graphical user interface (GUI) for better usability.
- Enable ticket cancellation and refund functionality.

This README provides a detailed guide to setting up and using the project. Let me know if you need any modifications!

