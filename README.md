<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Run HTML Code</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f4f4f4;
            text-align: center;
            padding: 20px;
        }
        textarea {
            width: 80%;
            height: 150px;
            font-family: monospace;
            padding: 10px;
            font-size: 16px;
            margin: 10px 0;
        }
        button {
            padding: 10px 20px;
            background-color: #4CAF50;
            color: white;
            font-size: 16px;
            border: none;
            cursor: pointer;
        }
        button:hover {
            background-color: #45a049;
        }
        #output {
            margin-top: 20px;
            padding: 20px;
            border: 1px solid #ccc;
            background-color: white;
            min-height: 50px;
        }
    </style>
</head>
<body>

    <h1>Run Your HTML Code</h1>
    <p>Type your HTML code below and click "Render HTML" to see the result:</p>

    <!-- Textarea for HTML input -->
    <textarea id="htmlInput">&lt;h2&gt;Hello, World!&lt;/h2&gt;</textarea><br>

    <!-- Button to render HTML -->
    <button onclick="renderHTML()">Render HTML</button>

    <!-- Area where the HTML will be rendered -->
    <div id="output"></div>

    <script>
        function renderHTML() {
            // Get the HTML code from the textarea
            const htmlCode = document.getElementById('htmlInput').value;
            
            // Render the HTML code inside the 'output' div
            document.getElementById('output').innerHTML = htmlCode;
        }
    </script>

</body>
</html>
