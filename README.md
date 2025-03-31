# Wedding-QR
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Wedding QR</title>
    <style>
        body {
            background-color: #f5efe7;
            text-align: center;
            font-family: 'Arial', sans-serif;
            color: #8b5e3c;
            overflow: hidden;
        }
        h1 {
            font-family: 'Dancing Script', cursive;
            font-size: 2.5rem;
            margin-top: 50px;
        }
        .decorations {
            position: absolute;
            width: 100%;
            top: 0;
            left: 0;
            pointer-events: none;
        }
        .star, .bell, .ring, .celebration {
            position: absolute;
            animation: float 5s infinite ease-in-out;
        }
        @keyframes float {
            0%, 100% { transform: translateY(0); }
            50% { transform: translateY(20px); }
        }
        .star { color: gold; font-size: 30px; left: 10%; animation-duration: 4s; }
        .bell { color: goldenrod; font-size: 40px; left: 50%; animation-duration: 6s; }
        .ring { color: #d4af37; font-size: 35px; right: 10%; animation-duration: 5s; }
        .celebration {
            font-size: 50px;
            position: absolute;
            bottom: 10%;
            left: 50%;
            transform: translateX(-50%);
            animation: bounce 1s infinite;
        }
        @keyframes bounce {
            0%, 100% { transform: translate(-50%, 0); }
            50% { transform: translate(-50%, -10px); }
        }
    </style>
    <link href="https://fonts.googleapis.com/css2?family=Dancing+Script:wght@600&display=swap" rel="stylesheet">
</head>
<body>
    <div class="decorations">
        <div class="star">⭐</div>
        <div class="bell">🔔</div>
        <div class="ring">💍</div>
    </div>
    <h1>Welcome to Our Special Celebration</h1>
    <p>Join us in celebrating this beautiful occasion of Alma and Roce!</p>
    <div class="celebration">🎉🥳🎊</div>
</body>
</html>
