# College Online Voting System(Covs)

## Project Description

The **College Online Voting System** is a web-based platform designed to facilitate secure and efficient voting for college elections. The system allows students to register and cast votes online, while administrators and staff manage the election process. The project was developed specifically for a college election using **PHP**, **MySQLi**, **MySQL Database**, **HTML**, **CSS**, **JavaScript (jQuery and Ajax)**, and **Bootstrap** for the design.

### Features

#### Admin Side:
- Login/Logout
- Manage Candidates
- Activate/Deactivate Voters
- Manage Students
- Generate Election Reports
- Manage User/Staff List
- View User Time Logs

#### Staff Side:
- Login/Logout
- Manage Candidates
- View Voters List
- Manage Students
- Generate Election Reports
- View User/Staff List

#### Voters:
- Register with Student ID
- Vote for Candidates

### Technology Stack:
- **Backend:** PHP, MySQLi
- **Frontend:** HTML, CSS, Bootstrap, JavaScript (jQuery, Ajax)
- **Database:** MySQL

## Installation and Setup Instructions

1. **Clone the Repository:**
   ```bash
   git clone https://github.com/your-username/college-online-voting-system.git
   cd college-online-voting-system
   ```

2. **Database Setup:**
   - Create a MySQL database in your local server (e.g., `vote`).
   - Import the provided SQL file (`vote.sql`) into the created database.

3. **Configuration:**
   - In the project folder, locate the `config.php` file and update the database credentials:
     ```php
     <?php
     $conn = new mysqli('localhost', 'root', '', 'vote');
     ?>
     ```

4. **Run the Project:**
   - Open a browser and access the project via `http://localhost/college-online-voting-system/`.

5. **Login Credentials:**
   - Default Admin:
     - Login Id: 1
     - Username: `admin`
     - Password: `admin`
   - Default User:
     - Login Id: 4
     - Username: `user`
     - Password: `user`

## Project Structure

- `/admin` - Admin-related pages
- `/staff` - Staff-related pages
- `/voters` - Voter registration and voting
- `/assets` - CSS, JS, images, and Bootstrap files
- `/config.php` - Database connection

## Usage

- **Admin** can manage the election process by adding candidates, activating or deactivating voters, and generating reports.
- **Staff** has limited management access, including viewing voter lists and generating reports.
- **Voters** must register with their student ID and, once approved by the admin, can vote for their chosen candidates.

