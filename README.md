# Hospital Management System

## Installation

1. Ensure you have Java Development Kit (JDK) installed on your system.
2. Clone the repository or download the source code files.
3. Open the project in your preferred Java IDE (e.g., IntelliJ IDEA, Eclipse, or NetBeans).
4. Build the project and resolve any dependencies.
5. Ensure you have a MySQL database server running on your local machine or a remote server.
6. Update the database connection details in the `conn.java` file to match your environment.

## Usage

1. Run the `Login.java` file to launch the Hospital Management System application.
2. Enter the username and password to log in.
   - The default username is `adisri` and the password is `234567`.
3. The main `Reception` screen will be displayed, providing access to various functionalities:
   - Add New Patient
   - Room Management
   - Department Management
   - Employee Information
   - Patient Information
   - Patient Discharge
   - Update Patient Details
   - Hospital Ambulance
   - Room Search
   - Logout

## API

The Hospital Management System utilizes the following Java classes and their methods:

1. `conn.java`:
   - `Connection connection`: Establishes a connection to the MySQL database.
   - `Statement statement`: Executes SQL queries.

2. `DbUtils.java`:
   - This class is currently empty and can be used to define utility methods or enums related to the database.

3. `jButton.java`:
   - `jButton(String login)`: Constructs a new JButton with the specified label.

4. `Login.java`:
   - `actionPerformed(ActionEvent e)`: Handles the login process and opens the `Reception` screen upon successful authentication.

5. `New_Patient.java`:
   - `actionPerformed(ActionEvent e)`: Handles the creation of a new patient record and updates the room availability in the database.

6. `Reception.java`:
   - This class sets up the main user interface for the Hospital Management System, providing access to various functionalities through buttons.

7. `Room.java`:
   - Displays a table of available rooms, their availability, price, and bed type.
   - Provides a "Back" button to navigate back to the previous screen.

## Contributing

Contributions to the Hospital Management System project are welcome. If you find any issues or have suggestions for improvements, please create a new issue or submit a pull request on the project's GitHub repository.

## License

This project is licensed under the [MIT License](LICENSE).

## Testing

To test the Hospital Management System, follow these steps:

1. Run the `Login.java` file and verify that the login functionality works correctly with the default credentials.
2. Test the various functionalities accessible from the `Reception` screen, such as adding a new patient, managing rooms, and accessing patient/employee information.
3. Ensure that the data is properly stored and retrieved from the MySQL database.
4. Verify that the room availability is updated correctly when a new patient is added.
5. Test the "Back" button functionality in the `Room` screen.

Please note that additional unit tests and integration tests can be added to the project to ensure comprehensive testing coverage.


![Image](https://github.com/user-attachments/assets/cecdbb91-b1fc-4160-a234-0172bdfe6bdd)

![Image](https://github.com/user-attachments/assets/e8a95fd2-3527-4f1f-9376-ff25ffcfc45a)

![Image](https://github.com/user-attachments/assets/0e665828-4fc7-4ff6-b0a0-ce5f627830aa)

