<!DOCTYPE html><html lang="uk">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Вакумний масажер зі знижкою -45%</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      margin: 0;
      padding: 0;
      background: #fff0f5;
      color: #333;
    }
    .container {
      max-width: 600px;
      margin: 0 auto;
      padding: 20px;
    }
    .hero {
      text-align: center;
      padding: 20px;
    }
    .hero img {
      width: 100%;
      max-width: 300px;
    }
    h1 {
      font-size: 26px;
      margin: 10px 0;
    }
    .price {
      font-size: 24px;
      color: #e91e63;
      margin: 10px 0;
    }
    .price del {
      color: #888;
      margin-left: 10px;
    }
    .btn {
      background: #ff4081;
      color: white;
      border: none;
      padding: 12px 24px;
      font-size: 18px;
      border-radius: 8px;
      cursor: pointer;
      margin: 20px 0;
    }
    .features {
      background: #fff;
      padding: 20px;
      border-radius: 8px;
      margin-top: 20px;
    }
    .features p {
      margin: 8px 0;
      font-size: 16px;
    }
    .timer {
      font-weight: bold;
      color: #d32f2f;
    }
  </style>
</head>
<body>
  <div class="container">
    <div class="hero">
      <h1>Портативний Вакумний масажер</h1>
      <img src="https://via.placeholder.com/300x300?text=Massage+Gun" alt="Вібромасажер">
      <div class="price">
        499 грн <del>907 грн</del>
      </div>
      <button class="btn" onclick="window.location.href='https://t.me/yourshopbot'">КУПИТИ</button>
      <div class="timer">Акція закінчиться через: <span id="countdown"></span></div>
    </div>
    <div class="features">
      <p>✅ 12 рівнів</p>
      <p>✅ 6 режимів швидкості</p>
      <p>✅ До 3200 об/хв</p>
      <p>✅ Безшумна робота</p>
      <p>✅ Компактний та легкий</p>
    </div>
  </div>
  <script>
    // Countdown Timer (3 години від моменту завантаження)
    const countdownEl = document.getElementById('countdown');
    const endTime = new Date(Date.now() + 3 * 60 * 60 * 1000);function updateCountdown() {
  const now = new Date();
  const diff = endTime - now;
  if (diff <= 0) {
    countdownEl.textContent = 'Акція завершена';
    return;
  }
  const hours = String(Math.floor(diff / (1000 * 60 * 60))).padStart(2, '0');
  const minutes = String(Math.floor((diff % (1000 * 60 * 60)) / (1000 * 60))).padStart(2, '0');
  const seconds = String(Math.floor((diff % (1000 * 60)) / 1000)).padStart(2, '0');
  countdownEl.textContent = `${hours}:${minutes}:${seconds}`;
}

updateCountdown();
setInterval(updateCountdown, 1000);

  </script>
</body>
</html>
