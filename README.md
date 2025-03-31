<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Alma & Roce - Wedding Celebration</title>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Great+Vibes&family=Cormorant+Garamond:wght@700&display=swap');
        body {
            background: linear-gradient(to bottom, #ffecd1, #ffb3c1, #ffc3a0);
            text-align: center;
            font-family: 'Cormorant Garamond', serif;
            color: #5a3d2b;
            overflow: hidden;
            position: relative;
        }
        h1 {
            font-size: 4rem;
            margin-top: 30px;
            color: #8B0000;
            font-family: 'Great Vibes', cursive;
        }
        .couple-name {
            font-size: 5rem;
            font-weight: bold;
            color: #b30000;
            text-transform: uppercase;
            font-family: 'Great Vibes', cursive;
            margin-top: 20px;
        }
        p {
            font-size: 1.8rem;
            margin: 10px 0;
        }
        .banner {
            background: url('https://your-banner-image.com') no-repeat center center/cover;
            height: 250px;
            margin-bottom: 20px;
            border-radius: 20px;
        }
        .invitation-box {
            background: rgba(255, 255, 255, 0.85);
            padding: 30px;
            border-radius: 20px;
            display: inline-block;
            box-shadow: 0px 0px 15px rgba(0, 0, 0, 0.2);
            width: 70%;
        }
        .date-box {
            font-size: 2.8rem;
            font-weight: bold;
            color: #c0392b;
            background: #fce4ec;
            padding: 10px 30px;
            border-radius: 15px;
            display: inline-block;
            margin-top: 15px;
            font-family: 'Great Vibes', cursive;
        }
        .venue {
            font-size: 1.8rem;
            font-weight: bold;
            color: #5a3d2b;
        }
        .venue a {
            text-decoration: none;
            color: #8B0000;
        }
        .venue a:hover {
            text-decoration: underline;
        }
        .car {
            position: absolute;
            bottom: 50px;
            left: 10%;
            width: 120px;
            height: 80px;
            background: url('https://your-red-black-car-image.com') no-repeat center center/cover;
            cursor: pointer;
            animation: moveCar 5s ease-in-out infinite;
        }
        @keyframes moveCar {
            0% {
                left: 10%;
                transform: rotate(0deg);
            }
            50% {
                left: 80%;
                transform: rotate(10deg);
            }
            100% {
                left: 10%;
                transform: rotate(0deg);
            }
        }
        .smoke {
            position: absolute;
            bottom: 100px;
            left: 50%;
            transform: translateX(-50%);
            width: 150px;
            height: 50px;
            background: url('https://your-smoke-image-link.com') no-repeat center center/cover;
            opacity: 0.6;
            animation: smokeEffect 1s infinite;
        }
        @keyframes smokeEffect {
            0% {
                opacity: 0.6;
                transform: translateX(-50%) scale(1);
            }
            50% {
                opacity: 0.2;
                transform: translateX(-50%) scale(1.5);
            }
            100% {
                opacity: 0.6;
                transform: translateX(-50%) scale(1);
            }
        }
        .location1, .location2 {
            position: absolute;
            top: 50%;
            transform: translateY(-50%);
            width: 50px;
            height: 50px;
            background: url('https://your-location-icon-link.com') no-repeat center center/cover;
            cursor: pointer;
        }
        .location1 {
            left: 10%;
        }
        .location2 {
            right: 10%;
        }
        .location1:hover, .location2:hover {
            opacity: 0.7;
        }
        .quote {
            font-style: italic;
            font-size: 2rem;
            margin-bottom: 20px;
            color: #8B0000;
            font-family: 'Great Vibes', cursive;
        }
        .heart {
            font-size: 3.5rem;
            cursor: pointer;
            transition: color 0.5s ease-in-out;
            display: inline-block;
            margin-top: 20px;
            color: red;
        }
        .heart.active {
            color: #ff69b4;
        }
        .fireworks {
            position: absolute;
            top: 10%;
            left: 50%;
            transform: translateX(-50%);
            animation: fireworks 1s infinite;
            z-index: 2;
        }
        @keyframes fireworks {
            0% {
                transform: translateX(-50%) scale(0.5);
                opacity: 0;
            }
            100% {
                transform: translateX(-50%) scale(1.5);
                opacity: 1;
            }
        }
        .crackers {
            background: url('https://your-crackers-image.com') no-repeat center center/cover;
            height: 200px;
            position: absolute;
            bottom: 0;
            width: 100%;
            z-index: -2;
        }
    </style>
    <script>
        function goToLocation(location) {
            if (location === 1) {
                window.location.href = "https://maps.app.goo.gl/2D7oGVRd4yptLPxg9?g_st=aw";
            } else if (location === 2) {
                window.location.href = "https://maps.app.goo.gl/Kzf5KGDBpRRDwzky9?g_st=aw";
            }
        }
    </script>
</head>
<body>
    <div class="stars"></div>
    <div class="leaves"></div>
    <div class="fireworks"></div>
    <div class="crackers"></div>
    <div class="banner"></div>
    <div class="invitation-box">
        <h1>With Love & Blessings</h1>
        <p class="quote">"Two hearts, one journey, a lifetime of love begins!"</p>
        <h1 class="couple-name">ALMA & ROCE</h1>
        <p class="date-box">15th April 2025</p>
        <p class="venue">Venue: At our residence, Hebbal Hatti</p>
        <p>Double-tap the heart to see the location</p>
    </div>
    <div class="location1" onclick="goToLocation(1)"></div>
    <div class="location2" onclick="goToLocation(2)"></div>
    <div class="car"></div>
    <div class="smoke"></div>
</body>
</html>
