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
            color: #ff8c00;
            font-weight: bold;
            text-shadow: 3px 3px 8px rgba(255, 165, 0, 0.6);
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
        .hanging-bells {
            position: absolute;
            top: 0;
            left: 50%;
            transform: translateX(-50%);
            width: 100px;
            height: 100px;
            background: url('https://your-hanging-bells-image.png') no-repeat center center/contain;
        }
        .flower-entrance {
            position: absolute;
            top: 0;
            left: 50%;
            transform: translateX(-50%);
            width: 100%;
            height: 200px;
            background: url('https://your-flower-entrance-image.png') no-repeat center center/contain;
        }
        .falling-stars {
            position: absolute;
            width: 5px;
            height: 5px;
            background: gold;
            border-radius: 50%;
            opacity: 0.8;
            animation: fall 3s linear infinite;
        }
        @keyframes fall {
            0% { transform: translateY(-50px); opacity: 1; }
            100% { transform: translateY(100vh); opacity: 0; }
        }
    </style>
</head>
<body>
    <div class="flower-entrance"></div>
    <h1>Welcome to Our Grand Celebration!</h1>
    <p class="quote">"A journey of love begins with a spark."</p>
    
    <div class="hanging-bells"></div>
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
            star.classList.add("falling-stars");
            document.body.appendChild(star);
            star.style.left = Math.random() * window.innerWidth + "px";
            star.style.animationDuration = Math.random() * 3 + 2 + "s";
            setTimeout(() => star.remove(), 3000);
        }
        setInterval(createStar, 300);
    </script>
</body>
</html>
