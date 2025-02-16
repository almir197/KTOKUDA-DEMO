<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>КТО КУДА? | Демо версия</title>
    <style>
        /* Общие стили */
        body {
            font-family: 'Arial', sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f0f2f5;
            color: #333;
        }

        /* Шапка */
        header {
            background-color: #4CAF50;
            color: white;
            padding: 10px 20px;
            display: flex;
            justify-content: space-between;
            align-items: center;
            box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
            position: fixed;
            width: 100%;
            top: 0;
            z-index: 1000;
        }

        header h1 {
            margin: 0;
            font-size: 24px;
            font-weight: bold;
        }

        header nav a {
            color: white;
            text-decoration: none;
            margin-left: 20px;
            font-size: 16px;
            transition: opacity 0.3s;
        }

        header nav a:hover {
            opacity: 0.8;
        }

        /* Основной контент */
        .main-content {
            display: flex;
            margin-top: 60px;
        }

        /* Боковая панель */
        .sidebar {
            width: 250px;
            background-color: white;
            padding: 20px;
            box-shadow: 2px 0 4px rgba(0, 0, 0, 0.1);
            position: fixed;
            height: calc(100vh - 60px);
            overflow-y: auto;
        }

        .sidebar h2 {
            font-size: 18px;
            color: #4CAF50;
            margin-bottom: 15px;
        }

        .sidebar ul {
            list-style-type: none;
            padding: 0;
        }

        .sidebar ul li {
            margin-bottom: 10px;
        }

        .sidebar ul li a {
            color: #333;
            text-decoration: none;
            font-size: 14px;
            transition: color 0.3s;
        }

        .sidebar ul li a:hover {
            color: #4CAF50;
        }

        /* Новостная лента */
        .feed {
            margin-left: 270px;
            flex: 1;
            padding: 20px;
        }

        .post {
            background-color: white;
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
            margin-bottom: 20px;
        }

        .post h3 {
            margin: 0;
            font-size: 18px;
            color: #4CAF50;
        }

        .post p {
            margin: 10px 0;
            font-size: 14px;
            color: #555;
        }

        .post img {
            width: 100%;
            border-radius: 10px;
            margin-top: 10px;
        }

        .post .actions {
            display: flex;
            justify-content: space-between;
            margin-top: 15px;
        }

        .post .actions button {
            background-color: #4CAF50;
            color: white;
            border: none;
            padding: 8px 16px;
            border-radius: 5px;
            cursor: pointer;
            font-size: 14px;
            transition: background-color 0.3s;
        }

        .post .actions button:hover {
            background-color: #45a049;
        }

        /* Правая панель */
        .right-sidebar {
            width: 300px;
            background-color: white;
            padding: 20px;
            box-shadow: -2px 0 4px rgba(0, 0, 0, 0.1);
            position: fixed;
            right: 0;
            height: calc(100vh - 60px);
            overflow-y: auto;
        }

        .right-sidebar h2 {
            font-size: 18px;
            color: #4CAF50;
            margin-bottom: 15px;
        }

        .right-sidebar ul {
            list-style-type: none;
            padding: 0;
        }

        .right-sidebar ul li {
            margin-bottom: 10px;
        }

        .right-sidebar ul li a {
            color: #333;
            text-decoration: none;
            font-size: 14px;
            transition: color 0.3s;
        }

        .right-sidebar ul li a:hover {
            color: #4CAF50;
        }

        /* Футер */
        footer {
            background-color: #333;
            color: white;
            text-align: center;
            padding: 20px;
            margin-top: 20px;
            position: relative;
            bottom: 0;
            width: 100%;
        }

        footer p {
            margin: 0;
            font-size: 14px;
        }

        footer a {
            color: #4CAF50;
            text-decoration: none;
            transition: opacity 0.3s;
        }

        footer a:hover {
            opacity: 0.8;
        }
    </style>
</head>
<body>
    <header>
        <h1>Демо версия КТО КУДА?</h1>
        <nav>
            <a href="#profile">Профиль</a>
            <a href="#events">Мероприятия</a>
            <a href="#chats">Чаты</a>
            <a href="#ai-chat">Общение с ИИ</a>
            <a href="#settings">Настройки</a>
        </nav>
    </header>

    <div class="main-content">
        <!-- Боковая панель -->
        <div class="sidebar">
            <h2>Меню</h2>
            <ul>
                <li><a href="#profile">Профиль</a></li>
                <li><a href="#events">Мероприятия</a></li>
                <li><a href="#chats">Чаты</a></li>
                <li><a href="#ai-chat">Общение с ИИ</a></li>
                <li><a href="#settings">Настройки</a></li>
            </ul>
        </div>

        <!-- Новостная лента -->
        <div class="feed">
            <div class="post">
                <h3>Шопинг в MEGA SILKWAY</h3>
                <p>Группа из 11 человек собирается на шопинг в MEGA SILKWAY в эти выходные. Присоединяйтесь!</p>
                <img src="https://source.unsplash.com/800x400/?shopping,mall" alt="Шопинг">
                <div class="actions">
                    <button>Присоединиться</button>
                    <button>Комментировать</button>
                </div>
            </div>

            <div class="post">
                <h3>Катание на велосипедах</h3>
                <p>Сегодня в 15:00 группа из 9 человек собирается покататься на велосипедах по Президентскому парку.</p>
                <img src="https://source.unsplash.com/800x400/?biking,park" alt="Велосипеды">
                <div class="actions">
                    <button>Присоединиться</button>
                    <button>Комментировать</button>
                </div>
            </div>

            <div class="post">
                <h3>Концерт</h3>
                <p>Концерт популярной группы состоится 16.09 в Астане. Билеты уже в продаже!</p>
                <img src="https://source.unsplash.com/800x400/?concert,music" alt="Концерт">
                <div class="actions">
                    <button>Присоединиться</button>
                    <button>Комментировать</button>
                </div>
            </div>
        </div>

        <!-- Правая панель -->
        <div class="right-sidebar">
            <h2>Рекомендации</h2>
            <ul>
                <li><a href="#event1">Шопинг в MEGA SILKWAY</a></li>
                <li><a href="#event2">Катание на велосипедах</a></li>
                <li><a href="#event3">Концерт</a></li>
            </ul>
        </div>
    </div>

    <!-- Футер -->
    <footer>
        <p>Сайт сделан компанией <a href="#quex">Quex</a>. Основатели: Альмир, Жеткизген и Заир.</p>
    </footer>
</body>
</html>
