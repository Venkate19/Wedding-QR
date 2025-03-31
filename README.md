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
        .stars, .leaves {
            position: absolute;
            width: 100%;
            height: 100%;
            top: 0;
            left: 0;
            opacity: 0.3;
            z-index: -1;
        }
        .stars {
            background: url('https://your-stars-image.com') repeat;
        }
        .leaves {
            background: url('https://your-leaves-image.com') repeat;
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
    </style>
    <script>
        setTimeout(function() {
            window.location.href = "https://maps.google.com/?q=Hebbal+hatti";
        }, 6000); // Redirects after 6 seconds

        function goToLocation() {
            let heart = document.getElementById("heart");
            heart.classList.toggle("active");
            setTimeout(() => {
                window.location.href = "https://maps.google.com/?q=Hebbal+hatti";
            }, 500);
        }
    </script>
</head>
<body>
    <div class="stars"></div>
    <div class="leaves"></div>
    <div class="banner"></div>
    <div class="invitation-box">
        <h1>With Love & Blessings</h1>
        <p class="quote">"Two hearts, one journey, a lifetime of love begins!"</p>
        <h1>Alma & Roce</h1>
        <p class="date-box">15th April 2025</p>
        <p class="venue">Venue: At our residence, Hebbal Hatti</p>
        <p>Double-tap the heart to see the location</p>
        <span class="heart" id="heart" ondblclick="goToLocation()">❤️</span>
    </div>
</body>
</html>
