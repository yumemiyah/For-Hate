<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Tap to Open</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            margin: 0;
            background-color: #f0f8ff;
        }

        .button {
            background-color: #ff7f50;
            color: white;
            padding: 15px 30px;
            font-size: 20px;
            border-radius: 10px;
            cursor: pointer;
            transition: background-color 0.3s;
        }

        .button:hover {
            background-color: #ff4500;
        }

        .message {
            display: none;
            margin-top: 20px;
            background-color: #ffebcd;
            padding: 20px;
            border-radius: 10px;
            font-size: 18px;
            text-align: center;
        }
    </style>
</head>
<body>

    <div>
        <button class="button" onclick="showMessage()">Tap to open me</button>
        <div class="message" id="message">
            <p>Hello, you just revealed the message! 🎉</p>
        </div>
    </div>

    <script>
        function showMessage() {
            var message = document.getElementById('message');
            message.style.display = 'block'; // Show the hidden message
        }
    </script>

</body>
</html>