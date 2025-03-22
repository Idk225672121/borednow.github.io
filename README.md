<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Unblocked Games</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            margin: 0;
            padding: 0;
            background-image: url('https://images.unsplash.com/photo-1534796636912-3b95b3ab5986?ixlib=rb-1.2.1&auto=format&fit=crop&w=1950&q=80'); /* Cool gaming background */
            background-size: cover;
            background-position: center;
            background-attachment: fixed;
            color: white;
        }
        h1 {
            font-size: 3rem;
            margin: 20px 0;
            text-shadow: 2px 2px 5px rgba(0, 0, 0, 0.5);
        }
        .game-container {
            display: flex;
            justify-content: center;
            flex-wrap: wrap;
            gap: 20px;
            padding: 20px;
        }
        .game {
            background: rgba(0, 0, 0, 0.7); /* Semi-transparent black background */
            padding: 20px;
            border-radius: 15px;
            box-shadow: 0 0 15px rgba(0, 0, 0, 0.5);
            width: 400px;
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }
        .game:hover {
            transform: scale(1.05);
            box-shadow: 0 0 20px rgba(0, 0, 0, 0.8);
        }
        iframe {
            width: 100%;
            height: 300px;
            border: none;
            border-radius: 10px;
        }
        .fullscreen-btn {
            display: block;
            margin: 10px auto;
            padding: 10px 20px;
            background-color: #007bff;
            color: white;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            font-size: 1rem;
            transition: background-color 0.3s ease;
        }
        .fullscreen-btn:hover {
            background-color: #0056b3;
        }
    </style>
</head>
<body>
    <h1>Welcome to Unblocked Games</h1>
    <div class="game-container">
        <div class="game">
            <h2>Google Dino</h2>
            <iframe id="game1" src="https://chromedino.com/m/" title="Google Dino"></iframe>
            <button class="fullscreen-btn" onclick="toggleFullScreen('game1')">Full Screen</button>
        </div>
        <div class="game">
            <h2>1v1.LOL</h2>
            <iframe id="game2" src="https://1v1.lol/" title="1v1 LOL"></iframe>
            <button class="fullscreen-btn" onclick="toggleFullScreen('game2')">Full Screen</button>
        </div>
        <div class="game">
            <h2>Super Mario</h2>
            <iframe id="game3" src="https://supermarioemulator.com/mario.php" title="Super Mario"></iframe>
            <button class="fullscreen-btn" onclick="toggleFullScreen('game3')">Full Screen</button>
        </div>
        <div class="game">
            <h2>Slow Roads</h2>
            <iframe id="game4" src="https://slowroads.io/" title="Slow Roads"></iframe>
            <button class="fullscreen-btn" onclick="toggleFullScreen('game4')">Full Screen</button>
        </div>
        <div class="game">
            <h2>Krunker.io</h2>
            <iframe id="game5" src="https://krunker.io/" title="Krunker.io"></iframe>
            <button class="fullscreen-btn" onclick="toggleFullScreen('game5')">Full Screen</button>
        </div>
    </div>

    <script>
        // Full-Screen Function
        function toggleFullScreen(elementId) {
            const element = document.getElementById(elementId);
            if (element.requestFullscreen) {
                element.requestFullscreen();
            } else if (element.mozRequestFullScreen) {
                element.mozRequestFullScreen();
            } else if (element.webkitRequestFullscreen) {
                element.webkitRequestFullscreen();
            } else if (element.msRequestFullscreen) {
                element.msRequestFullscreen();
            }
        }
    </script>
</body>
</html>
