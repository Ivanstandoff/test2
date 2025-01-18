<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Rust – Вики о игре</title>
    <link href="https://fonts.googleapis.com/css2?family=Fjalla+One&display=swap" rel="stylesheet">
    <style>
        html {
            scroll-behavior: smooth; /* Плавная прокрутка */
        }
        body {
            background: url('https://cdn.discordapp.com/attachments/1314225469419294780/1330131442646388847/image.png?ex=678cdcf0&is=678b8b70&hm=dedd56087c729808020cb61c8e705b3dc64cbf61156f0514a4b142ad36ee1c2c') no-repeat center center fixed;
            background-size: cover;
            color: #fff;
            font-family: 'Fjalla One', Arial, sans-serif;
            line-height: 1.6;
            margin: 0;
            padding: 0;
            overflow-x: hidden;
        }
        header {
            background-color: rgba(34, 34, 34, 0.9);
            color: #ff0000;
            padding: 1em 0;
            text-align: center;
            position: relative;
            z-index: 2;
        }
        nav ul {
            list-style: none;
            padding: 0;
        }
        nav ul li {
            display: inline;
            margin-right: 1em;
        }
        nav ul li a {
            color: #ff0000;
            text-decoration: none;
            transition: color 0.3s;
        }
        nav ul li a:hover {
            color: #f1c40f;
        }
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 1em;
            background-color: rgba(0, 0, 0, 0.8);
            border-radius: 10px;
            box-shadow: 0 4px 20px rgba(0, 0, 0, 0.5);
            position: relative;
            z-index: 1;
            margin-bottom: 2em;
        }
        h1, h2 {
            color: #ff0000;
            text-shadow: 1px 1px 5px rgba(0, 0, 0, 0.7);
        }
        .image-container {
            display: flex;
            justify-content: center;
            margin: 1em 0;
            position: relative;
        }
        .image-container img {
            max-width: 100%;
            height: auto;
            opacity: 0.5;
            transition: opacity 0.5s;
        }
        .image-container img:hover {
            opacity: 1;
        }
        .hamburger {
            cursor: pointer;
            width: 30px;
            height: 30px;
            margin: 20px;
            position: relative;
            z-index: 2;
        }
        .line {
            width: 100%;
            height: 4px;
            background-color: white;
            margin: 6px 0;
            transition: 0.4s;
        }
        .side-panel {
            height: 100%;
            width: 0;
            position: fixed;
            top: 0;
            left: 0;
            background-color: rgba(51, 51, 51, 0.9);
            overflow-x: hidden;
            transition: 0.5s;
            padding-top: 60px;
            z-index: 1;
        }
        .side-panel a {
            padding: 10px 15px;
            text-decoration: none;
            font-size: 22px;
            color: #818181;
            display: block;
            transition: 0.3s;
        }
        .side-panel a:hover {
            color: #f1c40f;
        }
        .closebtn {
            position: absolute;
            top: 0;
            right: 25px;
            font-size: 36px;
            margin-left: 50px;
            color: #fff;
        }
        .main-content {
            padding-top: 20px;
        }
        table {
            width: 100%;
            border-collapse: collapse;
            margin: 1em 0;
        }
        table, th, td {
            border: 1px solid #fff;
        }
        th, td {
            padding: 10px;
            text-align: center;
        }
        th {
            background-color: rgba(34, 34, 34, 0.8);
        }
    </style>
</head>
<body>
    <div class="hamburger" onclick="togglePanel()">
        <div class="line"></div>
        <div class="line"></div>
        <div class="line"></div>
    </div>
    <div id="sidePanel" class="side-panel">
        <a href="javascript:void(0)" class="closebtn" onclick="togglePanel()">&times;</a>
        <a href="#about">О игре</a>
        <a href="#gameplay">Геймплей</a>
        <a href="#resources">Ресурсы</a>
        <a href="#crafting">Крафтинг</a>
        <a href="#buildings">Строительство</a>
        <a href="#tips">Советы</a>
        <a href="#faq">Часто задаваемые вопросы</a>
    </div>
    <header>
        <h1>Добро пожаловать в Вики по игре Rust</h1>
        <nav>
            <ul>
                <li><a href="#about">О игре</a></li>
                <li><a href="#gameplay">Геймплей</a></li>
                <li><a href="#resources">Ресурсы</a></li>
                <li><a href="#crafting">Крафтинг</a></li>
                <li><a href="#buildings">Строительство</a></li>
                <li><a href="#tips">Советы</a></li>
                <li><a href="#faq">Часто задаваемые вопросы</a></li>
            </ul>
        </nav>
    </header>
    <main class="main-content">
        <section id="about" class="container">
            <h2>О игре</h2>
            <div class="image-container">
                <img src="https://cdn.discordapp.com/attachments/1314225469419294780/1329516092191670292/image.png?ex=678c9a19&is=678b4899&hm=446f26cbb5bc241c7f256d3f2810229e62c6c005ab6fbc73f92f08b0644c274a&" alt="Скриншот геймплея Rust">
            </div>
            <p>Rust - многопользовательская онлайн-игра на выживание от компании Facepunch Studios. Игроки должны выжить в дикой природе, используя
               свои навыки и ресурсы. Игра сочетает в себе элементы строительства, крафтинга и PvP-сражений.</p>
            <p>Главным элементом игры является реальное взаимодействие между игроками, которое может включать как сотрудничество в группах и совместную
               постройку укреплений, так и враждебность, рейдерство и битвы за ресурсы. Все эти элементы создают уникальный и захватывающий геймплей,
               который удерживает игроков на долгие часы.</p>
        </section>
        <section id="gameplay" class="container">
            <h2>Геймплей</h2>
            <div class="image-container">
                <img src="https://cdn.discordapp.com/attachments/1314225469419294780/1328826537763672074/image.png?ex=678c1227&is=678ac0a7&hm=b0b379555250e86f9bda02c46af8e7568231317510ffbd90738f07276daff128&" alt="Бой в Rust">
            </div>
            <p>Rust предлагает игрокам динамичный геймплей, сочетающий элементы выживания, строительства и сражений. Игроки начинают с минимальным
               набором инструментов и должны искать ресурсы, чтобы строить укрытия и изготавливать оружие.</p>
            <h3>Пища и Вода</h3>
            <p>Пища и вода жизненно необходимы для выживания. Игроки должны охотиться, собирать ягоды и искать источники воды, чтобы удовлетворить свои
               базовые потребности. На острове Rust можно встретить различные виды животных, таких как олени, кабаны и волки. Охота на них позволит
               собрать мясо, кожу и жир, необходимые для крафтинга и питания.</p>
            <h3>Боевые действия</h3>
            <p>Игроки могут сражаться с другими игроками или NPC, используя разнообразное оружие и ловушки. В PvP режимах важно уметь хорошо стрелять и прятаться.
               В Rust есть множество видов оружия, от простых дубинок и луков до огнестрельного оружия, такого как пистолеты, автоматические винтовки и дробовики.
               Создание и улучшение оружия является ключевым аспектом для выживания и защиты своих ресурсов.</p>
            <h3>Сбор ресурсов</h3>
            <p>Сбор ресурсов является важным элементом геймплея. Игроки могут добывать дерево, камень, металлы и другие материалы, необходимые для строительства
               и изготовления предметов. Процесс добычи осуществляется с помощью различных инструментов, таких как топоры и кирки. Игроки также могут находить
               ресурсы путём обыска разрушенных баз и заброшенных построек.</p>
            <h3>Крафтинг</h3>
            <p>Крафтинг - важная часть игры. В Rust существует обширная система крафтинга, позволяющая игрокам создавать невероятный ассортимент предметов,
               начиная от простых орудий и заканчивая сложными механизмами. Игроки могут создавать всё: от оружия и брони до строительных материалов и мебели.</p>
        </section>
        <section id="resources" class="container">
            <h2>Ресурсы</h2>
            <p>В Rust существует множество ресурсов, которые игроки могут собирать и использовать для выживания и строительства. Вот некоторые из них:</p>
            <ul>
                <li><strong>Дерево:</strong> Основной ресурс, используемый для строительства и крафта.</li>
                <li><strong>Камень:</strong> Используется для создания инструментов и строительства.</li>
                <li><strong>Металлы:</strong> Включает в себя железо и серу, необходимые для создания более сложных предметов.</li>
                <li><strong>Пища:</strong> Включает мясо, ягоды и другие съедобные предметы.</li>
                <li><strong>Вода:</strong> Необходима для выживания, может быть найдена в реках и озерах.</li>
            </ul>
            <div class="image-container">
                <img src="https://cdn.discordapp.com/attachments/1314225469419294780/1330107353160486934/image.png?ex=678cc681&is=678b7501&hm=ca5d62c144172afdc84304546757225d31fb94db7de49041216da6fe148de1fb&" alt="Ресурсы в Rust">
            </div>
        </section>
        <section id="crafting" class="container">
            <h2>Крафтинг</h2>
            <p>Крафтинг в Rust позволяет игрокам создавать различные предметы, которые помогут им выжить в суровых условиях. Игроки могут создавать оружие, инструменты,
               броню и даже строить свои базы. Система крафтинга очень обширна и требует от игроков собирать ресурсы и изучать рецепты.</p>
            <div class="image-container">
                <img src="https://cdn.discordapp.com/attachments/1275898985307181271/1330144274465161287/fP5L87x5POo.png?ex=678ce8e3&is=678b9763&hm=68d20332bb59687e0ac5a97139685666cf60e5fdca1a9b3870a28 e8d60ffc482&" alt="Крафт инг в Rust">
            </div>
            <p>Крафтинг включает в себя создание различных предметов, таких как инструменты, оружие и строительные материалы. Игроки могут комбинировать ресурсы для создания более сложных предметов, что позволяет им адаптироваться к различным условиям игры.</p>
        </section>
        <section id="buildings" class="container">
            <h2>Строительство</h2>
            <p>Строительство в Rust является ключевым элементом выживания. Игроки могут создавать свои базы, используя собранные ресурсы. Базы могут варьироваться от простых укрытий до сложных укреплений с защитными механизмами.</p>
            <div class="image-container">
                <img src="https://cdn.discordapp.com/attachments/1314225469419294780/1330107353160486934/image.png?ex=678cc681&is=678b7501&hm=ca5d62c144172afdc84304546757225d31fb94db7de49041216da6fe148de1fb&" alt="Строительство в Rust">
            </div>
            <p>Игроки могут использовать различные материалы для строительства, включая дерево, камень и металл. Каждый материал имеет свои характеристики, влияющие на прочность и защиту построек.</p>
        </section>
        <section id="tips" class="container">
            <h2>Советы</h2>
            <p>Вот несколько советов для успешного выживания в Rust:</p>
            <ul>
                <li>Собирайте ресурсы постоянно, чтобы не остаться без необходимых материалов.</li>
                <li>Стройте базу в безопасном месте, вдали от других игроков.</li>
                <li>Используйте ловушки и защитные механизмы для защиты своей базы.</li>
                <li>Сотрудничайте с другими игроками, чтобы увеличить шансы на выживание.</li>
                <li>Изучайте рецепты крафта, чтобы создавать более мощные предметы.</li>
            </ul>
        </section>
        <section id="faq" class="container">
            <h2>Часто задаваемые вопросы</h2>
            <h3>Как начать играть в Rust?</h3>
            <p>Для начала игры вам нужно купить Rust в Steam и установить его на свой компьютер. После этого вы можете присоединиться к серверу и начать свое приключение.</p>
            <h3>Можно ли играть в Rust в одиночку?</h3>
            <p>Да, в Rust можно играть в одиночку, но это будет сложнее, чем в команде. Рекомендуется находить союзников для повышения шансов на выживание.</p>
            <h3>Как защитить свою базу?</h3>
            <p>Для защиты базы используйте прочные материалы, устанавливайте двери и ловушки, а также следите за окружающей территорией.</p>
        </section>
    </main>
    <script>
        function togglePanel() {
            var panel = document.getElementById("sidePanel");
            if (panel.style.width === "250px") {
                panel.style.width = "0";
            } else {
                panel.style.width = "250px";
            }
        }
    </script>
</body>
</html>
