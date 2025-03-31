<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Wedding Invitation</title>
    <style>
        body {
            background: linear-gradient(135deg, #ffb6c1, #dda0dd, #87cefa);
            text-align: center;
            font-family: 'Great Vibes', cursive;
            color: #4b0082;
            overflow: hidden;
            position: relative;
        }
        h1 {
            font-size: 4rem;
            margin-top: 30px;
            color: #ff4500;
            font-weight: bold;
            text-shadow: 3px 3px 8px rgba(0, 0, 0, 0.3);
            font-family: 'Satisfy', cursive;
        }
        .quote {
            font-size: 2rem;
            color: #ffffff;
            margin-bottom: 15px;
            font-style: italic;
            font-family: 'Dancing Script', cursive;
        }
        .section-title {
            font-size: 3rem;
            color: #8a2be2;
            margin-top: 30px;
            text-transform: uppercase;
            font-family: 'Lobster', cursive;
        }
        .p1 {
            font-size: 1.8rem;
            margin-top: 20px;
            color: #5f9ea0;
            font-family: 'Courgette', cursive;
        }
        .date {
            font-size: 1.8rem;
            color: #ff8c00;
            font-weight: bold;
            margin-bottom: 10px;
            text-shadow: 2px 2px 5px rgba(255, 140, 0, 0.6);
            font-family: 'Cinzel Decorative', cursive;
        }
        .venue {
            font-size: 1.8rem;
            color: #4682b4;
            font-weight: bold;
            margin-bottom: 10px;
            text-shadow: 0px 0px 15px rgba(70, 130, 180, 0.8);
            font-family: 'Playfair Display', serif;
        }
        .venue a {
            color: #4682b4;
            text-decoration: none;
            font-weight: bold;
            display: inline-block;
            animation: glow 1.5s infinite alternate;
        }
        @keyframes glow {
            0% { text-shadow: 0 0 10px rgba(70, 130, 180, 0.8); }
            100% { text-shadow: 0 0 20px rgba(70, 130, 180, 1); }
        }
        .click-indicator {
            font-size: 1.5rem;
            color: #ffffff;
            margin-top: 5px;
            font-style: italic;
            animation: blink 1.2s infinite alternate;
        }
        .invitation-box {
            background: rgba(255, 255, 255, 0.9);
            padding: 25px;
            border-radius: 20px;
            display: inline-block;
            box-shadow: 0px 0px 15px rgba(0, 0, 0, 0.3);
        }
        .firework {
            position: absolute;
            width: 20px;
            height: 20px;
            background-color: transparent;
            border-radius: 50%;
            box-shadow: 0 0 15px 5px rgba(255, 223, 0, 1);
            animation: explode 0.8s ease-out forwards;
        }
        @keyframes explode {
            0% { transform: scale(1); opacity: 1; }
            100% { transform: scale(3); opacity: 0; }
        }
        @keyframes blink {
            0% { opacity: 1; }
            100% { opacity: 0; }
        }
    </style>
</head>
<body>
    <h1>Welcome to Our Grand Celebration!</h1>
    <p class="quote">"A journey of love begins with a spark."</p>
    
    <div class="invitation-box">
        <h2 class="section-title">Alma & Roce</h2>
        <p class="p1">Join us in celebrating the union of Alma and Roce!</p>
        <p class="date">Date: 28th April 2025</p>
        <p class="venue">Venue: <a href="https://maps.app.goo.gl/2D7oGVRd4yptLPxg9?g_st=aw" target="_blank">Our Residence, Hebbal Hatti</a></p>
        <p class="click-indicator">(Click venue link for directions!)</p>
    </div>
    
    <div class="invitation-box" style="margin-top: 30px;">
        <h2 class="section-title">Reception</h2>
        <p class="p1">Celebrate the beginning of a new journey with us!</p>
        <p class="date">Date: 1st May 2025</p>
        <p class="venue">Venue: <a href="https://maps.app.goo.gl/Kzf5KGDBpRRDwzky9?g_st=aw" target="_blank">Immaculate Conception Church, Nandagad, Khanapur, Belgaum</a></p>
        <p class="click-indicator">(Click venue link for directions!)</p>
    </div>
    
    <script>
        function createFirework() {
            const firework = document.createElement("div");
            firework.classList.add("firework");
            document.body.appendChild(firework);
            firework.style.left = Math.random() * window.innerWidth + "px";
            firework.style.top = Math.random() * window.innerHeight + "px";
            setTimeout(() => firework.remove(), 800);
        }
        setInterval(createFirework, 500);
    </script>
</body>
</html>
