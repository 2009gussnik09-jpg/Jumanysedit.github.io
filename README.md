<!DOCTYPE html>

<html lang="ru">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Jumanys — YouTube, Twitch & Telegram</title>
  <link href="https://fonts.googleapis.com/css2?family=Orbitron:wght@400;700&family=Roboto:wght@400;500&display=swap" rel="stylesheet">
  <style>
    body {
      margin: 0;
      font-family: 'Roboto', sans-serif;
      background: linear-gradient(135deg, #18181b, #2c2c34);
      color: #efeff1;
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      min-height: 100vh;
      text-align: center;
      overflow: hidden;
    }

```
.background-glow {
  position: absolute;
  top: -50%;
  left: -50%;
  width: 200%;
  height: 200%;
  background: radial-gradient(circle, rgba(145,70,255,0.2), transparent 70%),
              radial-gradient(circle, rgba(255,0,0,0.2), transparent 70%),
              radial-gradient(circle, rgba(34,158,217,0.2), transparent 70%);
  animation: rotateGlow 25s linear infinite;
  z-index: 0;
}

@keyframes rotateGlow {
  from { transform: rotate(0deg); }
  to { transform: rotate(360deg); }
}

h1 {
  font-family: 'Orbitron', sans-serif;
  font-size: 3rem;
  margin: 1rem 0;
  background: linear-gradient(90deg, #9146ff, #ff0000, #229ED9);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  animation: gradientShift 5s infinite linear;
}

@keyframes gradientShift {
  0% {background-position: 0%}
  100% {background-position: 200%}
}

p {
  font-size: 1.2rem;
  margin-bottom: 2rem;
  color: #adadb8;
  opacity: 0;
  animation: fadeIn 2s forwards;
}

@keyframes fadeIn {
  to { opacity: 1; }
}

.cards {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  gap: 2rem;
  z-index: 1;
}

.card {
  background: #22222a;
  border-radius: 15px;
  padding: 2rem 3rem;
  width: 200px;
  text-align: center;
  box-shadow: 0 0 20px rgba(0,0,0,0.5);
  transition: transform 0.3s, box-shadow 0.3s;
  cursor: pointer;
}

.card:hover {
  transform: translateY(-10px);
  box-shadow: 0 0 30px rgba(255,255,255,0.6);
}

.card h2 {
  margin: 1rem 0;
  font-size: 1.5rem;
  background: linear-gradient(90deg, #9146ff, #ff0000, #229ED9);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
}

.card a {
  display: inline-block;
  margin-top: 1rem;
  padding: 0.5rem 1rem;
  border-radius: 8px;
  text-decoration: none;
  color: white;
  background-color: inherit;
  transition: background-color 0.3s;
}

.card.youtube a { background-color: #ff0000; }
.card.youtube a:hover { background-color: #cc0000; }

.card.twitch a { background-color: #9146ff; }
.card.twitch a:hover { background-color: #772ce8; }

.card.telegram a { background-color: #229ED9; }
.card.telegram a:hover { background-color: #1c8abf; }
```

  </style>
</head>
<body>
  <div class="background-glow"></div>
  <h1>Jumanys</h1>
  <p>Добро пожаловать на страницы моих каналов!</p>
  <div class="cards">
    <div class="card youtube">
      <h2>YouTube</h2>
      <a href="https://www.youtube.com/@jumanygt9096" target="_blank">Перейти</a>
    </div>
    <div class="card twitch">
      <h2>Twitch</h2>
      <a href="https://www.twitch.tv/jumanys" target="_blank">Перейти</a>
    </div>
    <div class="card telegram">
      <h2>Telegram</h2>
      <a href="https://t.me/Jumanys777" target="_blank">Перейти</a>
    </div>
  </div>
</body>
</html>
