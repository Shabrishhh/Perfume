<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>I LOVE YOU CELESTE</title>
    <style>
        body {
            background-color: black;
            color: white;
            font-family: Arial, sans-serif;
            text-align: center;
            padding: 50px;
            position: relative;
            overflow: hidden;
        }
        h1 {
            color: pink;
        }
        p {
            max-width: 600px;
            margin: auto;
            line-height: 1.6;
        }
        .heart {
            position: absolute;
            width: 50px;
            height: 50px;
            background-color: red;
            clip-path: polygon(50% 0%, 100% 35%, 85% 100%, 50% 75%, 15% 100%, 0% 35%);
            opacity: 0.7;
            animation: float 5s linear infinite;
        }
        @keyframes float {
            0% {
                transform: translateY(100vh) scale(0.8);
                opacity: 1;
            }
            100% {
                transform: translateY(-10vh) scale(1.5);
                opacity: 0;
            }
        }
    </style>
</head>
<body>
    <h1>I LOVE YOU CELESTE</h1>
    <p>
        She wears his scent, not as a keepsake,<br>
        not as a gesture, but as something unspoken.<br>
        It settles on her skin,<br>
        a quiet presence,<br>
        a reminder of warmth.<br><br>
        Not his, not hers—just there,<br>
        familiar, steady,<br>
        woven into the air around them.
    </p>
    
    <script>
        function createHeart() {
            const heart = document.createElement("div");
            heart.classList.add("heart");
            heart.style.left = Math.random() * 100 + "vw";
            heart.style.animationDuration = (Math.random() * 3 + 2) + "s";
            document.body.appendChild(heart);
            setTimeout(() => heart.remove(), 5000);
        }
        setInterval(createHeart, 150);
    </script>
</body>
</html>

