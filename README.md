# 🏨 Stay Reservation System

## 📌 Overview

The **Stay Reservation System** is a simple Java-based console application that allows users to manage hotel room reservations. It provides functionalities for reserving a room, viewing reservations, retrieving room numbersng reservations, and deleting reservations.

## ✨ Features

- ✅ **Reserve a Room:** Allows users to book a hotel room by providing guest details.
- 📜 **View Reservations:** Displays all existing reservations in a tabular format.
- 🔍 **Get Room Number:** Retrieves the room number for a given reservation ID and guest name.
- ✏️ **Update Reservations:** Updates guest details for an existing reservation.
- ❌ **Delete Reservations:** Removes a reservation from the system.
- 🚪 **Exit System:** Gracefully exits the application with a delay for better user experience.

## 🛠️ Technologies Used

- ☕ **Java** (Core Java concepts like JDBC, Exception Handling, Loops, and Conditionals)
- 🗄️ **MySQL** (Database to store reservations)
- 🔗 **JDBC** (Java Database Connectivity to interact with MySQL)

## 🗂️ Database Schema

The application interacts with the following table:

```sql
CREATE TABLE reservations (
    reservation_id INT AUTO_INCREMENT PRIMARY KEY,
    guest_name VARCHAR(100) NOT NULL,
    room_number INT NOT NULL,
    contact_number VARCHAR(15) NOT NULL,
    reservation_date TIMESTAMP DEFAULT CURRENT_TIMESTAMP
);
```

## ⚙️ Prerequisites

Before running the project, ensure you have:

- ✅ **Java Development Kit (JDK 8 or later)** installed.
- ✅ **MySQL Database** running with the required table.
- ✅ **JDBC Driver** (MySQL Connector) configured in your project.

## 🚀 Setup Instructions

1. **Clone the Repository:**
   ```sh
   git clone https://github.com/prathu77/Stay-Reservation-System.git
   ```
2. **Navigate to the Project Directory:**
   ```sh
   cd Stay-Reservation-System
   ```
3. **Compile the Java Program:**
   ```sh
   javac -cp .;mysql-connector-java-8.0.26.jar com/p1/HotelReservationSystem.java
   ```
4. **Run the Application:**
   ```sh
   java -cp .;mysql-connector-java-8.0.26.jar com.p1.HotelReservationSystem
   ```

## 📖 How to Use

1. Run the application.
2. Choose an option from the menu:
   - `1️⃣` to **Reserve a Room**.
   - `2️⃣` to **View Reservations**.
   - `3️⃣` to **Get Room Number**.
   - `4️⃣` to **Update a Reservation**.
   - `5️⃣` to **Delete a Reservation**.
   - `0️⃣` to **Exit**.
3. Follow the on-screen prompts to enter required details.

## 🔮 Future Enhancements

- 🖥️ Add **Graphical User Interface (GUI)** for better user experience.
- 🔍 Implement **Advanced Search & Filtering** for reservations.
- 🔒 Enhance **Security Features** using Prepared Statements to prevent SQL Injection.

## 👨‍💻 Author

- **Prathamesh Shelke**

