
**Prompt:**

Please create a web server using **FastAPI** in **Python** to handle submissions from a contact form.

### 🔗 API Endpoint:
- **URL:** `http://hostname/contact-form`
- **Method:** `POST`
- **Content-Type:** `application/json`

### 📤 Request JSON Format:
```json
{
  "name": "John Doe",
  "email": "john@example.com",
  "message": "Hello, I’d like to get in touch with you!"
}
```

### 📥 Response JSON Format:
On success:
```json
{
  "success": true,
  "message": "Your message has been received and forwarded to email."
}
```

On error:
```json
{
  "success": false,
  "error": "An error occurred while sending the message."
}
```

---

### 💡 Requirements:

1. **Use FastAPI** to create a web server that handles the `/contact-form` POST endpoint.
2. **Validate** input fields (`name`, `email`, `message`) as required non-empty strings.
3. After validation, **forward the message to a Gmail account** using Python's email libraries or Gmail SMTP.
4. You can use the following Gmail SMTP configuration:
   - SMTP server: `smtp.gmail.com`
   - Port: `587`
   - Use TLS
   - Authentication: Gmail email + App Password (not regular password)

5. The email should be formatted like:
   ```
   Subject: New Contact Form Submission
   From: John Doe <john@example.com>
   To: your-email@gmail.com

   Message:
   Hello, I’d like to get in touch with you!
   ```

6. Return the appropriate success/error JSON response.

7. You do **not** need to implement any front-end or HTML—only the FastAPI backend with email forwarding.
