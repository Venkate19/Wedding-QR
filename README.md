<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Wedding Invitation</title>
    <style>
        body {
            background: linear-gradient(135deg, #ff9a9e, #fad0c4, #fad390);
            text-align: center;
            font-family: 'Pacifico', cursive;
            color: #4b0082;
            overflow: hidden;
            position: relative;
        }
        h1 {
            font-size: 4rem;
            margin-top: 30px;
            color: #008080;
            font-weight: bold;
            text-shadow: 3px 3px 8px rgba(0, 0, 0, 0.3);
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
            color: #ff1493;
            margin-top: 30px;
            text-transform: uppercase;
            font-family: 'Lobster', cursive;
        }
        .p1 {
            font-size: 1.5rem;
            margin-top: 20px;
            color: #4b0082;
        }
        .date, .venue {
            font-size: 1.5rem;
            color: #ffd700;
            font-weight: bold;
            margin-bottom: 10px;
        }
        .venue a {
            color: #008080;
            text-decoration: none;
            font-weight: bold;
            position: relative;
            display: inline-block;
            animation: pulse 1.5s infinite;
        }
        .venue a:hover {
            color: #ff4500;
        }
        .click-indicator {
            font-size: 1.2rem;
            color: #ffffff;
            margin-top: 5px;
            font-style: italic;
            animation: blink 1.2s infinite alternate;
        }
        .invitation-box {
            background: rgba(255, 255, 255, 0.8);
            padding: 25px;
            border-radius: 20px;
            display: inline-block;
            box-shadow: 0px 0px 15px rgba(0, 0, 0, 0.3);
        }
        .firework {
            position: absolute;
            width: 20px;
            height: 20px;
            background-color: gold;
            border-radius: 50%;
            animation: explode 1s ease-out infinite;
        }
        @keyframes explode {
            0% { transform: scale(1); opacity: 1; }
            100% { transform: scale(3); opacity: 0; }
        }
        @keyframes pulse {
            0% { transform: scale(1); }
            50% { transform: scale(1.1); }
            100% { transform: scale(1); }
        }
        @keyframes blink {
            0% { opacity: 1; }
            100% { opacity: 0; }
        }
    </style>
</head>
<body>
    <h1>Welcome to Our Special Day!</h1>
    <p class="quote">"Love is a journey best traveled together."</p>
    
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
            setTimeout(() => firework.remove(), 1000);
        }
        setInterval(createFirework, 500);
    </script>
</body>
</html>
