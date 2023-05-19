
<h1 align="center"> 
 DoctorApp </h1>

<p align="center">
<a href="Java url">
    <img alt="Java" src="https://img.shields.io/badge/Java->=8-darkblue.svg" />
</a>
<a href="Maven url" >
    <img alt="Maven" src="https://img.shields.io/badge/maven-3.0.5-brightgreen.svg" />
</a>
<a href="Spring Boot url" >
    <img alt="Spring Boot" src="https://img.shields.io/badge/Spring Boot-3.0.6-brightgreen.svg" />
</a>

<a >
    <img alt="MySQL" src="https://img.shields.io/badge/MySQL-blue.svg">
</a>
</p>

This is a Spring Boot project for an  DoctorApp that allows users to manage pateint,doctor, autentication, and ENUM for specialization. The project uses MySQL for storing data, Hibernate for object-relational mapping, and Maven for building the project.



<br>

## Framework Used
* Spring Boot

---
<br>

## Dependencies
The following dependencies are required to run the project:

* Spring Boot Dev Tools
* Spring Web
* Spring Data JPA
* MySQL Driver
* Lombok
* Validation
* Swagger

<br>

## Database Configuration
To connect to a MySQL database, update the application.properties file with the appropriate database URL, username, and password. The following properties need to be updated:
```
spring.datasource.driverClassName=com.mysql.cj.jdbc.Driver
spring.datasource.url = jdbc:mysql://localhost:3306/<DatabaseName>
spring.datasource.username = <userName>
spring.datasource.password = <password>
spring.jpa.show-sql = true
spring.jpa.hibernate.ddl-auto = update
spring.jpa.properties.hibernate.show_sql=true
spring.jpa.properties.hibernate.use_sql_comments=true
spring.jpa.properties.hibernate.format_sql=true
```
<br>

## Language Used
* Java

---
<br>

## Models
The following models are available:

Doctor
* id (integer) - The doctor ID.
* name (string) - The user name.
* specialization (ENUM) - The Doctor specialization.

Patient
* integer -  patientId;
* String- patientFirstName;
* String patientLastName;
* String patientEmail;
* String patientPassword;
* String patientContact;

 Appointment
 
 *  AppointmentKey id;
 *  Doctor doctor;
 * Patient patient;
 
Autentication Token
 * Long tokenId;
 * String token;
 * LocalDate tokenCreationDate;
 *  Patient patient;


## Data Flow

1. The user at client side sends a request to the application through the API endpoints.
2. The API receives the request and sends it to the appropriate controller method.
3. The controller method makes a call to the method in service class.
4. The method in service class builds logic and retrieves or modifies data from the database, which is in turn given to controller class
5. The controller method returns a response to the API.
6. The API sends the response back to the user.

---

<br>






>## Project Summary
This project provides a starting point for building a Spring Boot doctor API. It includes the basic functionality required for managing patient ,doctor and appointment and can be extended to meet the specific needs of your application.


## Author

👤 **Pooja Gurnule**

* GitHub: [Pooja Gurnule](https://github.com/poojagurnule)



---

## 🤝 Contributing

Contributions, issues and feature requests are welcome!<br />Feel free to check [issues page]("url").

---

## Show your support

Give a ⭐️ if this project helped you!

---

## 📝 License

Copyright © 2023 [Pooja Gurnule](https://github.com/poojagurnule).<br />



---
