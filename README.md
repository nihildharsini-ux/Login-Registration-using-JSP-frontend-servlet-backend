Login + Registration Using JSP Frontend + Servlet Backend

Objective:
To build a complete authentication system using JSP forms and a central Servlet.

Description:
•	register.jsp → collects username & password
•	login.jsp → collects login details
•	Servlet receives data via request parameters
•	Performs JDBC insert (for register) and JDBC select (for login)
•	Servlet returns response messages back to JSP
•	register.jsp + login.jsp
•	One Servlet (RegisterLoginServlet)
•	JDBC for validation
•	Proper routing based on req.getServletPath()

Database:
CREATE DATABASE authdb;

USE authdb;

CREATE TABLE users (
    id INT AUTO_INCREMENT PRIMARY KEY,
    username VARCHAR(50) UNIQUE,
    password VARCHAR(50)
);












