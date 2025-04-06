**Prompt:**

Create a web server using **raw TCP socket programming in Python** (without using any frameworks like Flask or FastAPI). The server should demonstrate handling of the following HTTP methods:

### ✅ Supported HTTP Methods:
- **GET**
- **POST**
- **PUT**
- **DELETE**

### 🛠️ Requirements:

1. **Basic HTTP Server with Raw TCP Socket**
   - Handle HTTP 1.1 requests over a raw socket
   - Parse the HTTP method, headers, and body manually

2. **GET (Static Content)**
   - Serve a simple `index.html` file when accessing `/`
   - The `index.html` should include a basic interface (e.g., buttons or forms) to test all four HTTP methods using JavaScript `fetch()`

3. **GET (RESTful API)**
   - Provide a test endpoint: `GET /api/message`
   - Return JSON like:
     ```json
     { "message": "Hello from the raw TCP server!" }
     ```

4. **POST /api/data**
   - Accept a JSON payload in the request body
   - Return a success JSON response with the received data echoed back

5. **PUT /api/data**
   - Accept a JSON payload in the request body
   - Return a message like `"Data updated successfully"`

6. **DELETE /api/data**
   - Accept a JSON payload (e.g., containing an `id` to delete)
   - Return a message like `"Data deleted successfully"`

### 🧪 Test Page (index.html):
- Simple web interface with buttons or forms to test all methods using JavaScript
- Use `fetch()` to send requests to the server
- Show the server response in the browser

### 💡 Notes:
- Everything should be implemented with only the Python standard library (`socket`, `json`, etc.)
- No third-party HTTP libraries should be used
- You can hard-code or simulate storage (no need for a real database)
- Focus on demonstrating the HTTP methods and raw socket parsing
