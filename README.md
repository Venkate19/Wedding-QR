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
            color: #8B008B;
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

        .invitation-box {
            background: rgba(255, 255, 255, 0.8);
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0px 4px 10px rgba(0, 0, 0, 0.1);
            margin-bottom: 20px;
            width: 100%; /* Ensure it takes full width */
            box-sizing: border-box;
            border: 2px solid #8a2be2;
        }

        .p1, .date, .venue {
            font-size: 1.5rem;
            margin: 15px 0;
            font-family: 'Roboto', sans-serif;
        }

        .join-us, .celebrate-text {
            font-family: 'Lobster', cursive;
            font-size: 1.8rem;
            color: #4e77a0;
            letter-spacing: 1px;
            text-transform: none;
            margin: 10px 0;
        }

        .date {
            font-size: 1.8rem;
            font-family: 'Roboto', sans-serif;
            color: #a0522d;
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
            font-family: cursive;
            color: #ff69b4;
            text-decoration: none;
            font-weight: bold;
            padding: 8px 15px;
            border-radius: 8px;
            border: 2px solid #ff69b4;
            display: inline-block;
            animation: blowing-out 1s ease-in-out infinite;
            font-size: 1.5rem;
            background: rgba(255, 255, 255, 0.8);
            box-shadow: 2px 2px 10px rgba(0, 0, 0, 0.2);
        }

        @keyframes blowing-out {
            0% { transform: scale(1); }
            50% { transform: scale(1.1); }
            100% { transform: scale(1); }
        }

        .hand-container {
            display: flex;
            justify-content: center;
            align-items: center;
            flex-direction: column;
            margin-top: 20px;
        }

        .hand-emoji {
            font-size: 3rem;
            animation: handMove 1s ease-in-out infinite, bounce 0.5s ease-in-out infinite alternate;
            margin-top: 5px;
        }

        @keyframes handMove {
            0% {
                transform: translateY(-10px);
            }
            50% {
                transform: translateY(10px);
            }
            100% {
                transform: translateY(-10px);
            }
        }

        @keyframes bounce {
            0% {
                transform: translateY(0);
            }
            50% {
                transform: translateY(-10px);
            }
            100% {
                transform: translateY(0);
            }
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
            
            <div class="hand-container">
                <p>Find us here:</p>
                <div class="hand-emoji">👇</div>
            </div>

            <div class="venue-container">
                <p class="venue">Venue:</p>
                <a href="https://maps.app.goo.gl/2D7oGVRd4yptLPxg9?g_st=aw">At Our Residence, Hebbal Hatti</a>
            </div>
        </div>
        
        <div class="invitation-box">
            <h2 class="section-title">Reception</h2>
            <p class="celebrate-text">Celebrate the beginning of a new journey with us!</p>
            <p class="date">Date: 1st May 2025</p>
            
            <div class="hand-container">
                <p>Find us here:</p>
                <div class="hand-emoji">👇</div>
            </div>

            <div class="venue-container">
                <p class="venue">Venue:</p>
                <a href="https://maps.app.goo.gl/Kzf5KGDBpRRDwzky9?g_st=aw">Immaculate Conception Church, Nandagad, Khanapur, Belgaum</a>
            </div>
        </div>
    </div>
</body>
</html>
