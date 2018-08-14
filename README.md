# JSP-With-Jdbc

[![N|Solid](http://selftutorials.in/self_res/assets/courses/jsp_servlet_mysql.jpg)](http://selftutorials.in/)

This project uses Java JSP and Servlet technology to demostrate a website, which can do basic CRUD operations on MySql database.

 
### How to Setup this Project

JSP-with-Jdbc requires Java 8+ to run.

Run the following sql script to create the database user

```sh
CREATE USER 'webstudent'@'localhost' IDENTIFIED BY 'webstudent';
GRANT ALL PRIVILEGES ON * . * TO 'webstudent'@'localhost';
```

Create sample student table

```sh
CREATE DATABASE  IF NOT EXISTS `web_student_tracker` /*!40100 DEFAULT CHARACTER SET latin1 */;
USE `web_student_tracker`;
DROP TABLE IF EXISTS `student`;
CREATE TABLE `student` (
  `id` int(11) NOT NULL AUTO_INCREMENT,
  `first_name` varchar(45) DEFAULT NULL,
  `last_name` varchar(45) DEFAULT NULL,
  `email` varchar(45) DEFAULT NULL,
  PRIMARY KEY (`id`)
) ENGINE=InnoDB AUTO_INCREMENT=6 DEFAULT CHARSET=latin1;
LOCK TABLES `student` WRITE;
INSERT INTO `student` VALUES (1,'Mary','Public','mary@luv2code.com'),(2,'John','Doe','john@luv2code.com'),(3,'Ajay','Rao','ajay@luv2code.com'),(4,'Bill','Neely','bill@luv2code.com'),(5,'Maxwell','Dixon','max@luv2code.com');
UNLOCK TABLES;
```

**Reference Link: https://www.udemy.com/jsp-tutorial/learn/v4/overview**



