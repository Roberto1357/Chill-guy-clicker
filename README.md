# Chill-guy-clicker
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Chill Guy Clicker</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            background-color: #f0f0f0;
            margin: 0;
            padding: 0;
        }

        .container {
            margin: 50px auto;
            padding: 20px;
            max-width: 600px;
            background: #ffffff;
            border-radius: 10px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
        }

        h1 {
            font-size: 2em;
            color: #333;
        }

        p {
            font-size: 1.5em;
            color: #666;
            margin: 20px 0;
        }

        #chillGuyContainer {
            display: flex;
            justify-content: center;
            margin-top: 20px;
        }

        #chillGuy {
            width: 200px;
            height: auto;
            cursor: pointer;
            transition: transform 0.2s ease;
        }

        #chillGuy:active {
            transform: scale(1.1);
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>Chill Guy Clicker</h1>
        <p>Klicks: <span id="clickCount">0</span></p>
        <div id="chillGuyContainer">
            <img id="chillGuy" src="https://i.imgur.com/W4ckW0A.jpg" alt="Chill Guy Meme">
        </div>
    </div>
    <script>
        let clickCount = 0;

        // Referenz zum Klickzähler und zum Bild
        const clickCountElement = document.getElementById("clickCount");
        const chillGuy = document.getElementById("chillGuy");

        // Funktion: Erhöht den Klickzähler
        function increaseClickCount() {
            clickCount++;
            clickCountElement.textContent = clickCount;
        }

        // Event Listener: Klicke auf das Chill Guy Bild
        chillGuy.addEventListener("click", increaseClickCount);
    </script>
</body>
</html>
