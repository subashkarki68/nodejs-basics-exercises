# nodejs-basics-exercises

# Node.js Web Server Examples

## Hello World Server:

Set up a basic HTTP server using a framework or the built-in Node.js `http` module.
Configure the server to respond with "Hello, World!" for all incoming requests.

**Example:**
- **Request:** `GET /`
- **Response:** `Hello, World!`

## Dynamic Content:

Modify your server to extract the name from the URL path using routing mechanisms.
Respond with a personalized greeting using the extracted name.

**Example:**
- **Request:** `GET /greet/John`
- **Response:** `Hello, John!`

## Query Parameters:

Update your server to parse and extract query parameters from the incoming request.
Include the extracted name from the query parameters in the response.

**Example:**
- **Request:** `GET /greet?name=Alice`
- **Response:** `Hello, Alice!`

## Static File Server:

Use the Node.js `fs` module to read and serve static HTML files.
Create an HTML file and configure your server to serve it when a specific route is requested.

**Example:**
- **Request:** `GET /static.html`
- **Response:** Contents of static.html file

## 404 Not Found:

Implement a mechanism to handle undefined routes.
Respond with a 404 Not Found status code along with a custom error message.

**Example:**
- **Request:** `GET /nonexistent`
- **Response:** `404 Not Found - Custom error message`

# JSON Response

Create a new route that returns a JSON object. Populate the JSON object with various pieces of information.

**Example:**
- **Request:** `GET /api/data`
- **Response:** `{"name": "John", "age": 25, "city": "Example City"`

# Header Manipulation

Explore the Node.js `response.setHeader` method to modify the response headers. Experiment with setting custom headers like `Content-Type` and `Cache-Control`.

**Example:**
- **Request:** `GET /`
- **Response:**
    ```yaml
    Hello, World!
    Content-Type: application/json
    Cache-Control: no-cache
    ```

# Redirects

Implement a new route that triggers a redirect to another URL. Choose an appropriate HTTP status code for redirection (e.g., 301 or 302).

**Example:**
- **Request:** `GET /redirect`
- **Response:** `302 Found - Redirecting to /new-location`

# Method Handling

Extend your server to handle different HTTP methods (GET, POST, etc.) for a specific route. Customize the server response based on the method used.

**Example:**
- **Request:** `POST /submit`
- **Response:** `POST request received`
  
# Middleware Basics

Create a middleware function that logs information about each incoming request. Include details such as the request method, URL, and a timestamp.

**Example:**
- Middleware Log: `GET request at / - Timestamp: 2024-02-07 12:34:56`

# Request Body Parsing

Update your server to handle POST requests. Extract data from the request body and respond with a message that includes the posted data.

**Example:**
- Request: `POST /submit` - Body: `{"username": "user123", "password": "pass123"}`
- Response: `Data received from user123`

  # Server Shutdown

Implement a mechanism to capture the termination signal (`SIGINT`). Gracefully close the server before exiting the application.

**Example:**
- Console Output:

    ```arduino
    Server is shutting down gracefully...
    Server closed. Application exiting.
    ```

