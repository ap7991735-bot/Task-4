# Task-4
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Job Application Form</title>

    <!-- ===== CSS Styling ===== -->
    <style>
        body {
            background: #f3f6fa;
            font-family: Arial, sans-serif;
            padding: 40px;
        }

        .container {
            max-width: 450px;
            margin: auto;
            background: #fff;
            padding: 25px;
            border-radius: 10px;
            box-shadow: 0px 0px 10px rgba(0,0,0,0.15);
        }

        h2 {
            text-align: center;
            margin-bottom: 20px;
        }

        label {
            font-weight: bold;
            display: block;
            margin-top: 15px;
        }

        input, textarea {
            width: 100%;
            padding: 10px;
            margin-top: 5px;
            border: 1px solid #ccc;
            border-radius: 5px;
        }

        textarea {
            height: 120px;
        }

        button {
            width: 100%;
            padding: 12px;
            background: #007bff;
            color: white;
            border: none;
            margin-top: 20px;
            border-radius: 5px;
            cursor: pointer;
            font-size: 16px;
        }

        button:hover {
            background: #0056b3;
        }

        .error {
            color: red;
            font-size: 14px;
        }

        .success {
            color: green;
            font-size: 16px;
            text-align: center;
            margin-top: 15px;
        }
    </style>
</head>
<body>

    <div class="container">
        <h2>Job Application Form</h2>

        <form id="applicationForm">
            <!-- Name field -->
            <label for="name">Name:</label>
            <input type="text" id="name" placeholder="Enter your name">

            <!-- Email field -->
            <label for="email">Email:</label>
            <input type="text" id="email" placeholder="Enter your email">

            <!-- Phone field -->
            <label for="phone">Phone:</label>
            <input type="text" id="phone" placeholder="Enter your phone number">

            <!-- Message field -->
            <label for="message">Message:</label>
            <textarea id="message" placeholder="Enter your message"></textarea>

            <div id="errorMsg" class="error"></div>
            <div id="successMsg" class="success"></div>

            <button type="submit">Submit Application</button>
        </form>
    </div>


    <!-- ===== JavaScript Validation ===== -->
    <script>
        document.getElementById("applicationForm").addEventListener("submit", function(event) {
            event.preventDefault(); // Prevent form submission

            let name = document.getElementById("name").value.trim();
            let email = document.getElementById("email").valu
