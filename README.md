<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Do you like me?</title>
    <style>
        body {
            text-align: center;
            font-family: Arial, sans-serif;
            background-color: #f0f8ff;
            margin-top: 50px;
        }
        button {
            padding: 10px 20px;
            font-size: 18px;
            margin: 10px;
            cursor: pointer;
            border: none;
            border-radius: 5px;
            transition: background-color 0.3s;
        }
        #yes {
            background-color: #4CAF50;
            color: white;
        }
        #no {
            background-color: #f44336;
            color: white;
        }
    </style>
</head>
<body>

    <h1>làm bồ anh nhé ?</h1>
    <button id="yes">Yes</button>
    <button id="no">No</button>

    <script>
        document.getElementById("yes").onclick = function() {
            alert("iu thế!");
        }

        document.getElementById("no").onclick = function() {
            // Get the button element
            const noButton = document.getElementById("no");
            
            // Generate random position
            const randomX = Math.random() * (window.innerWidth - noButton.offsetWidth);
            const randomY = Math.random() * (window.innerHeight - noButton.offsetHeight - 100); // Keep it within the viewport

            // Set the button's new position
            noButton.style.position = "absolute"; // Make position absolute to move it freely
            noButton.style.left = randomX + "px";
            noButton.style.top = randomY + "px";
        }
    </script>

</body>
</html>

