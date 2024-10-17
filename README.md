<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Happy Birthday!</title>
    <style>
        body {
            font-family: 'Arial', sans-serif;
            background-color: #f0e4d7;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            margin: 0;
        }

        .card {
            background-color: #fff;
            border-radius: 10px;
            box-shadow: 0px 8px 15px rgba(0, 0, 0, 0.1);
            padding: 40px;
            text-align: center;
            max-width: 500px;
            width: 100%;
        }

        h1 {
            font-size: 2.5em;
            color: #ff6f61;
        }

        .balloons {
            font-size: 3em;
            margin-bottom: 20px;
        }

        input[type="date"] {
            padding: 10px;
            width: 70%;
            border-radius: 5px;
            border: 1px solid #ddd;
            font-size: 1.1em;
        }

        button {
            margin-top: 20px;
            background-color: #ff6f61;
            border: none;
            color: white;
            padding: 15px 30px;
            font-size: 1.2em;
            cursor: pointer;
            border-radius: 5px;
        }

        button:hover {
            background-color: #e65a4f;
        }

        .message {
            font-size: 1.5em;
            color: #333;
            margin-top: 30px;
        }
    </style>
</head>
<body>
    <div class="card">
        <div class="balloons">🎈🎉🎂</div>
        <h1>Happy Birthday!</h1>
        <p>Enter your birth date to receive a special message<br>
        from Pranto and Siraj:</p>
        <input type="date" id="birthday" name="birthday">
        <button onclick="showMessage()">Get Message</button>
        <div class="message" id="message"></div>
    </div>

    <script>
        function showMessage() {
            const birthday = document.getElementById("birthday").value;
            const messageDiv = document.getElementById("message");

            if (birthday) {
                messageDiv.textContent = "Wishing you a day filled with love, joy, and wonderful moments. Happy Birthday sweety!Give us treat as soon as posible";
            } else {
                messageDiv.textContent = "Please select your birth date!";
            }
        }
    </script>
</body>
</html>
