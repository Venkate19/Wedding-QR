<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Wedding Invitation</title>
    <link href="https://fonts.googleapis.com/css2?family=Cinzel:wght@700&family=Great+Vibes&family=Pacifico&family=Roboto:wght@400;700&display=swap" rel="stylesheet">
    <style>
        @keyframes star-glow {
            0% { text-shadow: 0 0 5px #ffd700, 0 0 10px #ffa500; transform: scale(1); }
            50% { text-shadow: 0 0 15px #ffd700, 0 0 30px #ffa500; transform: scale(1.1); }
            100% { text-shadow: 0 0 5px #ffd700, 0 0 10px #ffa500; transform: scale(1); }
        }

        body {
            background: linear-gradient(135deg, #f0f8ff, #d3f4ff); /* Light color gradient background */
            text-align: center;
            font-family: 'Great Vibes', cursive;
            color: #4b0082;
            margin: 0;
            padding: 0;
        }

        .container {
            max-width: 100%;
            padding: 20px;
            box-sizing: border-box;
        }

        h1 {
            font-size: 4rem;
            color: #ff6347;
            font-weight: bold;
            text-shadow: 3px 3px 8px rgba(255, 99, 71, 0.6);
            font-family: 'Pacifico', cursive; /* Elegant handwriting font for MOTES WEDS SEEMA */
        }

        .quote {
            font-size: 1.8rem;
            color: #6a5acd;
            font-style: italic;
            font-family: 'Dancing Script', cursive;
            line-height: 1.5;
            padding: 10px;
        }

        .section-title {
            font-size: 2.5rem;
            color: #8a2be2;
            text-transform: uppercase;
            font-family: 'Cinzel', serif; /* Stylish font for section titles */
        }

        .p1, .date, .venue {
            font-size: 1.5rem;
            margin: 15px 0;
            font-family: 'Roboto', sans-serif; /* Modern font for text */
        }

        .p1-celebrate {
            font-family: 'Roboto', sans-serif;
            font-size: 1.8rem;
            color: #d2691e;
            font-weight: bold;
        }

        .venue a {
            color: #2e8b57; /* Stylish green for venue link */
            text-decoration: none;
            font-weight: bold;
            padding: 5px 10px;
            border-radius: 5px;
            display: inline-block;
            animation: star-glow 1.5s infinite alternate;
            font-family: 'Roboto', sans-serif;
        }

        .click-indicator {
            font-size: 1rem;
            color: #ff4500;
            font-weight: bold;
            margin-top: 5px;
        }

        .invitation-box {
            background: rgba(255, 255, 255, 0.8); /* Semi-transparent white background for content boxes */
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0px 4px 10px rgba(0, 0, 0, 0.1);
            margin-bottom: 20px;
        }

    </style>
</head>
<body>
    <div class="container">
        <h1>MOTES WEDS SEEMA</h1>
        <p class="quote">"A journey of love begins with a spark."</p>
        
        <div class="invitation-box">
            <h2 class="section-title">Alma & Roce</h2>
            <p class="p1">Join us in celebrating the union of Alma and Roce!</p>
            <p class="date">Date: 28th April 2025</p>
            <p class="venue">Venue: <a href="https://maps.app.goo.gl/2D7oGVRd4yptLPxg9?g_st=aw">At Our Residence, Hebbal Hatti</a></p>
            <p class="click-indicator">(Click venue for location)</p>
        </div>
        
        <div class="invitation-box">
            <h2 class="section-title">Reception</h2>
            <p class="p1-celebrate">Celebrate the beginning of a new journey with us!</p>
            <p class="date">Date: 1st May 2025</p>
            <p class="venue">Venue: <a href="https://maps.app.goo.gl/Kzf5KGDBpRRDwzky9?g_st=aw">Immaculate Conception Church, Nandagad, Khanapur, Belgaum</a></p>
            <p class="click-indicator">(Click venue for location)</p>
        </div>
    </div>
</body>
</html>
