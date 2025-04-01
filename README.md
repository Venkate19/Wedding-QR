<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Wedding Invitation</title>
    <style>
        @keyframes highlight {
            0% { background-color: yellow; }
            100% { background-color: transparent; }
        }
        body {
            background: linear-gradient(135deg, #fdfcfb, #e2d1c3);
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
            font-size: 2.5rem;
            color: #ff8c00;
            font-weight: bold;
            text-shadow: 3px 3px 8px rgba(255, 165, 0, 0.6);
            font-family: 'Satisfy', cursive;
        }
        .quote {
            font-size: 1.5rem;
            color: #6a5acd;
            font-style: italic;
            font-family: 'Dancing Script', cursive;
        }
        .section-title {
            font-size: 2rem;
            color: #8a2be2;
            text-transform: uppercase;
            font-family: 'Lobster', cursive;
        }
        .p1, .date, .venue {
            font-size: 1.2rem;
            margin: 15px 0;
        }
        .venue a {
            color: #4682b4;
            text-decoration: none;
            font-weight: bold;
            animation: highlight 1.5s infinite alternate;
            padding: 2px 5px;
            border-radius: 5px;
        }
        .click-indicator {
            font-size: 1rem;
            color: #ff4500;
            font-weight: bold;
            margin-top: 5px;
        }
        .invitation-box {
            background: white;
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0px 4px 10px rgba(0, 0, 0, 0.1);
            margin-bottom: 20px;
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>Welcome to Our Grand Celebration!</h1>
        <p class="quote">"A journey of love begins with a spark."</p>
        
        <div class="invitation-box">
            <h2 class="section-title">Alma & Roce</h2>
            <p class="p1">Join us in celebrating the union of Alma and Roce!</p>
            <p class="date">Date: 28th April 2025</p>
            <p class="venue">Venue: <a href="https://maps.app.goo.gl/2D7oGVRd4yptLPxg9?g_st=aw" target="_blank">Our Residence, Hebbal Hatti</a></p>
            <p class="click-indicator">(Click venue for location)</p>
        </div>
        
        <div class="invitation-box">
            <h2 class="section-title">Reception</h2>
            <p class="p1">Celebrate the beginning of a new journey with us!</p>
            <p class="date">Date: 1st May 2025</p>
            <p class="venue">Venue: <a href="https://maps.app.goo.gl/Kzf5KGDBpRRDwzky9?g_st=aw" target="_blank">Immaculate Conception Church, Nandagad, Khanapur, Belgaum</a></p>
            <p class="click-indicator">(Click venue for location)</p>
        </div>
    </div>
</body>
</html>
