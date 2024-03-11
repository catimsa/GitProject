# GitProject
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Random Quote Generator</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            margin: 0;
            padding: 0;
        }
        #quote {
            font-size: 24px;
            margin: 20px auto;
            max-width: 80%;
        }
        #generate-btn {
            padding: 10px 20px;
            font-size: 18px;
            background-color: #007bff;
            color: #fff;
            border: none;
            cursor: pointer;
        }
    </style>
</head>
<body>
    <h1>Random Quote Generator</h1>
    <div id="quote"></div>
    <button id="generate-btn" onclick="generateQuote()">Generate Quote</button>

    <script>
        // Array of quotes
        const quotes = [
            "The only way to do great work is to love what you do. - Steve Jobs",
            "In the midst of chaos, there is also opportunity. - Sun Tzu",
            "Success is not final, failure is not fatal: It is the courage to continue that counts. - Winston Churchill",
            "Believe you can and you're halfway there. - Theodore Roosevelt",
            "The best way to predict the future is to invent it. - Alan Kay",
            "It does not matter how slowly you go as long as you do not stop. - Confucius"
        ];

        function generateQuote() {
            // Generate a random index
            const index = Math.floor(Math.random() * quotes.length);
            // Display the random quote
            document.getElementById('quote').innerHTML = quotes[index];
        }
    </script>
</body>
</html>
