# Full-Stack Employee Management System 👩‍💻
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
![System architecture diagram](https://i.imgur.com/ol8zvUP.png)


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

## Layered Architecture
![layered architecture diagram](https://i.imgur.com/5hJx1fS.png)
This diagram depicts the layered architecture of our application, illustrating how an HTTP request is handled from Postman to the database (DB) and back:

- **Postman:** Tool for sending HTTP requests to the API.
- **DTO:** Object that transfers data between layers.
- **Controller Layer:** Receives HTTP requests, processes them, and sends responses.
- **Service Layer:** Contains business logic and handles core operations.
- **Repository Layer:** Manages interaction with the database.
- **DB:** Persistently stores application data.

### The data flow is as follows:
1. Postman sends an HTTP request.
2. The controller receives the request and uses a DTO to transfer data to the service layer.
3. The service layer handles business logic and communicates with the repository layer.
4. The repository layer interacts with the database.
5. The response follows the reverse path, returning processed data to Postman.
