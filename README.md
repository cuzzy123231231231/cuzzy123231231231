<!DOCTYPE html>
<html>
<head>
    <title>Click to Say HI</title>
    <style>
        body {
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            margin: 0;
        }
        #popup {
            display: none;
            background-color: #f0f0f0;
            border: 1px solid #ccc;
            padding: 20px;
            position: absolute;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            z-index: 1000;
        }
    </style>
</head>
<body>
    <button id="clickMe">Click Me</button>
    <div id="popup">HI</div>
    <script>
        const clickMeButton = document.getElementById("clickMe");
        const popup = document.getElementById("popup");

        clickMeButton.addEventListener("click", function () {
            popup.style.display = "block";
        });

        popup.addEventListener("click", function () {
            popup.style.display = "none";
        });
    </script>
</body>
</html>
