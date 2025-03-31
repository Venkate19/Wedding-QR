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
        .moving-car {
            position: absolute;
            width: 60px;
            height: 60px;
            background: url('https://imgur.com/wrlEz7a.png') no-repeat center center/cover;
            bottom: 100px; /* Adjust car position */
            cursor: grab;
            z-index: 1;
        }
        .interactive-venue {
            position: absolute;
            left: 10%;
            top: 10%;
        }
        .interactive-venue2 {
            position: absolute;
            left: 70%;
            top: 10%;
        }
    </style>
</head>
<body>
    <div class="banner"></div>
    <div class="invitation-box">
        <h1>ALMA & ROCE</h1>
        <p class="quote">Two hearts, one journey, a lifetime of love begins!</p>
        <p class="p1">Join us in celebrating the beautiful occasion of Alma and Roce!</p>
        <p class="date">Date: 28th April 2025</p>
        <p class="venue">Venue: <a href="https://maps.app.goo.gl/2D7oGVRd4yptLPxg9?g_st=aw" target="_blank">Our Residence, Hebbal Hatti</a></p>
        <p class="date">Date: 1st May 2025</p>
        <p class="venue">Venue 2: <a href="https://maps.app.goo.gl/Kzf5KGDBpRRDwzky9?g_st=aw" target="_blank">Immaculate Conception Church, Nandagad, Khanapur, Belgaum</a></p>
    </div>

    <div class="moving-car" id="car"></div> <!-- Draggable car -->

    <script>
        let car = document.getElementById('car');
        let isDragging = false;

        // Start dragging the car
        car.addEventListener('mousedown', (e) => {
            isDragging = true;
            car.style.cursor = 'grabbing';
            let offsetX = e.clientX - car.getBoundingClientRect().left;

            // Move car as mouse moves
            const moveCar = (moveEvent) => {
                if (isDragging) {
                    let carPosition = moveEvent.clientX - offsetX;
                    // Restrict the car's position to the screen width
                    carPosition = Math.max(0, Math.min(carPosition, window.innerWidth - car.offsetWidth));
                    car.style.left = carPosition + 'px';
                }
            };

            // Stop dragging when mouse is released
            const stopDrag = () => {
                isDragging = false;
                car.style.cursor = 'grab';

                // If the car reaches the venue positions, redirect to Google Maps
                let carPosition = car.getBoundingClientRect().left + car.offsetWidth / 2;
                if (carPosition >= window.innerWidth * 0.10 && carPosition <= window.innerWidth * 0.20) {
                    window.location.href = 'https://maps.app.goo.gl/2D7oGVRd4yptLPxg9?g_st=aw'; // Venue 1 Google Maps
                } else if (carPosition >= window.innerWidth * 0.70 && carPosition <= window.innerWidth * 0.80) {
                    window.location.href = 'https://maps.app.goo.gl/Kzf5KGDBpRRDwzky9?g_st=aw'; // Venue 2 Google Maps
                }

                // Remove event listeners for mouse move and mouse up after drag ends
                document.removeEventListener('mousemove', moveCar);
                document.removeEventListener('mouseup', stopDrag);
            };

            // Attach the event listeners for moving and stopping the car
            document.addEventListener('mousemove', moveCar);
            document.addEventListener('mouseup', stopDrag);
        });
    </script>
</body>
</html>
