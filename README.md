<!DOCTYPE html>
<html lang="ru">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Jumanys — YouTube, Twitch & Telegram</title>
  <style>
    @import url('https://fonts.googleapis.com/css2?family=Orbitron:wght@400;700&display=swap');

    body {
      margin: 0;
      font-family: 'Orbitron', sans-serif;
      background: linear-gradient(135deg, #18181b, #2c2c34);
      color: #efeff1;
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      height: 100vh;
      text-align: center;
      overflow: hidden;
    }

    h1 {
      font-size: 3rem;
      margin-bottom: 0.5rem;
      background: linear-gradient(90deg, #9146ff, #ff0000, #229ED9);
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
      animation: gradientShift 5s infinite linear;
    }

    p {
      font-size: 1.3rem;
      margin-bottom: 2rem;
      color: #adadb8;
    }

    @keyframes gradientShift {
      0% {background-position: 0%}
      100% {background-position: 200%}
    }

    .links {
      display: flex;
      gap: 1.5rem;
    }

    .links a {
      padding: 1rem 2rem;
      border-radius: 0.75rem;
      text-decoration: none;
      font-weight: bold;
      color: white;
      box-shadow: 0 0 10px rgba(0,0,0,0.3);
      transition: transform 0.2s, box-shadow 0.2s;
    }

    .links a:hover {
      transform: scale(1.1);
      box-shadow: 0 0 20px rgba(255,255,255,0.5);
    }

    .youtube { background-color: #ff0000; }
    .twitch { background-color: #9146ff; }
    .telegram { background-color: #229ED9; }

    .background-glow {
      position: absolute;
      top: -50%;
      left: -50%;
      width: 200%;
      height: 200%;
      background: radial-gradient(circle, rgba(145,70,255,0.2), transparent 70%),
                  radial-gradient(circle, rgba(255,0,0,0.2), transparent 70%),
                  radial-gradient(circle, rgba(34,158,217,0.2), transparent 70%);
      animation: rotateGlow 20s linear infinite;
      z-index: 0;
    }

    @keyframes rotateGlow {
      from { transform: rotate(0deg); }
      to { transform: rotate(360deg); }
    }

    body > * { position: relative; z-index: 1; }

  </style>
</head>
<body>
  <div class="background-glow"></div>
  <h1>Jumanys</h1>
  <p>Добро пожаловать на страницы моих каналов YouTube, Twitch и Telegram</p>
  <div class="links">
    <a class="youtube" href="https://www.youtube.com/@jumanygt9096" target="_blank">YouTube</a>
    <a class="twitch" href="https://www.twitch.tv/jumanys" target="_blank">Twitch</a>
    <a class="telegram" href="https://t.me/Jumanys777" target="_blank">Telegram</a>
  </div>
</body>
</html>

