# online-registration-portal
This project has a login page,Home Page, registration page and logout page 
I have created a complete login and registration system with Python, Flask and MySQL.

prerequisite:

1) Download and install MySQL Community Server and MySQL Workbench.
2) Python 3.7
3) Install Python Flask with the command: pip install flask
4) Install Flask-MySQLdb with the command: pip install flask-mysqldb

Creating Database:

1) Open MySQL Workbench
2) Fill out your MySQL details
3) Click Test Connection, if successful you can click OK
4) Open your connection
Execute the following SQL statements:
CREATE DATABASE IF NOT EXISTS `pythonlogin` DEFAULT CHARACTER SET utf8 COLLATE utf8_general_ci;
USE `pythonlogin`;

CREATE TABLE IF NOT EXISTS `accounts` (
	`id` int(11) NOT NULL AUTO_INCREMENT,
  	`username` varchar(50) NOT NULL,
  	`password` varchar(255) NOT NULL,
    `mobileno` varchar(50) NOT NULL,
  	`email` varchar(100) NOT NULL,
    `phoneno` varchar(100) NOT NULL,
    PRIMARY KEY (`id`)
) ENGINE=InnoDB AUTO_INCREMENT=2 DEFAULT CHARSET=utf8;

INSERT INTO `accounts` (`id`, `username`, `password`,`mobileno`, `email`,`phoneno`) VALUES (1, 'preeti', 'evaan', '0183587654','test@test.com','959242434');


File Structure:

\-- online-portal
  |-- main.py
  \-- static
    |-- style.css
  \-- templates
    |-- index.html
    |-- register.html
    |-- home.html
    |-- profile.html
    |-- layout.html
