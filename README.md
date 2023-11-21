# wdc_group_project
Account details:
User:
    ID:1
    password:123456
    
Admin:
    ID:2
    password:123456
    
Manager:
    ID:1
    password:123456
    
Here are the key technologies and concepts used in the provided code:

1. **Express.js:**
   - Web application framework for Node.js.

2. **Session Management:**
   - `req.session` for storing and retrieving user information.

3. **Middleware for Database Connection Pooling:**
   - Use of `req.pool.getConnection` for managing database connections.

4. **MySQL Queries:**
   - Interacting with a MySQL database for retrieving and updating user information, fetching trip details, and getting hotspots.

5. **Routing:**
   - Defining routes for handling different HTTP requests (`GET`, `POST`) on various endpoints.

6. **RESTful API Endpoints:**
   - Designing endpoints such as `/getUserInfor`, `/updateInfor`, `/getTrips`, and `/getHotspots` to provide specific functionalities over HTTP.

7. **JSON Responses:**
   - Returning data in JSON format using `res.json()`.

8. **Data Retrieval and Update:**
   - Executing SQL queries to retrieve user information, update user details, and fetch trip and hotspot data.

9. **Dynamic SQL Query Building:**
   - Constructing SQL queries dynamically based on the parameters received in the request.

10. **Conditional Statements:**
    - Using conditional statements to check and modify data based on certain conditions, such as health status.

11. **Error Handling:**
    - Implementing error handling with `res.sendStatus(500)` for database connection and query errors.
