<h1 align="center">
Instagram Project </h1>

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

This is an Instagram-inspired project built with Spring Boot. The user controller handles various user-related operations in the application. The project exposes RESTful endpoints for user management, authentication, liking posts, following other users, and more.


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

> ## Data Flow

1. The user at client side sends a request to the application through the API endpoints.
2. The API receives the request and sends it to the appropriate controller method.
3. The controller method makes a call to the method in service class.
4. The method in service class builds logic and retrieves or modifies data from the database, which is in turn given to controller class
5. The controller method returns a response to the API.
6. The API sends the response back to the user.
>## Schema
The following schemas are used in the project:

* **User:** Represents user information including user ID, name, Instagram details, password, email, phone number, blue tick status, and date of birth.
* **SignUpOutput:** Contains the status and message of the sign-up operation.
SignInInput: Includes the email and password for user authentication during sign-in.
* **SignInOutput:** Provides the status and token after successful user authentication.
* **Post:** Represents a post with a post ID, creation date, post data, caption, location, and associated user.
* **PostLike:** Represents a like given to a post, including the like ID, the post being liked, and the user who liked it.
* **InstagramComment:** Represents a comment on a post, including the comment ID, comment body, the post being commented on, and the user who made the comment.

Please note that the actual implementation and details of these schemas may vary within the project code.

> ## Endpoints

* PUT /user
Update user information.

* POST /user/signup
Create a new user account.

* POST /user/signin
Authenticate and sign in a user.

* POST /user/like
Like a post.

* POST /user/follow/{myId}/{otherId}
Follow another user.

* DELETE /user/signout
Sign out the currently authenticated user.

* Admin Controller
The project also includes an admin controller for administrative tasks.

* PUT /admin/user/{id}/{blueTick}
Assign a blue tick (verification badge) to a user.

* Post Controller
The post controller handles post-related operations.

* GET /post
Retrieve all posts.

* POST /post
Create a new post.

* GET /post/{postId}/likeCount
Get the number of likes for a specific post.

* Comment Controller
The comment controller manages comments on posts.

* POST /comment
Add a new comment to a post.



>## Project Summary
This project is an Instagram-inspired application developed using Spring Boot. It aims to provide users with a platform to share and interact with posts, follow other users, like posts, and comment on them. The project utilizes RESTful APIs to expose various endpoints for user management, authentication, post handling, and comment management.

The project provides a solid foundation for building an Instagram-like application using Spring Boot. Developers can extend and enhance the functionality by adding additional features such as user profiles, direct messaging, explore pages, and image/video uploads.

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
