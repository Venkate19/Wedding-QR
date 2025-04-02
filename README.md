<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Wedding Invitation</title>
    <link href="https://fonts.googleapis.com/css2?family=Great+Vibes&family=Pacifico&family=Roboto:wght@400;700&family=Lobster&family=Sacramento&family=Quicksand&display=swap" rel="stylesheet">
    <style>
        body {
            background: linear-gradient(135deg, #f0f8ff, #d3f4ff);
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
            color: #ffb6c1; /* Lighter pink */
            font-family: 'Quicksand', sans-serif;
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

        .venue {
            font-size: 1.2rem; /* Smaller font size */
            font-weight: bold;
        }

        .venue-container {
            display: flex;
            justify-content: center;
            align-items: center;
            flex-direction: row;
            gap: 10px;
        }

        .venue a {
            font-family: 'Lobster', cursive;
            color: #ff69b4;
            text-decoration: none;
            font-weight: bold;
            padding: 5px 10px;
            border-radius: 5px;
            display: inline-block;
            font-size: 1.5rem;
            animation: blink 1s infinite alternate;
        }

        @keyframes blink {
            0% { opacity: 1; }
            50% { opacity: 0; }
            100% { opacity: 1; }
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

            <div class="venue-container">
                <p class="venue">Venue:</p>
                <a href="https://maps.app.goo.gl/2D7oGVRd4yptLPxg9?g_st=aw">At Our Residence, Hebbal Hatti</a>
            </div>
        </div>
        
        <div class="invitation-box">
            <h2 class="section-title">Reception</h2>
            <p class="celebrate-text">Celebrate the beginning of a new journey with us!</p>
            <p class="date">Date: 1st May 2025</p>
            
            <div class="venue-container">
                <p class="venue">Venue:</p>
                <a href="https://maps.app.goo.gl/Kzf5KGDBpRRDwzky9?g_st=aw">Immaculate Conception Church, Nandagad, Khanapur, Belgaum</a>
            </div>
        </div>
    </div>
</body>
</html>
