<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Grafick-effect-c-</title>
    <style>
        /* Загальні стилі */
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background: linear-gradient(135deg, #1e3c72, #2a5298);
            color: #fff;
            text-align: center;
            overflow-x: hidden;
        }

        /* Заголовок */
        header {
            background: #111;
            padding: 20px;
            font-size: 24px;
            font-weight: bold;
            text-transform: uppercase;
            letter-spacing: 2px;
            animation: slideDown 1s ease-out;
        }

        header:hover {
            color: #ffcc00;
            text-shadow: 0 0 10px #ffcc00;
            transition: all 0.5s ease;
        }

        /* Основний блок */
        main {
            padding: 50px;
        }

        h1 {
            font-size: 48px;
            margin-bottom: 20px;
            animation: fadeIn 2s ease-out;
            transition: all 0.5s ease;
        }

        h1:hover {
            transform: scale(1.2);
            color: #ffcc00;
            text-shadow: 0 0 15px #ffcc00;
        }

        p {
            font-size: 18px;
            line-height: 1.6;
            margin-bottom: 30px;
            animation: fadeIn 2.5s ease-out;
            transition: color 0.3s ease;
        }

        p:hover {
            color: #ffcc00;
        }

        /* Кнопка */
        a {
            text-decoration: none;
            color: #ffcc00;
            font-weight: bold;
            border: 2px solid #ffcc00;
            padding: 10px 20px;
            border-radius: 5px;
            transition: all 0.3s ease;
            display: inline-block;
            animation: bounce 3s infinite;
        }

        a:hover {
            background: #ffcc00;
            color: #111;
            transform: rotate(5deg) scale(1.1);
            box-shadow: 0 0 20px #ffcc00;
        }

        /* Футер */
        footer {
            background: #111;
            padding: 10px;
            font-size: 14px;
            position: fixed;
            bottom: 0;
            width: 100%;
        }

        /* Анімації */
        @keyframes fadeIn {
            from {
                opacity: 0;
            }
            to {
                opacity: 1;
            }
        }

        @keyframes slideDown {
            from {
                transform: translateY(-100%);
            }
            to {
                transform: translateY(0);
            }
        }

        @keyframes bounce {
            0%, 20%, 50%, 80%, 100% {
                transform: translateY(0);
            }
            40% {
                transform: translateY(-10px);
            }
            60% {
                transform: translateY(-5px);
            }
        }

        /* Анімовані "бульбашки" */
        .bubble {
            position: absolute;
            background: rgba(255, 255, 255, 0.1);
            border-radius: 50%;
            animation: float 8s infinite ease-in-out;
            z-index: -1;
        }

        .bubble:nth-child(1) {
            width: 100px;
            height: 100px;
            left: 10%;
            animation-duration: 6s;
            animation-delay: 0s;
        }

        .bubble:nth-child(2) {
            width: 120px;
            height: 120px;
            left: 30%;
            animation-duration: 8s;
            animation-delay: 2s;
        }

        .bubble:nth-child(3) {
            width: 80px;
            height: 80px;
            left: 50%;
            animation-duration: 10s;
            animation-delay: 4s;
        }

        .bubble:nth-child(4) {
            width: 140px;
            height: 140px;
            left: 70%;
            animation-duration: 12s;
            animation-delay: 6s;
        }

        .bubble:nth-child(5) {
            width: 60px;
            height: 60px;
            left: 90%;
            animation-duration: 14s;
            animation-delay: 8s;
        }

        @keyframes float {
            0% {
                transform: translateY(100vh) scale(0.8);
                opacity: 0;
            }
            50% {
                opacity: 0.5;
            }
            100% {
                transform: translateY(-200px) scale(1);
                opacity: 0;
            }
        }
    </style>
</head>
<body>
    <header>
        Grafick-effect-c-
    </header>
    <main>
        <h1>Welcome to the Grafick-effect-c- Project!</h1>
        <p>Create amazing graphical effects for C++ and more. This is an open-source project aimed at simplifying development with graphical tools.</p>
        <a href="https://github.com/TimaOst1uK/Grafick-effect-c-" target="_blank">View on GitHub</a>
    </main>

    <!-- Додані анімовані бульбашки -->
    <div class="bubble"></div>
    <div class="bubble"></div>
    <div class="bubble"></div>
    <div class="bubble"></div>
    <div class="bubble"></div>

    <footer>
        &copy; 2024 Grafick-effect-c- Team
    </footer>
</body>
</html>
