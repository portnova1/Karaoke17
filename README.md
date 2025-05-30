<!DOCTYPE html>
<html lang="ru">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>Караоке Бар 17</title>
  <style>
    body {
      margin: 0;
      font-family: 'Segoe UI', sans-serif;
      background-color: #1a0f2b;
      color: #ffffff;
    }

    header, section {
      padding: 60px 20px;
      max-width: 1200px;
      margin: 0 auto;
    }

    header {
      background: linear-gradient(to bottom right, #2c145f, #4a2d91);
      text-align: center;
    }

    h1 {
      font-size: 48px;
      color: #e6ccff;
    }

    h2 {
      color: #d9b3ff;
      border-bottom: 2px solid #d9b3ff;
      padding-bottom: 10px;
      margin-bottom: 20px;
    }

    .menu-tabs button {
      background: #3b216f;
      color: #fff;
      padding: 10px 20px;
      margin: 5px;
      border: none;
      cursor: pointer;
    }

    .menu-tabs button.active {
      background: #5e35b1;
    }

    .menu-content {
      display: none;
    }

    .menu-content.active {
      display: block;
    }

    .gallery img {
      width: 30%;
      margin: 10px;
      border-radius: 10px;
    }

    .rules, .promotions {
      background-color: #2a1a3f;
      border-radius: 10px;
      padding: 20px;
    }

    .btn-book {
      display: block;
      margin: 40px auto;
      background: #9c27b0;
      color: #fff;
      border: none;
      padding: 15px 30px;
      font-size: 20px;
      cursor: pointer;
      border-radius: 5px;
      text-decoration: none;
    }

    footer {
      background-color: #12081f;
      text-align: center;
      padding: 20px;
    }

    footer a {
      color: #b388ff;
      margin: 0 10px;
      text-decoration: none;
    }

    @media (max-width: 768px) {
      .gallery img {
        width: 90%;
      }
    }
  </style>
</head>
<body>

<header>
  <h1>Караоке Бар 17</h1>
  <p>Добро пожаловать! Мы — стильный караоке-бар с уютной атмосферой и авторской кухней. Идеальное место для вечера с друзьями!</p>
</header>

<section>
  <h2>Меню</h2>
  <div class="menu-tabs">
    <button class="tab-btn active" onclick="showTab('kitchen')">Кухня</button>
    <button class="tab-btn" onclick="showTab('drinks')">Напитки</button>
    <button class="tab-btn" onclick="showTab('desserts')">Десерты</button>
  </div>
  <div id="kitchen" class="menu-content active">
    <p>Добавьте фотографии и описание блюд кухни здесь</p>
    <!-- <img src="photo1.jpg"> -->
  </div>
  <div id="drinks" class="menu-content">
    <p>Добавьте фотографии напитков здесь</p>
  </div>
  <div id="desserts" class="menu-content">
    <p>Добавьте фотографии десертов здесь</p>
  </div>
</section>

<section>
  <h2>Караоке Комнаты</h2>
  <div class="gallery">
    <!-- Пример:
    <img src="room1.jpg">
    <img src="room2.jpg">
    -->
    <p>Добавьте фото комнат здесь</p>
  </div>
</section>

<section class="rules">
  <h2>Правила Заведения</h2>
  <ul>
    <li>Минимальный заказ — 5000₸ на человека.</li>
    <li>Время работы: с 18:00 до 04:00.</li>
    <li>Соблюдайте чистоту и уважайте других гостей.</li>
    <li>Запрещено приносить свои напитки и еду.</li>
  </ul>
</section>

<section class="promotions">
  <h2>Актуальные Акции</h2>
  <ul>
    <li>🎉 Счастливые часы — 20% скидка с 18:00 до 20:00</li>
    <li>🎂 Именинникам — бесплатный десерт и песня в подарок!</li>
    <li>👯‍♀️ Приходи с подругой — получите бокал вина бесплатно!</li>
  </ul>
</section>

<a href="https://wa.me/77001234567" class="btn-book" target="_blank">Забронировать Комнату</a>

<footer>
  <p>Следите за нами в соцсетях:</p>
  <a href="https://instagram.com/yourpage" target="_blank">Instagram</a> |
  <a href="https://t.me/yourpage" target="_blank">Telegram</a>
</footer>

<script>
  function showTab(tabId) {
    document.querySelectorAll('.menu-content').forEach(div => {
      div.classList.remove('active');
    });
    document.querySelectorAll('.tab-btn').forEach(btn => {
      btn.classList.remove('active');
    });
    document.getElementById(tabId).classList.add('active');
    event.target.classList.add('active');
  }
</script>

</body>
</html>
