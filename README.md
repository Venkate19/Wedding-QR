<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Wedding Invitation</title>
    <style>
        body {
            background-color: #f5efe7;
            text-align: center;
            font-family: 'Dancing Script', cursive;
            color: #8b5e3c;
            overflow: hidden;
        }
        h1 {
            font-size: 3rem;
            margin-top: 50px;
        }
        p {
            font-size: 1.5rem;
        }
        .decorations {
            position: absolute;
            width: 100%;
            top: 0;
            left: 0;
            pointer-events: none;
        }
        .banner {
            background: url('https://your-image-link.com') no-repeat center center/cover;
            height: 200px;
            margin-bottom: 20px;
        }
        .invitation-box {
            background: rgba(255, 255, 255, 0.9);
            padding: 20px;
            border-radius: 15px;
            display: inline-block;
            box-shadow: 0px 0px 10px rgba(0, 0, 0, 0.2);
        }
        .date {
            font-size: 2rem;
            font-weight: bold;
            color: #d4af37;
        }
        .venue a {
            color: #8b5e3c;
            font-weight: bold;
            text-decoration: none;
        }
        .venue a:hover {
            text-decoration: underline;
        }
    </style>
    <link href="https://fonts.googleapis.com/css2?family=Dancing+Script:wght@600&display=swap" rel="stylesheet">
</head>
<body>
    <div class="banner"></div>
    <div class="invitation-box">
        <h1>You're Invited!</h1>
        <p>Join us in celebrating the beautiful occasion of Alma and Roce</p>
        <p class="date">Date: 15th April 2025</p>
        <p class="venue">Venue: <a href="https://maps.google.com/?q=Your+Venue+Address" target="_blank">[Your Venue Name]</a></p>
    </div>
</body>
</html>

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
