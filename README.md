## Hi there 👋

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Techno Circle Animation</title>
    <style>
        body {
            margin: 0;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            background: black;
        }

        .container {
            display: flex;
            gap: 20px;
        }

        .circle {
            width: 100px;
            height: 100px;
            border-radius: 50%;
            background: #00ffea;
            opacity: 0.7;
            animation: pulse 1.5s infinite ease-in-out;
        }

        /* Define the pulsing animation */
        @keyframes pulse {
            0% {
                transform: scale(0.8);
                opacity: 0.5;
            }
            50% {
                transform: scale(1.5);
                opacity: 1;
            }
            100% {
                transform: scale(0.8);
                opacity: 0.5;
            }
        }

        /* Stagger the animation of the circles for a techno rhythm effect */
        .circle:nth-child(2) {
            animation-delay: 0.2s;
        }

        .circle:nth-child(3) {
            animation-delay: 0.4s;
        }
    </style>
</head>
<body>

    <div class="container">
        <div class="circle"></div>
        <div class="circle"></div>
        <div class="circle"></div>
    </div>

</body>
</html>
