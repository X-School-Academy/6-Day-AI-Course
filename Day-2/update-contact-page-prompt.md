**Prompt:**

Please update the contact page code to integrate with my new api backend.

### 📝 What to update:
Add JavaScript code that sends form data to the following API when the form is submitted.

### 🔗 API Details:
- **Endpoint:** `http://hostname/contact-form`
- **Method:** `POST`
- **Content-Type:** `application/json`
- **Expected JSON Format:**
```json
{
  "name": "John Doe",
  "email": "john@example.com",
  "message": "Hi, I’d like to connect!"
}
```

### ✅ On Success:
- Show a confirmation message like: `Thank you for reaching out!`

### ❌ On Error:
- Show an error message like: `Something went wrong. Please try again later.`

### ⚙️ Additional Requirements:
- Use **vanilla JavaScript** (no external libraries).
- Prevent the default form submission behavior.
- Use `fetch()` to make the POST request.
- Add basic validation to ensure all fields are filled before submitting.
- Keep everything in the existing HTML/CSS/JavaScript structure (no backend modifications needed here).
