<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>¿Me perdonas?</title>
    <style>
        body {
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            height: 100vh;
            background-color: #f0f8ff;
            font-family: Arial, sans-serif;
        }
        h1 {
            font-size: 2em;
            margin-bottom: 20px;
        }
        .buttons {
            display: flex;
            gap: 20px;
            margin-bottom: 20px;
        }
        button {
            padding: 10px 20px;
            font-size: 1em;
            cursor: pointer;
        }
        #thankYouMessage {
            display: none;
            text-align: center;
            margin-top: 20px;
        }
    </style>
</head>
<body>
    <h1>¿Me perdonas?</h1>
    <div class="buttons">
        <button id="yesButton">Sí</button>
        <button id="noButton">No</button>
    </div>
    <div id="thankYouMessage">
        <p>Gracias mi amor, te amo</p>
    </div>

    <script>
        document.getElementById('yesButton').addEventListener('click', function() {
            document.getElementById('thankYouMessage').style.display = 'block';
        });

        document.getElementById('noButton').addEventListener('click', function() {
            // No se hace nada cuando se clica "No"
        });
    </script>
</body>
</html>
