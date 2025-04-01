<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Wedding Invitation</title>
    <link href="https://fonts.googleapis.com/css2?family=Great+Vibes&family=Pacifico&family=Roboto:wght@400;700&family=Lobster&family=Sacramento&family=Quicksand&display=swap" rel="stylesheet">
    <style>
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
            color: #7a5c8d; /* New color for Motes Weds Seema */
            font-family: 'Quicksand', sans-serif; /* Modern stylish font for Motes Weds Seema */
            font-weight: bold;
            text-shadow: 3px 3px 8px rgba(122, 92, 141, 0.6);
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
            font-family: 'Cinzel', serif;
        }

        .p1, .date, .venue {
            font-size: 1.5rem;
            margin: 15px 0;
            font-family: 'Roboto', sans-serif;
        }

        .join-us, .celebrate-text {
            font-family: 'Lobster', cursive; /* Stylish font for Join Us and Celebrate */
            font-size: 1.8rem; /* Smaller size for balance */
            color: #4e77a0; /* A cool, calming blue */
            letter-spacing: 1px;
            text-transform: none; /* Changed to normal case */
            margin: 10px 0;
        }

        .date {
            font-size: 1.8rem;
            font-family: 'Roboto', sans-serif;
            color: #d2691e;
            font-weight: bold;
        }

        .venue a {
            font-family: 'Roboto', sans-serif;
            color: #2e8b57; /* Stylish green for venue link */
            text-decoration: none;
            font-weight: bold;
            padding: 5px 10px;
            border-radius: 5px;
            display: inline-block;
            animation: blowing-out 1s ease-in-out infinite;
        }

        @keyframes blowing-out {
            0% { transform: scale(1); }
            50% { transform: scale(1.1); }
            100% { transform: scale(1); }
        }

        .click-indicator {
            font-size: 1rem;
            color: #ff4500;
            font-weight: bold;
            margin-top: 5px;
        }

        .invitation-box {
            background: rgba(255, 255, 255, 0.8);
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
            <p class="join-us">Join us in celebrating the union of Alma and Roce!</p>
            <p class="date">Date: 28th April 2025</p>
            <p class="venue">Venue: <a href="https://maps.app.goo.gl/2D7oGVRd4yptLPxg9?g_st=aw">At Our Residence, Hebbal Hatti</a></p>
            <p class="click-indicator">(Click venue for location)</p>
        </div>
        
        <div class="invitation-box">
            <h2 class="section-title">Reception</h2>
            <p class="celebrate-text">Celebrate the beginning of a new journey with us!</p>
            <p class="date">Date: 1st May 2025</p>
            <p class="venue">Venue: <a href="https://maps.app.goo.gl/Kzf5KGDBpRRDwzky9?g_st=aw">Immaculate Conception Church, Nandagad, Khanapur, Belgaum</a></p>
            <p class="click-indicator">(Click venue for location)</p>
        </div>
    </div>
</body>
</html>
