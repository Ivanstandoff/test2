<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Counter-Strike 2</title>
    <style>
        body {
            margin: 0;
            font-family: Arial, sans-serif;
            color: #fff;
            background: url('https://cdn.discordapp.com/attachments/1314225469419294780/1330160093840408649/pic-20230322-3840x2160-5802885889.png?ex=678cf79f&is=678ba61f&hm=f9a895ef5315d359eed074fcd38443f7ab34de338c12f1d7d60186a969d99a50') no-repeat center center fixed;
            background-size: cover;
            animation: fadeIn 1s ease-in;
        }

        @keyframes fadeIn {
            from { opacity: 0; }
            to { opacity: 1; }
        }

        header {
            background: rgba(0, 0, 0, 0.7);
            padding: 20px;
            text-align: center;
            animation: slideDown 0.5s ease-in;
        }

        @keyframes slideDown {
            from { transform: translateY(-100%); }
            to { transform: translateY(0); }
        }

        nav a {
            color: #fff;
            margin: 0 15px;
            text-decoration: none;
            font-weight: bold;
            transition: color 0.3s;
        }

        nav a:hover {
            color: #ffcc00;
        }

        .container {
            width: 80%;
            margin: auto;
            overflow: hidden;
            padding: 20px;
        }

        .main-content {
            display: flex;
            flex-direction: column;
            align-items: center;
            margin: 20px 0;
        }

        .game-info {
            background: rgba(0, 0, 0, 0.8);
            padding: 20px;
            border-radius: 5px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.5);
            width: 100%;
            max-width: 800px;
            margin: 20px 0;
            animation: zoomIn 0.5s ease-in;
        }

        @keyframes zoomIn {
            from { transform: scale(0); }
            to { transform: scale(1); }
        }

        img {
            max-width: 100%;
            height: auto;
            border-radius: 5px;
            margin: 10px 0;
        }

        footer {
            text-align: center;
            padding: 10px 0;
            background: rgba(0, 0, 0, 0.7);
            position: relative;
            bottom: 0;
            width: 100%;
        }

        .link-button {
            display: inline-block;
            padding: 10px 20px;
            background: #ffcc00;
            color: #333;
            text-decoration: none;
            border-radius: 5px;
            transition: background 0.3s;
        }

        .link-button:hover {
            background: #e6b800;
        }
    </style>
</head>
<body>

<header>
    <h1>Counter-Strike 2</h1>
    <nav>
        <a href="#about">О игре</a>
        <a href="#features">Особенности</a>
        <a href="#gallery">Галерея</a>
        <a href="#download" class="link-button">Скачать игру</a>
    </nav>
</header>

<div class="container">
    <div class="main-content">
        <section id="about" class="game-info">
            <h2>О игре</h2>
            <p>Counter-Strike 2 — это многопользовательская игра в жанре шутера от первого лица, разработанная компанией Valve. Игра является продолжением популярной серии Counter-Strike и предлагает новые механики, улучшенную графику и обновленный игровой процесс.</p>
            <img src="https://cdn.discordapp.com/attachments/1314225469419294780 /1330159866999865344/Counter-strike_2.png?ex=678cf769&is=678ba5e9&hm=89eaffaf474abac144c715e4d7fb2db9e0d51bfca3ee3cf08bfffb0616551d3a&" alt="Counter-Strike 2">
        </section>

        <section id="features" class="game-info">
            <h2>Особенности</h2>
            <ul>
                <li>Новая графика и улучшенные текстуры</li>
                <li>Обновленный игровой процесс и механики</li>
                <li>Поддержка новых карт и режимов игры</li>
                <li>Интеграция с Steam и поддержка кроссплатформенной игры</li>
            </ul>
            <img src="https://cdn.discordapp.com/attachments/1314225469419294780/1330159866999865344/Counter-strike_2.png?ex=678cf769&is=678ba5e9&hm=89eaffaf474abac144c715e4d7fb2db9e0d51bfca3ee3cf08bfffb0616551d3a&" alt="Особенности Counter-Strike 2">
        </section>

        <section id="gallery" class="game-info">
            <h2>Галерея</h2>
            <img src="https://cdn.discordapp.com/attachments/1314225469419294780/1330159866999865344/Counter-strike_2.png?ex=678cf769&is=678ba5e9&hm=89eaffaf474abac144c715e4d7fb2db9e0d51bfca3ee3cf08bfffb0616551d3a&" alt="Галерея Counter-Strike 2">
            <img src="https://cdn.discordapp.com/attachments/1314225469419294780/1330160093840408649/pic-20230322-3840x2160-5802885889.png?ex=678cf79f&is=678ba61f&hm=f9a895ef5315d359eed074fcd38443f7ab34de338c12f1d7d60186a969d99a50&" alt="Галерея Counter-Strike 2">
        </section>
    </div>
</div>

<footer>
    <p>&copy; 2023 Counter-Strike 2 Fan Site</p>
    <a href="https://store.steampowered.com/app/730/CounterStrike_Global_Offensive/" class="link-button">Перейти к игре</a>
</footer>

</body>
</html>
