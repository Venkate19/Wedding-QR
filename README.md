<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Wedding Invitation</title>
    <style>
        body {
            background: linear-gradient(to bottom, #f5e5b7, #f5efe7);
            text-align: center;
            font-family: 'Dancing Script', cursive;
            color: #8b5e3c;
            overflow: hidden;
        }
        h1 {
            font-size: 5rem; /* Increased font size */
            margin-top: 50px;
            color: #ff4b5c;
            text-transform: uppercase;
            font-weight: bolder; /* Increased font weight for more emphasis */
            text-shadow: 2px 2px 5px rgba(0, 0, 0, 0.3); /* Added text shadow for better contrast */
        }
        .quote {
            font-size: 1.8rem;
            color: #d4af37;
            margin-bottom: 20px;
            font-style: italic;
        }
        .p1 {
            font-size: 1.5rem;
            margin-top: 20px;
            color: #8b5e3c;
        }
        .date, .venue {
            font-size: 1.2rem;
            color: #d4af37;
            font-weight: bold;
        }
        .banner {
            background: url('https://your-banner-link.com') no-repeat center center/cover;
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
        .decorations {
            position: absolute;
            width: 100%;
            top: 0;
            left: 0;
            pointer-events: none;
        }
        .heart {
            font-size: 2.5rem;
            color: #ff4b5c;
            cursor: pointer;
        }
        .heart:hover {
            color: #d44b56;
        }
        .moving-car {
            position: absolute;
            width: 50px;
            height: 50px;
            background: url('https://your-car-link.com') no-repeat center center/cover;
            animation: moveCar 5s infinite;
        }
        .smoke {
            position: absolute;
            background: url('https://your-smoke-effect-link.com') no-repeat center center;
            width: 100px;
            height: 50px;
            top: 10px;
            left: 60px;
            animation: smokeEffect 5s infinite;
        }
        @keyframes moveCar {
            0% { left: 0; }
            50% { left: 50%; }
            100% { left: 100%; }
        }
        @keyframes smokeEffect {
            0% { left: 60px; }
            100% { left: 110px; }
        }
    </style>
    <link href="https://fonts.googleapis.com/css2?family=Dancing+Script:wght@600&display=swap" rel="stylesheet">
</head>
<body>
    <div class="banner"></div>
    <div class="invitation-box">
        <h1>ALMA & ROCE</h1>
        <p class="quote">Two hearts, one journey, a lifetime of love begins!</p>
        <div class="moving-car"></div>
        <div class="smoke"></div>
        <p class="p1">Join us in celebrating the beautiful occasion of Alma and Roce!</p>
        <p class="date">Date: 15th April 2025</p>
        <p class="venue">Venue: <a href="https://maps.app.goo.gl/2D7oGVRd4yptLPxg9?g_st=aw" target="_blank">Our Residence, Hebbal Hatti</a></p>
        <p class="venue">Venue 2: <a href="https://maps.app.goo.gl/Kzf5KGDBpRRDwzky9?g_st=aw" target="_blank">Immaculate Conception Church, Nandagad, Khanapur, Belgaum</a></p>
        <p class="venue">Reception: IC Church Campus</p>
        <p class="heart" onclick="location.href='https://maps.app.goo.gl/Kzf5KGDBpRRDwzky9?g_st=aw'">❤️</p>
    </div>
</body>
</html>
