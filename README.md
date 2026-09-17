<!DOCTYPE html>
<html lang="fa" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>ArmoLand | Minecraft Server</title>

    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: Tahoma, Arial, sans-serif;
        }

        body {
            background: #080808;
            color: #fff;
            min-height: 100vh;
        }

        header {
            position: sticky;
            top: 0;
            z-index: 100;
            background: rgba(8, 8, 8, 0.95);
            border-bottom: 1px solid #b8860b;
            padding: 18px 7%;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .logo {
            color: #d4af37;
            font-size: 28px;
            font-weight: 900;
            letter-spacing: 1px;
        }

        nav {
            display: flex;
            gap: 25px;
        }

        nav a {
            color: #ddd;
            text-decoration: none;
            transition: 0.3s;
            font-weight: bold;
        }

        nav a:hover {
            color: #d4af37;
        }

        .hero {
            min-height: 85vh;
            display: flex;
            justify-content: center;
            align-items: center;
            text-align: center;
            padding: 40px 20px;
            background:
                radial-gradient(circle at center, rgba(212,175,55,0.12), transparent 45%),
                #080808;
        }

        .hero-content {
            max-width: 850px;
        }

        .hero h1 {
            font-size: clamp(55px, 10vw, 110px);
            color: #d4af37;
            font-weight: 1000;
            text-shadow: 0 0 30px rgba(212,175,55,0.25);
            margin-bottom: 15px;
        }

        .hero h2 {
            font-size: clamp(22px, 4vw, 38px);
            margin-bottom: 20px;
        }

        .hero p {
            color: #aaa;
            font-size: 18px;
            line-height: 2;
            margin-bottom: 30px;
        }

        .buttons {
            display: flex;
            justify-content: center;
            gap: 15px;
            flex-wrap: wrap;
        }

        .btn {
            display: inline-block;
            padding: 14px 30px;
            border-radius: 8px;
            text-decoration: none;
            font-weight: bold;
            transition: 0.3s;
        }

        .btn-gold {
            background: #d4af37;
            color: #080808;
        }

        .btn-gold:hover {
            background: #f0cf55;
            transform: translateY(-3px);
        }

        .btn-dark {
            border: 1px solid #d4af37;
            color: #d4af37;
        }

        .btn-dark:hover {
            background: #d4af37;
            color: #080808;
            transform: translateY(-3px);
        }

        section {
            padding: 90px 7%;
        }

        .section-title {
            text-align: center;
            margin-bottom: 45px;
        }

        .section-title h2 {
            color: #d4af37;
            font-size: 38px;
            margin-bottom: 12px;
        }

        .section-title p {
            color: #888;
        }

        .cards {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(230px, 1fr));
            gap: 22px;
            max-width: 1100px;
            margin: auto;
        }

        .card {
            background: #101010;
            border: 1px solid #292929;
            border-radius: 14px;
            padding: 30px;
            text-align: center;
            transition: 0.3s;
        }

        .card:hover {
            transform: translateY(-7px);
            border-color: #d4af37;
            box-shadow: 0 10px 35px rgba(212,175,55,0.08);
        }

        .card .icon {
            font-size: 42px;
            margin-bottom: 15px;
        }

        .card h3 {
            color: #d4af37;
            margin-bottom: 12px;
            font-size: 23px;
        }

        .card p {
            color: #999;
            line-height: 1.8;
        }

        .server-box {
            max-width: 750px;
            margin: auto;
            background: linear-gradient(145deg, #121212, #090909);
            border: 1px solid #d4af37;
            border-radius: 18px;
            padding: 40px;
            text-align: center;
        }

        .server-ip {
            background: #050505;
            border: 1px solid #292929;
            padding: 18px;
            border-radius: 10px;
            margin: 25px 0;
            font-size: 20px;
            color: #d4af37;
            direction: ltr;
        }

        .status {
            color: #65d46e;
            font-weight: bold;
        }

        footer {
            border-top: 1px solid #292929;
            background: #050505;
            padding: 35px 20px;
            text-align: center;
            color: #777;
        }

        footer strong {
            color: #d4af37;
        }

        @media (max-width: 700px) {
            header {
                flex-direction: column;
                gap: 15px;
            }

            nav {
                gap: 14px;
                flex-wrap: wrap;
                justify-content: center;
            }

            section {
                padding: 65px 5%;
            }

            .server-box {
                padding: 25px 15px;
            }
        }
    </style>
</head>

<body>

<header>
    <div class="logo">ARMOLAND</div>

    <nav>
        <a href="#home">خانه</a>
        <a href="#features">ویژگی‌ها</a>
        <a href="#server">سرور</a>
        <a href="#about">درباره ما</a>
    </nav>
</header>

<section class="hero" id="home">
    <div class="hero-content">
        <h1>ARMOLAND</h1>

        <h2>دنیای جدید ماینکرفت</h2>

        <p>
            به سرور ArmoLand خوش آمدید؛
            جایی برای ساختن، رقابت کردن و تجربه کردن یک دنیای متفاوت.
        </p>

        <div class="buttons">
            <a href="#server" class="btn btn-gold">ورود به سرور</a>
            <a href="#features" class="btn btn-dark">بیشتر بدانید</a>
        </div>
    </div>
</section>

<section id="features">
    <div class="section-title">
        <h2>ویژگی‌های ArmoLand</h2>
        <p>چیزهایی که در سرور منتظر شماست</p>
    </div>

    <div class="cards">

        <div class="card">
            <div class="icon">⚔️</div>
            <h3>رقابت</h3>
            <p>
                با بازیکنان دیگر رقابت کنید و جایگاه خود را در سرور پیدا کنید.
            </p>
        </div>

        <div class="card">
            <div class="icon">💰</div>
            <h3>اقتصاد</h3>
            <p>
                خرید و فروش کنید، پول جمع کنید و اقتصاد خودتان را بسازید.
            </p>
        </div>

        <div class="card">
            <div class="icon">🏆</div>
            <h3>رنک‌ها</h3>
            <p>
                با پیشرفت در سرور به رنک‌های مختلف دسترسی پیدا کنید.
            </p>
        </div>

        <div class="card">
            <div class="icon">🎁</div>
            <h3>جوایز</h3>
            <p>
                با فعالیت در سرور جوایز و پاداش‌های مختلف دریافت کنید.
            </p>
        </div>

    </div>
</section>

<section id="server">
    <div class="section-title">
        <h2>اطلاعات سرور</h2>
        <p>آماده‌ای وارد ArmoLand بشی؟</p>
    </div>

    <div class="server-box">

        <h2>ARMOLAND NETWORK</h2>

        <div class="server-ip">
            IP: YOUR-SERVER-IP
        </div>

        <p class="status">
            ● سرور آنلاین
        </p>

        <br>

        <a href="#" class="btn btn-gold">
            کپی IP سرور
        </a>

    </div>
</section>

<section id="about">
    <div class="section-title">
        <h2>درباره ArmoLand</h2>
        <p>یک دنیای ساخته‌شده برای بازیکنان</p>
    </div>

    <div class="server-box">
        <p style="color:#aaa; line-height:2;">
            ArmoLand یک سرور ماینکرفت با هدف ساختن یک تجربه متفاوت،
            سرگرم‌کننده و حرفه‌ای برای بازیکنان است.
            اینجا تازه شروع ماجراست...
        </p>
    </div>
</section>

<footer>
    <p>
        © 2026 <strong>ArmoLand</strong> — All Rights Reserved
    </p>
</footer>

</body>
</html>
