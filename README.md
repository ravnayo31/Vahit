# Vahit<!DOCTYPE html><html lang="tr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Senin İçin Aşkım</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            background: linear-gradient(45deg, #ff9a9e, #fad0c4);
            color: white;
            padding: 20px;
        }
        .container {
            max-width: 400px;
            margin: auto;
            background: rgba(255, 255, 255, 0.2);
            padding: 20px;
            border-radius: 15px;
            box-shadow: 0px 0px 10px rgba(0, 0, 0, 0.2);
        }
        .message {
            font-size: 20px;
            margin: 20px 0;
        }
        button {
            background: #ff6b81;
            color: white;
            border: none;
            padding: 10px 20px;
            font-size: 18px;
            border-radius: 10px;
            cursor: pointer;
        }
        button:hover {
            background: #ff4757;
        }
        .yes-btn {
            margin-right: 20px;
        }
        .no-btn {
            position: absolute;
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>Beni Seviyor Musun? ❤️</h1>
        <button class="yes-btn" onclick="yesAnswer()">Evet 💖</button>
        <button class="no-btn" onmouseover="moveNoButton()">Hayır ❌</button>
        <p class="message"></p>
        <audio id="loveMusic" src="your-music-file.mp3" loop></audio>
    </div><script>
    function yesAnswer() {
        document.querySelector(".message").innerText = "Bunu biliyordum aşkım! 💕";
        document.getElementById("loveMusic").play();
    }
    
    function moveNoButton() {
        let button = document.querySelector(".no-btn");
        let x = Math.random() * window.innerWidth * 0.8;
        let y = Math.random() * window.innerHeight * 0.8;
        button.style.left = `${x}px`;
        button.style.top = `${y}px`;
    }
</script>

</body>
</html>
