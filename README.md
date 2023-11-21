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
    

Frontend:

1. **HTML5:**
   - The document structure is defined using HTML5 tags such as `<!DOCTYPE html>`, `<html>`, `<head>`, `<meta>`, `<link>`, `<script>`, `<body>`, `<div>`, `<img>`, `<a>`, `<button>`, `<ul>`, `<li>`, `<nav>`, `<hr>`, `<p>`, etc.

2. **CSS:**
   - External styles are linked using the `<link>` tag with references to both a local CSS file (`format.css`) and an external CSS file from PureCSS and Mapbox.

3. **Vue.js:**
   - The Vue.js library is included via `<script>` tags. It's a JavaScript framework for building user interfaces, and it's utilized to dynamically generate menu items based on data (`v-for="ITEM in top_menu"`) and bind values to the DOM (`{{ITEM.title}}`).

4. **JavaScript:**
   - Several JavaScript files are included using `<script>` tags, namely `vue.js` and `tool.js`. These scripts likely contain custom JavaScript code for additional functionality.

5. **Mapbox:**
   - Mapbox is integrated into the page using Mapbox GL JS library. The Mapbox API is used to display a map (`<div id='map'></div>`) with a specified style (`'mapbox://styles/mapbox/streets-v11'`). The access token is provided in the script (`mapboxgl.accessToken`).

6. **Responsive Design:**
   - PureCSS is used for styling, and it provides a responsive grid system and various styles for UI components. The class `pure-button pure-button-primary` is from PureCSS, styling a login button.

7. **Asynchronous Loading:**
   - The `defer` attribute is used for asynchronous loading of JavaScript files, ensuring that the scripts are executed in order after the HTML has been fully parsed.

In summary, the provided HTML document uses HTML5 for structure, CSS for styling (including styles from PureCSS and Mapbox), Vue.js for dynamic content, JavaScript for scripting and functionality, and Mapbox for displaying an interactive map.

Backend:
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
