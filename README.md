# Employee Management System 👩‍💻
A small project created using Spring Boot and React.js 💙

## Technology Stack
* Spring Boot 3
* React JS 18+
* Tailwind CSS
* Maven
* MySQL DB

## Requirements 
### Requirement #1
Build CRUD REST APIs (add, get, update and delete employees).

### Requirement #2
Build Frontend React App.

- [ ] Add New Employee
- [ ] List All Employee
- [ ] Update Existing Employee
- [ ] Delete Existing Employee

### Spring Boot React Full-Stack Architecture
For creating this Full-Stack application, we created a separate project for the frontend created with React and another project for the backend created with Spring Boot, so they are independent of each other.
![System architecture diagram](https://i.imgur.com/Cg21T9o.png)


### Some roles:
In the **client side**:
* `router` provides routes handling
* `components` reusable UI elements
* `services` communicates with the backend
* `axios` third-party library for making requests.

In the **server side**:
* `Spring Controller` exposes REST APIs
* `Service` contains the business logic
* `DAO` the responsable to talk with the DB
