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
            font-family: 'Caveat', cursive;
            color: #8b5e3c;
            overflow: hidden;
            position: relative;
        }
        h1 {
            font-size: 6rem;
            margin-top: 50px;
            color: #ff4b5c;
            text-transform: uppercase;
            font-weight: bolder;
            text-shadow: 2px 2px 10px rgba(0, 0, 0, 0.4);
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
            margin-bottom: 10px;
        }
        .venue a {
            color: #4b9bb3;
            text-decoration: none;
        }
        .venue a:hover {
            color: #ff4b5c;
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
            width: 60px;
            height: 60px;
            background: url('https://i.imgur.com/FxIRkes.png') no-repeat center center/cover;
            bottom: 10px; /* Keep the car closer to the bottom */
            animation: moveCar 5s infinite;
            z-index: 1;
        }
        .smoke {
            position: absolute;
            background: url('https://your-smoke-effect-link.com') no-repeat center center;
            width: 100px;
            height: 50px;
            top: 10px;
            left: 60px;
            animation: smokeEffect 5s infinite;
            z-index: 0;
        }
        .stars {
            position: absolute;
            top: 10px;
            left: 0;
            width: 100%;
            height: 100%;
            background: url('https://your-stars-link.com') repeat;
            z-index: -1;
            opacity: 0.5;
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
        .interactive-venue {
            position: absolute;
            top: 300px; /* Adjust to match venue's position on the screen */
            left: 50%;
            transform: translateX(-50%);
            padding: 10px;
            background-color: rgba(255, 255, 255, 0.8);
            border-radius: 10px;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.3);
            cursor: pointer;
        }
        .interactive-venue:hover {
            background-color: rgba(255, 255, 255, 0.9);
        }
    </style>
</head>
<body>
    <div class="stars"></div>
    <div class="banner"></div>
    <div class="invitation-box">
        <h1>ALMA & ROCE</h1>
        <p class="quote">Two hearts, one journey, a lifetime of love begins!</p>
        <div class="moving-car" id="movingCar"></div>
        <div class="smoke"></div>
        <p class="p1">Join us in celebrating the beautiful occasion of Alma and Roce!</p>
        <p class="date">Date: 28th April 2025</p>
        <p class="venue">Venue: <a href="https://maps.app.goo.gl/2D7oGVRd4yptLPxg9?g_st=aw" target="_blank">Our Residence, Hebbal Hatti</a></p>
        <p class="date">Date: 1st May 2025</p>
        <p class="venue">Venue 2: <a href="https://maps.app.goo.gl/Kzf5KGDBpRRDwzky9?g_st=aw" target="_blank">Immaculate Conception Church, Nandagad, Khanapur, Belgaum</a></p>
        <p class="venue">Reception: IC Church Campus</p>
        <p class="heart" onclick="location.href='https://maps.app.goo.gl/Kzf5KGDBpRRDwzky9?g_st=aw'">❤️</p>
    </div>

    <div class="interactive-venue" onclick="redirectToVenue()">
        Click here to visit the venue on Google Maps
    </div>

    <script>
        let car = document.getElementById('movingCar');
        let carPosition = 0; // Starting position of the car
        let carSpeed = 2; // Speed of the car movement
        let venuePosition = 50; // Position where the car will "reach" the venue

        // Function to move the car towards the venue
        function moveCar() {
            if (carPosition < venuePosition) {
                carPosition += carSpeed; // Move the car forward
                car.style.left = carPosition + '%'; // Update car's position
                requestAnimationFrame(moveCar); // Continue the animation
            } else {
                // When car reaches the venue, redirect to Google Maps
                redirectToVenue();
            }
        }

        // Function to redirect to the Google Maps venue link
        function redirectToVenue() {
            window.location.href = 'https://maps.app.goo.gl/2D7oGVRd4yptLPxg9?g_st=aw'; // Venue 1 map link
        }

        moveCar(); // Start moving the car when the page loads
    </script>
</body>
</html>
