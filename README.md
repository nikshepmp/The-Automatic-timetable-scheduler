
# AUTOMATIC TIMETABLE SCHEDULER

The Automatic Timetable Scheduler is a PHP-based application designed to automate the creation of class timetables for educational institutions such as schools, colleges, or universities. This system allows administrators to easily input course, faculty, and room data, and it then generates optimized and conflict-free timetables for students and teachers. The main aim of this system is to streamline the timetable creation process, saving time and reducing manual errors.


## Prerequisites

1. **XAMPP/WAMP/MAMP**: Install a local server like [XAMPP](https://www.apachefriends.org/index.html), [WAMP](http://www.wampserver.com/en/), or [MAMP](https://www.mamp.info/en/) that includes Apache, PHP, and MySQL.
2. **Git**: Make sure Git is installed on your system if you plan to clone the repository from GitHub.
3. **MySQL Database**: Ensure you have a MySQL database set up for the project.

## Steps to Install the PHP App

### Step 1: Clone the Repository

1. Go to the GitHub repository.
2. Clone the repository to your local system using Git (open the terminal or Git Bash):
    ```bash
    git clone https://github.com/Abhish7781/The-Automatic-timetable-scheduler.git
    ```
   Or alternatively, you can download the project as a ZIP file from the GitHub repository and extract it on your local machine.

### Step 2: Set Up the Server (XAMPP/WAMP/MAMP)

1. Install [XAMPP](https://www.apachefriends.org/index.html) / [WAMP](http://www.wampserver.com/en/) / [MAMP](https://www.mamp.info/en/) and start the Apache server and MySQL.

2. Navigate to the `htdocs` folder (for XAMPP) or the web root directory of your local server (for WAMP/MAMP).
   
   Example for XAMPP:
   ```text
   C:\xampp\htdocs

Move the Project Files, Copy the project files (from the cloned repository or the extracted ZIP) into this folder.

### Step-3: Create the Database
Open phpMyAdmin in your browser.

Create a new database for your application.

Example:
```bash
Database name: timetable_db
```
Import Database Schema:

If the repository has an .sql file for the database, import it into the newly created database.
Go to Import in phpMyAdmin, select the .sql file, and import it.

UPDATE DATASAE CONNECTION
```php
<?php
$servername = "localhost";   // or your server's IP
$username = "root";          // default username for MySQL
$password = "";              // default password for MySQL
$dbname = "timetable_db";    // the name of the database you created

// Create connection
$conn = new mysqli($servername, $username, $password, $dbname);

// Check connection
if ($conn->connect_error) {
    die("Connection failed: " . $conn->connect_error);
}
?>
```


## Deployment

To deploy this project run

```bash
  cd path/to/your/php/file
```
Execute the PHP file with the following command:
```bash
php index.php
```
Start PHP's built-in server:
```bash
php -S localhost:8000
```
Open a browser and visit:
```bash
http://localhost:8000/index.php
```
## DEFAULT User ID and Password
UserID
```bash
admin
```
Password
```bash
pass123
```
## Features

1. **Automatic Scheduling**  
   - Automatically generates schedules based on course requirements, teacher availability, and room allocation, reducing manual work and ensuring optimal usage of resources without overlapping.

2. **Faculty Specific & Admin Timetable**  
   - Provide Teacher specific timetable, making efficient use of the resource, in addtion it also provides main timetable from the admin.

3. **Customizable Timetable Configuration**  
   - Allows customization of class durations, break times, and class frequency (e.g., daily, weekly) to fit institutional needs.

4. **Exportable**  
   - Provides export options for timetables in HTML, PDF, and CSV formats, making it easy to distribute the timetable digitally or in printed form.

## Screenshots
HOME PAGE
![App Screenshot](https://i.pinimg.com/1200x/cf/59/1b/cf591b3cfaaea3956775d50d9037bc02.jpg)

USER LOGIN 
![App Screenshot](https://i.pinimg.com/1200x/40/57/b9/4057b9cb3c8fd0503b51db0fbc1424d9.jpg)

FACULTY ADDED

![App Screenshot](https://i.pinimg.com/1200x/cc/a2/b4/cca2b4ac349e0d5f52d0c4798742640d.jpg)

SAMPLE TIMETABLE

![App Screenshot](https://i.pinimg.com/1200x/1f/26/93/1f26936b5055d59dfddf8b5477c10ca4.jpg)


## Authors

- [Abhishek A B](mailto:abhishekab7781@gmail.com)

- [C Thushar](mailto:thusharc3.work@gmail.com)

- [Nikshep MP](mailto:nikshepmp.work@gmail.com)

- [Pratiksha D](mailto:prathikshad1005@gmail.com)

