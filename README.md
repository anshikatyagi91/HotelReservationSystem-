# HotelReservationSystem
Hotel Reservation System
Definition - The Hotel Reservation System is a Java-based console application designed to manage hotel room bookings efficiently. It enables users (such as hotel staff or admins) to add, view, update, and delete guest reservation details. This system uses MySQL as its backend database and connects to it via JDBC (Java Database Connectivity) to perform real-time CRUD (Create, Read, Update, Delete) operations. The aim is to streamline the reservation process, maintain proper records, and make room management seamless.

Project Requirements & Functionalities -
  System Requirements:-
    JDK (Java Development Kit) installed
    MySQL Database server
    MySQL JDBC Driver (Connector/J)
    IDE or text editor (Eclipse, IntelliJ IDEA, etc.)
    Command-line interface / Terminal


Functional Requirements (Features)-
  1.Reserve a Room:-
         Takes guest name, room number, and contact number as input. 
         Inserts the reservation into the MySQL database.

  2.View Reservations:-
         Displays all reservations in a neatly formatted table, including ID, guest name, room number, contact, and date.

  3.Get Room Number:-
         Based on reservation ID and guest name, retrieves the allocated room number.
  
  4.Update Reservation:-
         Allows updating of guest name, room number, and contact number for an existing reservation.

  5.Delete Reservation:-
         Deletes a reservation from the system using the reservation ID.

  6.Exit System:-
         Gracefully exits the application with a thank-you message.


Technologies & Concepts Used -
Technology/Concept  ----  Purpose/Usage
1.Java  ----  Core programming language for backend logic
2.JDBC (Java Database Connectivity)  ----  Connects Java app to MySQL database
3.MySQL ----  Relational database for storing reservation data
4.SQL  ----  Used to perform queries: INSERT, SELECT, UPDATE, DELETE
5.OOP (Object-Oriented Programming)  ----  Structuring logic into reusable methods
6.Error Handling  ----  Try-catch blocks for SQL and ClassNotFound exceptions
7.Scanner Class  ----  Takes input from users via console


Project Structure & Explanation -

Database Table:- reservations
CREATE TABLE reservations (
reservation_id INT AUTO_INCREMENT PRIMARY KEY,
guest_name VARCHAR(100),
room_number INT,
contact_number VARCHAR(20),
reservation_date TIMESTAMP DEFAULT CURRENT_TIMESTAMP
);

Java Code Components -
        main() – Loads JDBC driver, connects to DB, shows menu, handles options.
        reserveRoom() – Inserts a new reservation.
        viewReservations() – Retrieves and displays all records.
        getRoomNumber() – Fetches room number based on guest details.
        updateReservation() – Modifies existing reservation data.
        deleteReservation() – Removes reservation from the table.
        reservationExists() – Utility method to verify record before update/delete.

Summary - The Hotel Reservation System is a beginner-friendly but fully functional console-based application that demonstrates how Java can be used to interact with a relational database like MySQL. It shows how real-world business processes like hotel management can be digitally transformed using simple technologies.



