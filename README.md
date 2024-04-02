<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Student Registration Form</title>
<style>
    body {
        font-family: Arial, sans-serif;
        background-color: #f2f2f2; /* Changed background color */
    }
    form {
        max-width: 400px;
        margin: 0 auto;
        background-color: white;
        padding: 20px;
        border-radius: 8px;
        box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
    }
    label {
        display: block;
        margin-bottom: 5px;
    }
    input, select, textarea {
        width: 100%;
        padding: 8px;
        margin-bottom: 10px;
        box-sizing: border-box;
    }
    button {
        padding: 10px 20px;
        background-color: #007bff; /* Blue color */
        color: white;
        border: none;
        cursor: pointer;
        border-radius: 5px;
    }
    button:hover {
        background-color: #0056b3; /* Darker shade of blue on hover */
    }
</style>
</head>
<body>

<h2>Student Registration Form</h2>

<form action="/submit_registration" method="post">
    <label for="name">Name:</label>
    <input type="text" id="name" name="name" required>

    <label for="dob">Date of Birth:</label>
    <input type="date" id="dob" name="dob" required>

    <label for="gender">Gender:</label>
    <select id="gender" name="gender" required>
        <option value="">Select</option>
        <option value="male">Male</option>
        <option value="female">Female</option>
        <option value="other">Other</option>
    </select>

    <label for="address">Address:</label>
    <textarea id="address" name="address" required></textarea>

    <label for="telephone">Telephone:</label>
    <input type="tel" id="telephone" name="telephone" required>

    <label for="email">Email Address:</label>
    <input type="email" id="email" name="email" required>

    <label for="course">Course:</label>
    <input type="text" id="course" name="course" required>

    <button type="submit">Register</button>
    <button type="button" onclick="window.location.href='/cancel_registration'">Cancel</button>
</form>

</body>
</html>
