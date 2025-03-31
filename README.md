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
        .date {
            font-size: 1.5rem;
            color: #32CD32;
            font-weight: bold;
            margin-bottom: 10px;
            text-shadow: 2px 2px 5px rgba(50, 205, 50, 0.6);
        }
        .venue {
            font-size: 1.5rem;
            color: #FFD700;
            font-weight: bold;
            margin-bottom: 10px;
            text-shadow: 0px 0px 15px rgba(255, 215, 0, 0.8);
        }
        .venue a {
            color: #FFD700;
            text-decoration: none;
            font-weight: bold;
            display: inline-block;
            animation: glow 1.5s infinite alternate;
        }
        @keyframes glow {
            0% { text-shadow: 0 0 10px rgba(255, 215, 0, 0.8); }
            100% { text-shadow: 0 0 20px rgba(255, 215, 0, 1); }
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
        .star {
            position: absolute;
            width: 5px;
            height: 5px;
            background-color: gold;
            border-radius: 50%;
            animation: twinkle 1s ease-in-out infinite;
        }
        @keyframes twinkle {
            0% { opacity: 0.3; transform: scale(1); }
            50% { opacity: 1; transform: scale(1.5); }
            100% { opacity: 0.3; transform: scale(1); }
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
        function createStar() {
            const star = document.createElement("div");
            star.classList.add("star");
            document.body.appendChild(star);
            star.style.left = Math.random() * window.innerWidth + "px";
            star.style.top = Math.random() * window.innerHeight + "px";
            setTimeout(() => star.remove(), 2000);
        }
        setInterval(createStar, 300);
    </script>
</body>
</html>
