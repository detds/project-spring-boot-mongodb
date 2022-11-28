# MongoDB Project with Spring Boot
[![License: MIT](https://img.shields.io/badge/License-MIT-yellowgreen.svg)](https://github.com/detds/project-spring-boot-mongodb/blob/main/LICENSE)

A simple **backend** system where we can **create**, **read**, **update** or **delete** (CRUD) users who have posts and respective comments on their posts. It also contains a **search method** to find posts that contain a certain string anywhere (title, body or comments) and within a certain date range.

This project was created with **Spring Boot** framework and **Java**, using **Spring Data MongoDB** to interact with **MongoDB database**.

## Technologies used

- Java 17
- Spring Boot 2 (Spring Web, Spring Data MongoDB)
- Maven
- MongoDB Database
- Postman

## UML Domain Model

![UML Domain Model](https://github.com/detds/project-spring-boot-mongodb/blob/main/assets/DomainModel_UML.png)

## UML Aggregation Association

![UML Aggragation Association](https://github.com/detds/project-spring-boot-mongodb/blob/main/assets/Aggregation_UML.png)

## Summary of HTTP methods and description of its actions

 Methods | Urls                                 | Actions 
 ------- | ------------------------------------ | ------- 
 POST    | /users                               | create new User 
 GET     | /users                               | find all Users 
 GET     | /users/:id                           | find a User by :id 
 PUT     | /users/:id                           | update a User by :id 
 DELETE  | /users/:id                           | delete a User by :id 
 GET     | /posts/:id                           | find a Post by :id 
 GET     | /posts/titlesearch?text=:string      | find posts whose title has a certain :string
 GET     | /posts/fullsearch?text=:string&minDate=:minDate&maxDate:maxDate | Find posts whose :string can be in the title, body or comments within a date range of :minDate and :maxDate
 
 ### Author
 
 Dennis Teles
 
 ### LinkedIn
