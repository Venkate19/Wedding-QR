<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Alma & Roce - Wedding Celebration</title>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Great+Vibes&family=Playfair+Display:wght@500&display=swap');
        body {
            background: linear-gradient(to bottom, #ffd1dc, #ffdde1, #fff5e1);
            text-align: center;
            font-family: 'Playfair Display', serif;
            color: #8b5e3c;
            overflow: hidden;
            position: relative;
        }
        h1 {
            font-size: 3.5rem;
            margin-top: 50px;
            color: #b30000;
            font-family: 'Great Vibes', cursive;
        }
        p {
            font-size: 1.7rem;
            margin: 10px 0;
        }
        .banner {
            background: url('https://your-image-link.com') no-repeat center center/cover;
            height: 250px;
            margin-bottom: 20px;
        }
        .invitation-box {
            background: rgba(255, 255, 255, 0.9);
            padding: 30px;
            border-radius: 20px;
            display: inline-block;
            box-shadow: 0px 0px 15px rgba(0, 0, 0, 0.2);
            width: 70%;
        }
        .date-box {
            font-size: 2.5rem;
            font-weight: bold;
            color: #d4af37;
            background: #fff3cd;
            padding: 10px 25px;
            border-radius: 15px;
            display: inline-block;
            margin-top: 15px;
            font-family: 'Great Vibes', cursive;
        }
        .venue a {
            color: #8b5e3c;
            font-weight: bold;
            text-decoration: none;
            font-size: 1.6rem;
        }
        .venue a:hover {
            text-decoration: underline;
        }
        .stars {
            position: absolute;
            width: 100%;
            height: 100%;
            top: 0;
            left: 0;
            background: url('https://your-stars-image.com') repeat;
            opacity: 0.3;
            z-index: -1;
        }
        .quote {
            font-style: italic;
            font-size: 2rem;
            margin-bottom: 20px;
            color: #b30000;
            font-family: 'Great Vibes', cursive;
        }
        .heart {
            font-size: 3rem;
            cursor: pointer;
            transition: color 0.5s ease-in-out;
            display: inline-block;
            margin-top: 20px;
            color: red;
        }
        .heart.active {
            color: pink;
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
    <div class="banner"></div>
    <div class="invitation-box">
        <h1>With Love & Blessings</h1>
        <p class="quote">"Two hearts, one journey, a lifetime of love begins!"</p>
        <p>Join us in celebrating the joyful union of <b>Alma & Roce</b></p>
        <p class="date-box">15th April 2025</p>
        <p class="venue">Venue: At our residence, Hebbal Hatti - <a href="https://maps.google.com/?q=Hebbal+hatti" target="_blank">View on Map</a></p>
        <p>Double-tap the heart to go to the location</p>
        <span class="heart" id="heart" ondblclick="goToLocation()">❤️</span>
    </div>
</body>
</html>
