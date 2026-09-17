<!DOCTYPE html>
<html lang="fa" dir="rtl">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>ArmoLand | Minecraft Server</title>

<style>
*{
    margin:0;
    padding:0;
    box-sizing:border-box;
    font-family:Tahoma,Arial,sans-serif;
}

html{
    scroll-behavior:smooth;
}

body{
    background:#070707;
    color:#fff;
}

header{
    position:sticky;
    top:0;
    z-index:1000;
    background:rgba(7,7,7,.96);
    border-bottom:1px solid #b8942e;
    padding:18px 7%;
    display:flex;
    justify-content:space-between;
    align-items:center;
}

.logo{
    color:#d4af37;
    font-size:29px;
    font-weight:900;
    letter-spacing:2px;
}

nav{
    display:flex;
    gap:28px;
}

nav a{
    color:#ddd;
    text-decoration:none;
    font-weight:bold;
    transition:.25s;
}

nav a:hover{
    color:#d4af37;
}

.hero{
    min-height:88vh;
    display:flex;
    align-items:center;
    justify-content:center;
    text-align:center;
    padding:50px 20px;
    background:
        radial-gradient(circle at 50% 45%,rgba(212,175,55,.15),transparent 38%),
        linear-gradient(#080808,#050505);
}

.hero-content{
    max-width:900px;
}

.badge{
    display:inline-block;
    border:1px solid #b8942e;
    color:#d4af37;
    padding:8px 18px;
    border-radius:30px;
    margin-bottom:25px;
    font-size:14px;
}

.hero h1{
    font-size:clamp(55px,11vw,115px);
    color:#d4af37;
    font-weight:1000;
    letter-spacing:4px;
    text-shadow:0 0 35px rgba(212,175,55,.22);
}

.hero h2{
    margin-top:5px;
    font-size:clamp(22px,4vw,38px);
}

.hero p{
    color:#999;
    line-height:2;
    font-size:17px;
    margin:22px auto 32px;
    max-width:700px;
}

.buttons{
    display:flex;
    justify-content:center;
    gap:14px;
    flex-wrap:wrap;
}

.btn{
    border-radius:9px;
    padding:14px 30px;
    text-decoration:none;
    font-weight:bold;
    cursor:pointer;
    transition:.25s;
    border:none;
    display:inline-block;
}

.gold{
    background:#d4af37;
    color:#080808;
}

.gold:hover{
    background:#f0ce52;
    transform:translateY(-3px);
}

.dark{
    border:1px solid #d4af37;
    color:#d4af37;
    background:transparent;
}

.dark:hover{
    background:#d4af37;
    color:#080808;
    transform:translateY(-3px);
}

section{
    padding:90px 7%;
}

.title{
    text-align:center;
    margin-bottom:45px;
}

.title h2{
    color:#d4af37;
    font-size:38px;
    margin-bottom:10px;
}

.title p{
    color:#777;
}

.cards{
    max-width:1150px;
    margin:auto;
    display:grid;
    grid-template-columns:repeat(auto-fit,minmax(220px,1fr));
    gap:20px;
}

.card{
    background:#101010;
    border:1px solid #252525;
    border-radius:15px;
    padding:32px 25px;
    text-align:center;
    transition:.3s;
}

.card:hover{
    transform:translateY(-7px);
    border-color:#d4af37;
    box-shadow:0 10px 35px rgba(212,175,55,.08);
}

.icon{
    font-size:43px;
    margin-bottom:16px;
}

.card h3{
    color:#d4af37;
    font-size:22px;
    margin-bottom:12px;
}

.card p{
    color:#999;
    line-height:1.9;
}

.server-box{
    max-width:800px;
    margin:auto;
    padding:42px;
    text-align:center;
    background:linear-gradient(145deg,#121212,#090909);
    border:1px solid #b8942e;
    border-radius:18px;
}

.server-box h2{
    color:#d4af37;
    margin-bottom:20px;
}

.ip-box{
    direction:ltr;
    background:#050505;
    border:1px solid #292929;
    border-radius:10px;
    padding:18px;
    margin:20px 0;
    color:#d4af37;
    font-size:20px;
    font-weight:bold;
}

.status{
    color:#5ddd68;
    font-weight:bold;
    margin-bottom:25px;
}

.about-text{
    color:#999;
    line-height:2.2;
    font-size:16px;
}

footer{
    border-top:1px solid #242424;
    background:#050505;
    text-align:center;
    padding:35px 20px;
    color:#666;
}

footer strong{
    color:#d4af37;
}

.toast{
    position:fixed;
    bottom:25px;
    left:50%;
    transform:translateX(-50%) translateY(100px);
    background:#d4af37;
    color:#080808;
    padding:13px 25px;
    border-radius:9px;
    font-weight:bold;
    opacity:0;
    transition:.3s;
    z-index:9999;
}

.toast.show{
    opacity:1;
    transform:translateX(-50%) translateY(0);
}

@media(max-width:700px){
    header{
        flex-direction:column;
        gap:15px;
    }

    nav{
        gap:14px;
        flex-wrap:wrap;
        justify-content:center;
    }

    section{
        padding:65px 5%;
    }

    .server-box{
        padding:28px 17px;
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

        <div class="badge">MINECRAFT NETWORK</div>

        <h1>ARMOLAND</h1>

        <h2>دنیای جدید ماینکرفت</h2>

        <p>
            به ArmoLand خوش آمدید؛
            یک سرور ماینکرفت برای ساختن، رقابت، پیشرفت و تجربه یک دنیای متفاوت.
        </p>

        <div class="buttons">
            <a href="#server" class="btn gold">ورود به سرور</a>
            <a href="#features" class="btn dark">ویژگی‌های سرور</a>
        </div>

    </div>

</section>


<section id="features">

    <div class="title">
        <h2>ویژگی‌های ArmoLand</h2>
        <p>چیزهایی که در سرور منتظر شماست</p>
    </div>

    <div class="cards">

        <div class="card">
            <div class="icon">⚔️</div>
            <h3>رقابت</h3>
            <p>
                با بازیکنان دیگر رقابت کنید و جایگاه خودتان را در ArmoLand بسازید.
            </p>
        </div>

        <div class="card">
            <div class="icon">💰</div>
            <h3>اقتصاد</h3>
            <p>
                خرید و فروش کنید، پول جمع کنید و در اقتصاد سرور پیشرفت کنید.
            </p>
        </div>

        <div class="card">
            <div class="icon">🏆</div>
            <h3>رنک‌ها</h3>
            <p>
                با رنک‌های مختلف امکانات و ویژگی‌های بیشتری دریافت کنید.
            </p>
        </div>

        <div class="card">
            <div class="icon">🎁</div>
            <h3>جوایز</h3>
            <p>
                با فعالیت و پیشرفت در سرور جوایز مختلف دریافت کنید.
            </p>
        </div>

    </div>

</section>


<section id="server">

    <div class="title">
        <h2>اطلاعات سرور</h2>
        <p>آماده‌ای وارد ArmoLand بشی؟</p>
    </div>

    <div class="server-box">

        <h2>ARMOLAND NETWORK</h2>

        <div class="ip-box">
            armoland.mcsh.io
        </div>

        <div class="status">
            ● سرور آنلاین
        </div>

        <button class="btn gold" onclick="copyIP()">
            کپی IP سرور
        </button>

    </div>

</section>


<section id="about">

    <div class="title">
        <h2>درباره ArmoLand</h2>
        <p>یک دنیای ساخته‌شده برای بازیکنان</p>
    </div>

    <div class="server-box">

        <p class="about-text">
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


<div class="toast" id="toast">
    IP سرور کپی شد ✓
</div>


<script>

function copyIP(){

    const ip = "armoland.mcsh.io";

    navigator.clipboard.writeText(ip).then(function(){

        const toast = document.getElementById("toast");

        toast.classList.add("show");

        setTimeout(function(){
            toast.classList.remove("show");
        },2000);

    });

}

</script>

</body>
</html>
