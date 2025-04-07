# 2301030400052_Assignment-_2
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Travel Planner</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <div id="login-page" class="page active">
        <div class="container">
            <img src="logo.png" class="logo" alt="Logo">
            <input type="text" placeholder="NAME" class="input-field">
            <input type="password" placeholder="PASSWORD" class="input-field">
            <button class="btn" onclick="showPage('home-page')">START</button>
        </div>
    </div>

    <div id="home-page" class="page">
        <div class="container">
            <img src="logo.png" class="logo" alt="Logo">
            <h2 class="title">LET'S <span class="highlight">TRAVEL</span></h2>
            <div class="btn-container">
                <button class="btn" onclick="showPage('trip-page')">VIEW TRIP</button>
                <button class="btn" onclick="showPage('login-page')">SIGN OUT</button>
            </div>
        </div>
    </div>

    <div id="trip-page" class="page">
        <h1>Trip <span class="highlight">Highlights</span></h1>
        <div class="trip-container">
            <div class="trip-item"><img src="cologne.jpg" alt="Cologne"><p>Cologne<br>1 Jan - 5 Jan</p></div>
            <div class="trip-item"><img src="heidelberg.jpg" alt="Heidelberg"><p>Heidelberg<br>6 Jan - 10 Jan</p></div>
            <div class="trip-item"><img src="nuremberg.jpg" alt="Nuremberg"><p>Nuremberg<br>11 Jan - 15 Jan</p></div>
            <div class="trip-item"><img src="munich.jpg" alt="Munich"><p>Munich<br>16 Jan - 20 Jan</p></div>
            <div class="trip-item"><img src="frankfurt.jpg" alt="Frankfurt"><p>Frankfurt<br>21 Jan - 25 Jan</p></div>
        </div>
        <button class="btn" onclick="showPage('overview-page')">OVERVIEW</button>
    </div>

    <div id="overview-page" class="page">
        <h2 class="title">Overview</h2>
        <img src="cologne.jpg" class="main-image" alt="Cologne">
        <div class="trip-container">
            <div class="trip-item"><img src="cologne.jpg" alt="Cologne"><p>Cologne<br>1 Jan - 5 Jan</p></div>
            <div class="trip-item"><img src="heidelberg.jpg" alt="Heidelberg"><p>Heidelberg<br>6 Jan - 10 Jan</p></div>
            <div class="trip-item"><img src="nuremberg.jpg" alt="Nuremberg"><p>Nuremberg<br>11 Jan - 15 Jan</p></div>
            <div class="trip-item"><img src="munich.jpg" alt="Munich"><p>Munich<br>16 Jan - 20 Jan</p></div>
            <div class="trip-item"><img src="frankfurt.jpg" alt="Frankfurt"><p>Frankfurt<br>21 Jan - 25 Jan</p></div>
        </div>
        <button class="btn" onclick="showPage('trip-page')">BACK</button>
    </div>

    <script>
        function showPage(pageId) {
            document.querySelectorAll('.page').forEach(page => page.classList.remove('active'));
            document.getElementById(pageId).classList.add('active');
        }
    </script>
</body>
</html>
