<!DOCTYPE html>
<html>
<head>
    <title>Animated Text</title>
    <style>
        /* CSS Styles */
        body {
            background: linear-gradient(45deg, #1c92d2, #f0643b, #ffdd71, #30e8bf);
            background-size: 600% 600%;
            animation: gradient-slide 10s ease infinite;
            height: 100vh;
            display: flex;
            align-items: center;
            justify-content: center;
            overflow: hidden;
        }

        .animated-text {
            font-family: "Arial", sans-serif;
            font-size: 64px;
            font-weight: bold;
            color: #ffffff;
            opacity: 0;
            animation: fade-in 1s ease-in-out 1s forwards, bounce 1s ease-in-out infinite;
        }

        @keyframes gradient-slide {
            0% {
                background-position: 0% 50%;
            }
            50% {
                background-position: 100% 50%;
            }
            100% {
                background-position: 0% 50%;
            }
        }

        @keyframes fade-in {
            0% { opacity: 0; }
            100% { opacity: 1; }
        }

        @keyframes bounce {
            0%, 100% { transform: translateY(0); }
            50% { transform: translateY(-10px); }
        }
    </style>
</head>
<body>
    <div class="animated-text">Hello, I'm Chickaboo!</div>

    <script>
        // JavaScript code (optional)
        // You can add additional functionality or interactivity here if needed
    </script>
</body>
</html>
